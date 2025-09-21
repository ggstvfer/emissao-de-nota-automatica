# Checklist Deploy Railway

## ✅ Conta Criada

## 🔄 Em Andamento

- [ ] **Passo 1:** Acessar [Railway Dashboard](https://railway.app/dashboard)
- [ ] **Passo 2:** Clicar "New Project" > "Deploy from GitHub repo"
- [ ] **Passo 3:** Autorizar GitHub e selecionar repositório `emissao-de-nota-automatica`
- [ ] **Passo 4:** Aguardar deploy inicial (vai falhar - isso é normal!)
- [ ] **Passo 5:** **CRÍTICO** - Adicionar PostgreSQL MANUALMENTE:
  - Clicar "+" no painel lateral
  - Selecionar "PostgreSQL"
  - Clicar "Add"
  - Aguardar criação
- [ ] **Passo 6:** **CRÍTICO** - Conectar DATABASE_URL:
  - Ir no serviço PostgreSQL > aba "Variables"
  - Copiar valor de DATABASE_URL
  - Ir no serviço da app > aba "Variables"
  - Adicionar DATABASE_URL com o valor copiado
- [ ] **Passo 7:** Adicionar outras variáveis:
  ```
  JWT_SECRET=ruWyk96giZUzm89WTO8NmfTcjCiPSj0qkfdvIVxcs9M=
  NODE_ENV=production
  METRICS_ENABLED=1
  ```
- [ ] **Passo 8:** Aguardar redeploy automático
- [ ] **Passo 9:** Testar endpoints `/live` e `/ready`

## 🎯 Resultado Esperado

- [ ] URL do Railway funcionando
- [ ] Health checks retornando `{"status":"ok"}`
- [ ] App acessível publicamente

## 🔧 Troubleshooting

Se algo der errado:
1. Verificar **"Deployments"** para logs de erro
2. Verificar **"Variables"** se todas foram adicionadas
3. Verificar **"Logs"** para erros de runtime

## 📞 Suporte

- Documentação Railway: https://docs.railway.app/
- Issues no GitHub se precisar de ajuda