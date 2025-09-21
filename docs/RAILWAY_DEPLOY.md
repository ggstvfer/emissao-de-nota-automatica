# Deploy no Railway

## ✅ Conta Criada - Próximos Passos

### ⚠️ Importante: Docker + PostgreSQL

**Quando você usa Dockerfile customizado, o Railway NÃO cria automaticamente o PostgreSQL!**

Você precisa adicionar o PostgreSQL MANUALMENTE após conectar o repositório.

### Passo 1: Conectar Repositório GitHub

1. Acesse [Railway Dashboard](https://railway.app/dashboard)
2. Clique em **"New Project"**
3. Selecione **"Deploy from GitHub repo"**
4. **Permita acesso** ao Railway na sua conta GitHub
5. **Procure e selecione** o repositório `emissao-de-nota-automatica`
6. Clique em **"Deploy"**

### Passo 2: Aguardar Deploy Inicial (Sem Banco)

Railway irá:
- ✅ Detectar automaticamente o **Dockerfile**
- ❌ **NÃO CRIARÁ** o PostgreSQL automaticamente (por causa do Docker customizado)
- ✅ Fará deploy da aplicação (mas vai falhar por falta de DATABASE_URL)

### Passo 3: CRIAR PostgreSQL MANUALMENTE

**Após o deploy inicial (que vai falhar):**

1. No painel lateral, clique em **"+"** (Add Service)
2. Selecione **"PostgreSQL"**
3. Clique em **"Add"**
4. Aguarde o PostgreSQL ser criado

### Passo 3: Verificar PostgreSQL

Após o deploy inicial:

1. **Verifique se o PostgreSQL foi criado:**
   - Vá para **"Services"** no painel lateral
   - Deve haver um serviço **"PostgreSQL"** listado
   - Se não houver, clique em **"+"** e adicione **"PostgreSQL"**

2. **Verifique a DATABASE_URL:**
   - No serviço da aplicação, vá para **"Variables"**
   - Procure por **"DATABASE_URL"** (deve ser criada automaticamente)
   - Se não existir, copie do serviço PostgreSQL

### Passo 4: Configurar Variáveis de Ambiente

No painel do Railway, vá para **"Variables"** do seu serviço da aplicação e adicione:

```bash
JWT_SECRET=ruWyk96giZUzm89WTO8NmfTcjCiPSj0qkfdvIVxcs9M=
NODE_ENV=production
METRICS_ENABLED=1
```

**⚠️ Importante:** A `DATABASE_URL` deve aparecer automaticamente. Se não aparecer:
1. Vá no serviço PostgreSQL
2. Copie a `DATABASE_URL` de lá
3. Cole no serviço da aplicação

### Passo 4: Redeploy com Variáveis

Após adicionar as variáveis:
1. Railway fará **redeploy automático**
2. Monitore em **"Deployments"**
3. Aguarde conclusão

### Passo 5: Verificar Deploy

Quando deploy terminar:
1. **Clique na URL** gerada pelo Railway (ex: `https://emissao-de-nota-automatica.up.railway.app`)
2. **Teste os endpoints:**
   - `GET /live` - Deve retornar `{"status":"ok"}`
   - `GET /ready` - Deve retornar `{"status":"ok"}`

### 🎉 Deploy Concluído!

Seu app estará rodando em produção com:
- ✅ Backend Node.js + Fastify
- ✅ PostgreSQL gerenciado
- ✅ Migrações Prisma aplicadas
- ✅ Health checks funcionando

## Próximos Passos Opcionais

### Domínio Customizado
1. Vá para **"Settings" > "Domains"**
2. Adicione seu domínio
3. Configure DNS conforme instruído

### Monitoramento
- **Logs:** Aba "Logs" no Railway
- **Métricas:** Aba "Metrics"
- **Alertas:** Configure em "Settings > Alerts"

### Escalabilidade
Railway escala automaticamente, mas você pode ajustar manualmente em **"Settings > Scaling"**

## Passo 4: Deploy

1. Railway fará o deploy automaticamente
2. Monitore os logs na aba "Deployments"
3. Assim que deployar, você verá a URL pública do seu app

## Passo 5: Verificar Deploy

1. Acesse a URL fornecida pelo Railway
2. Teste os endpoints básicos:
   - `GET /live` - Health check
   - `GET /ready` - Readiness check

## Configuração de Domínio (Opcional)

1. Vá para "Settings" > "Domains"
2. Adicione seu domínio customizado
3. Configure os registros DNS conforme instruído

## Troubleshooting

### ❌ Erro: "PrismaClientInitializationError" / "openssl1.1-compat"

**Sintomas:** App crasha com erro sobre Prisma não conseguir carregar bibliotecas

**Causa:** Alpine Linux tem problemas de compatibilidade com OpenSSL e Prisma

**Solução:** Dockerfile atualizado para usar `node:20-slim` (Debian) em vez de Alpine:

```dockerfile
FROM node:20-slim AS runner  # ← Mudou de node:20-alpine
```

**Por que Debian slim:**
- ✅ Melhor compatibilidade com Prisma
- ✅ OpenSSL 1.1.x nativo
- ✅ Não precisa de workarounds para bibliotecas
- ✅ Mais estável para aplicações Node.js

**Se ainda der erro:**
1. **Forçar rebuild no Railway:**
   - Vá para aba "Deployments"
   - Clique em "Deploy" ou "Redeploy"
2. **Ou aguarde:** Railway pode detectar mudanças automaticamente em alguns minutos
3. **Ou faça um commit dummy:** Adicione um comentário no código e commite para forçar trigger

### Erro de Build
- Verifique se o Dockerfile está correto
- Certifique-se de que todas as dependências estão no package.json

### Erro de Database Connection
- Verifique se a variável `DATABASE_URL` está configurada
- Certifique-se de que o PostgreSQL service está saudável

### Erro de Prisma
- Execute `npx prisma generate` localmente primeiro
- Verifique se as migrações estão na pasta `prisma/migrations`

## Monitoramento

Railway fornece:
- Logs em tempo real
- Métricas de uso
- Alertas de erro
- Usage dashboard

## Escalabilidade

Railway escala automaticamente baseado no uso. Para controle manual:

1. Vá para "Settings" > "Scaling"
2. Ajuste CPU, RAM e réplicas conforme necessário

## Backup

Railway faz backup automático do PostgreSQL. Para exportar dados:

```bash
# Conectar ao banco via Railway CLI
railway connect

# Fazer dump do banco
pg_dump $DATABASE_URL > backup.sql
```

## Custos

- **Free Tier**: ~$5/mês para projetos pequenos
- **Pago**: Baseado no uso real (CPU, RAM, bandwidth)
- PostgreSQL incluído no plano gratuito até certos limites