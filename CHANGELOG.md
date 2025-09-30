# Changelog

## [0.1.2](https://github.com/ggstvfer/emissao-de-nota-automatica/compare/v0.1.1...v0.1.2) (2025-09-30)


### Features

* add AuthDebug component for authentication debugging and temporary route ([ab283f8](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/ab283f83ff0939e891f39811120eb0ce93efb74c))
* add authentication service for handling login, logout, and user session management ([2adefeb](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2adefebd1f8e312bfe9a7be6f34ef1eafaa14936))
* add automatic timestamp handling for createdAt and updatedAt in suppliers and clients; update SQL script for UUID and timestamp defaults ([e04b57d](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/e04b57d0eee6f873bb8a513fb0a2b62bfee0ab5e))
* Add comprehensive documentation for digital certificate setup and system corrections ([a19af3d](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/a19af3db80563fc6bb027a896f01cda705cbe678))
* add detailed logging in ServiceTypesService for create operation; improve error handling for duplicate entries ([68b1a47](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/68b1a47d9b1df4a8a873b2b37353146d5caf4ed7))
* add FormulaGroupDetailPage and FormulaGroupsPage components for managing formula groups and formulas ([4f821f4](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/4f821f46397c87c9d39bdcb157564aa4eb65300a))
* add ImportClients component for bulk client import functionality with JSON and CSV support ([38d0eb5](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/38d0eb5f3b7b66ae588f191bbdf0c899c1552345))
* add ImportSuppliers page for bulk supplier import functionality ([c00e2f7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/c00e2f712b1970fb231f657435a939fc2236cb25))
* add JWT authentication and debugging endpoints for NFSe API ([9ee050b](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/9ee050b2e46ded9cbd195e303bacc729b83fd41c))
* Add setup scripts and configuration for PFX certificate handling in NFSe system ([ee06c3f](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/ee06c3f2d2fb75d2921cd38f364d0c2755b5eca9))
* add Supabase configuration to environment variables ([4d509c9](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/4d509c9267eb4a71feaec8c949b396895c55b1b3))
* add Suppliers management page with search, delete, and pagination features ([2adefeb](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2adefebd1f8e312bfe9a7be6f34ef1eafaa14936))
* add SystemConfig and SystemStatus pages for system configuration and monitoring ([a4f133a](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/a4f133af45688bf142bf57ad2b97e57c70350d31))
* adiciona importação automática de clientes do Uphold com Puppeteer ([7200aa1](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7200aa1c9d1e3f7aa867df38abc5b7abb66d2909))
* adiciona migrações e arquivos de configuração para ServiceTypes ([7545d57](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7545d577b2ef60a9ea7fe640334eb4332d0e5f69))
* create UpholdConfig page for managing Uphold configurations ([c00e2f7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/c00e2f712b1970fb231f657435a939fc2236cb25))
* create Webhooks overview page to manage webhook configurations ([2adefeb](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2adefebd1f8e312bfe9a7be6f34ef1eafaa14936))
* DX Windows e smoke autônomo (AutoStartDev), melhorias NFSe e client ([03d7bc8](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/03d7bc8ba0c89ff473862a0f914abee7f5d5bdc5))
* enable webhook and retry routes; refactor account, client, and supplier routes to simplify schema usage ([8cb03cb](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/8cb03cb9fb56eee24dc3f2b0e8af75f84edc1e72))
* enhance AuthProvider to handle user profile loading with fallback creation; add SQL script for user_profiles table management ([63570a9](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/63570a906490b7895a150dc1845672140ddbc762))
* enhance AuthProvider to prevent duplicate user profile loading; add processedUserId state management ([68b1a47](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/68b1a47d9b1df4a8a873b2b37353146d5caf4ed7))
* enhance create method in ServiceTypesService with improved user authentication handling and error logging ([f3bc1ba](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/f3bc1ba0ac0e19139e37bca47c359ad9352c4bfd))
* enhance loadUserProfile with detailed logging and error handling; improve loading state management ([bddb3ed](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/bddb3ed4f21ab97c683239e82f326ed79fc4e183))
* enhance LoginDebug and AuthContext for improved logging and loading management; add safety timeout for loading state ([92b2368](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/92b23687af7bb91d9822c8efc0ef364ae92042f6))
* enhance migration script for simplified formulas with safety checks and logging; add temporary LoginDebug component for authentication debugging ([29e630e](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/29e630eeb05f6440d68fc48faafcb04d7b45fbdd))
* enhance Vercel and Supabase integration with serverless functions and environment variable setup ([2f1f44c](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2f1f44c4fd51ecfc22eafba08bb38be8995ffcdb))
* export necessary components from accounts and jobs modules ([5384050](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/53840504b49c0a5b595d1cb5e5f3da3ed223fd6e))
* força deploy com comentário de atualização dos Tipos de Serviço ([02c96cd](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/02c96cdc5729046f9d233a22775ed67269f3c7ef))
* implement AuthContext and AuthProvider with user profile management and session handling ([7c76969](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7c76969f9f44de9ac46dc57a6ca89eb57a978587))
* implement AuthContext with user profile loading and session management; add error handling and fallback profile creation ([e8ccf04](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/e8ccf040d8507ed0806de688f777a540dd5de6b8))
* implement client management module with CRUD operations ([5384050](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/53840504b49c0a5b595d1cb5e5f3da3ed223fd6e))
* Implement complete CRUD functionality for clients and suppliers with data persistence and improved response structure ([194f6f8](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/194f6f8500aa1e6668470788b029e7e9d302886a))
* implement comprehensive dependency management practices ([d763f05](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/d763f053ad5bc04033b059c6c36c0bc2ae2e6c76))
* Implement error boundary in App component and improve client/supplier handling ([3292846](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/329284632a26859383f116979da8ae88e6c3555c))
* implement retry job management module ([5384050](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/53840504b49c0a5b595d1cb5e5f3da3ed223fd6e))
* implement supplier management module with CRUD operations ([5384050](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/53840504b49c0a5b595d1cb5e5f3da3ed223fd6e))
* implement Webhook form for creating and editing webhooks with event selection ([2adefeb](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2adefebd1f8e312bfe9a7be6f34ef1eafaa14936))
* implement webhook management module ([5384050](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/53840504b49c0a5b595d1cb5e5f3da3ed223fd6e))
* implement webhooks service for CRUD operations on webhooks ([2adefeb](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2adefebd1f8e312bfe9a7be6f34ef1eafaa14936))
* implementa CRUD completo para tipos de serviço ([46cc2bf](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/46cc2bf43f1d672442aa704d2594dad29d4f3b19))
* Implementa melhorias na interface de emissão NFSe ([7c54f02](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7c54f0255845f8dba6d274d56f2ed5970beaa32b))
* implementa sistema de administração global ([724b6a6](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/724b6a6da600c8da7a2842beb8a28e27a56beb52))
* implementa Supabase Auth com login/registro email/senha ([64c0097](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/64c00977917be130e373566e8c690e73728260e1))
* Implementar migração e CRUD para fórmulas simplificadas ([07e47fc](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/07e47fcb0cec57d9955cd7110f23d33641b17b73))
* improve logging in ServiceTypeForm during submission; enhance error handling messages ([68b1a47](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/68b1a47d9b1df4a8a873b2b37353146d5caf4ed7))
* initialize UI project with Vite, React, and TypeScript ([2a606d7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/2a606d7538b31dbe3b63dd463fdcde1d1bae003b))
* migra frontend para usar Supabase diretamente ([1e9578a](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/1e9578a958e5ce84290f1dbe76674d07a2a5ecae))
* Migração completa para Supabase ([3778704](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/3778704c2ec584036d4db96bc5531c6a33b058c6))
* migrate API to ES modules and enhance certificate handling with base64 support ([a64c342](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/a64c342868c85661526772ab67cbc5232e4b019f))
* migrate to Supabase + Vercel deployment ([e4f7e77](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/e4f7e77c9ff12c17d5c6f04dec6eb3d70c077dea))
* otimiza build com chunks e corrige configuração Vercel ([303b338](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/303b338c989c676ac489e15cb5a540c84ce7f294))
* refactor import handling in ImportServiceTypes to use ServiceTypesService for batch import with enhanced logging and error handling ([9e7118d](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/9e7118d4bfcbd49051688f285faa4a7b520c98c9))
* refactor ServiceTypeForm to use ServiceTypesService; update loading and error handling; improve form data structure ([f339ead](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/f339eadf0431b449e27398b09f1e4321a1ee594a))
* refactor user profile loading to use direct supabase queries; add error handling and temporary profile creation ([1bba469](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/1bba469accec7b77fa1c95ba1056054bffab6eaa))
* remove deprecated API endpoints and add certificate handling for serverless environment ([6e126bf](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/6e126bf403e68e5fa397ce00bcc5e49f59870801))
* remove directUrl from datasource configuration in Prisma schema ([d656169](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/d656169a3bdcc34f438303a2ee2dc1f29c8ed2a8))
* update client data in CSV and JSON files for improved accuracy and consistency ([5b21367](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/5b213671bebd8e9ffef86918d1d324ad6a5d7de3))
* update dependencies and enhance logging in CRUD operations for suppliers and clients; implement automatic UUID generation in database ([75b7c83](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/75b7c83fdfe752b3a2f1ff7abb6619ffaf0c5c53))
* update table names in services to match Prisma schema; correct TypeScript types and field names ([652ba28](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/652ba281e3e08e11bca6c5fa0058838423a59677))


### Bug Fixes

* add database reset step in CI to ensure clean state ([a49f9c4](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/a49f9c4464217d336e91751aa32d89c117b0faf1))
* add id-token permission and explicit token for release-please ([d168be9](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/d168be99563524fe5ae29d2316b116439a10e2e5))
* add initial database migration to fix CI deployment ([6fb3b24](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/6fb3b2417f5a41a0b4e82c2e65fa65681c341b34))
* add missing ui/package-lock.json to repository ([d05b3a3](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/d05b3a3c7aa1a49ae5433ed08436d4b9e74791cf))
* add OpenSSL 1.1 compatibility for Prisma in Alpine Docker ([c461203](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/c46120393ac76a435c3622aa5b7cf86988f131ab))
* aplica configurações Vercel para corrigir deploy ([7d14cf7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7d14cf7c4ef6b713a1b609e023c5aba365d9dba2))
* atualiza schema e API para deploy ([d0fedfc](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/d0fedfcdf7cd1042ad0b3d930469693a2495d702))
* change Docker base image from Alpine to Debian slim for Prisma compatibility ([520b93e](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/520b93e0d8fc4462366e8e29573d2d9460d4c617))
* configure Prisma to use library engine for better container compatibility ([77f82a0](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/77f82a06b00566b2af05c0a6a398caae5124c9f4))
* correct ESLint errors in cancel-reason test ([cf4da01](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/cf4da01583eb009e7a04fe37f1adb12678ff8644))
* correct migration order and make idempotent ([5051bce](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/5051bce91dd9918dd72f134066369e66685ecb91))
* corrige deploy e interface ([665b81b](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/665b81bf927028875bbd32588c27ea3462e92bc5))
* corrige ícone do menu Tipos de Serviço ([f6e72b0](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/f6e72b0b0b091abc946c90081dd1abc05b6c551e))
* Corrigir configuração de build do Vercel ([ac048da](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/ac048da664bd229e7f00325c5e1f66a194e95be6))
* Corrigir persistência de dados no Vercel ([f167e17](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/f167e172cb257e9a93a53ea6859e04b600e26dfc))
* install UI dependencies in CI workflow ([1342692](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/13426929bbd8ead039f6f96fa1af4b02a06741a1))
* move permissions to workflow level for release-please ([edd41ca](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/edd41ca3d086831684f0571e1168e4e59d8d05ec))
* move vite e @vitejs/plugin-react para dependencies para Vercel ([0ee073e](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/0ee073ee1c1a030381bc7d85302be906ab687be7))
* reinstall dependencies and restore build script for Vercel ([563bf45](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/563bf45038a5e8f20d76f874f35cab1c8c9c1e65))
* remove package-lock.json from .gitignore to allow tracking lockfiles ([3418b09](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/3418b09f4c65a8764c8882f9b1e0a717c62e6e94))
* remove TypeScript do build e simplifica vercel.json para resolver errors ([5dd1446](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/5dd1446e280d164a341e249478a01687fe0a24cf))
* resolve TypeScript build errors for Vercel deployment ([0268753](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/02687539f9f235a0393ac7fd521e75e66c112697))
* simplifica tipos de serviço conforme Uphold ([1720afd](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/1720afd7cf93e4bf96c7cef6090c447dc2e24093))
* simplifica vercel.json - remove ignoreCommand e usa npm ci ([637687f](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/637687f2deec13ceb92dbc94756213029484fa79))
* simplify build script to bypass TypeScript errors in Vercel ([cc96077](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/cc9607705f37c29e3a903294b5bd34d91a1f505b))
* **smoke:** ensure Param is first and set working directory for auto-start; feat(nfse): include verificationCode in GET /nfse/:id response ([0ead4a7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/0ead4a7d19f96f26e18b53ba59727994807e7aac))
* update @types/react-dom version for compatibility ([a4f133a](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/a4f133af45688bf142bf57ad2b97e57c70350d31))
* update build and install commands in package.json and vercel.json for consistency ([72ac34e](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/72ac34ee89a717fc1074b45e0e54a23d59fcdb31))
* update filter logic in NfseList component for better readability ([7f8fec4](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7f8fec43914ee713739a6bb772d09c4d63757c4c))
* update release-please action to non-deprecated version ([6e82ba7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/6e82ba72bc918b2b66ab6c2ddbb52f84a65bc9b7))
* update Vercel configuration for proper deployment ([24171f6](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/24171f6f919923833e65f1bfba2b16e720927e6d))


### Chores

* **main:** release v0.1.2 with idempotency payloadHash, agent stub for dev, nfseNumber filter ([0a481a8](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/0a481a84e7833eae7cd5bfaad96c9fbacd3d1cd1))
* **release:** v0.1.1 version bump and changelog ([353c5ee](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/353c5ee2060c8e9f7ad655896414b4c4b0270f68))
* trigger release-please v0.1.2 ([4f65dcd](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/4f65dcd765e30b40bdfa1aad978f800ba29e06f1))
* update deployment configurations for Supabase and Vercel integration ([c7c15b3](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/c7c15b3ba9b355e9ea5f653f234f228f7972a8fd))
* upgrade xml-crypto to 6.1.2 (fix critical advisories) ([4007efd](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/4007efd39547e881ee7db17813b6b490a647e616))


### Documentation

* add comprehensive deploy documentation ([9832203](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/9832203534420eb5e7278035b10f8545577f11bb))
* add release-please setup instructions ([c656c51](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/c656c518b82012bb20263b4a642840b5e9404c9e))
* add troubleshooting for DATABASE_URL error in Railway ([681cb23](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/681cb232302d40f9202500b07a9af26378a3d0c0))
* add troubleshooting for Prisma engine resolution error ([e5a6cd5](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/e5a6cd560099c1db62c84a8413d753ac3868fd2a))
* badge do workflow de smoke no README e resumo no Job Summary; .env.example atualizado (IN_MEMORY_DB e exemplos do agente) ([5f400a7](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/5f400a709233cd4ee1e62ed37ced46ff2e5a999e))
* clarify Railway Docker + PostgreSQL setup ([7569e53](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7569e53c9b6a59b8963fd0d2c06278fa6258e817))
* improve Railway troubleshooting for cached Dockerfile issue ([cd0fefc](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/cd0fefcb80d11c65a0b1e9b7795035c496de0c2a))
* update Railway deploy guide with step-by-step checklist ([451e93f](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/451e93fb16b25131bbc2ee13d1bf496f21422ed6))


### Code Refactoring

* **abrassf-generator:** build root open tag with array join to avoid manual space logic ([482b617](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/482b617ab2ac3638e28a91d6d75011c140142a76))
* clean up imports and enhance security in formulas service ([cd156b8](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/cd156b87897863df0dfc764fb5068e4da62543b2))
* remove unused schemas and improve code clarity in account, client, and supplier routes ([7f8fec4](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7f8fec43914ee713739a6bb772d09c4d63757c4c))
* reorder imports for better organization and consistency across files ([aa22a69](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/aa22a69f78329d0c38dc5b49f9931abec28de034))


### Tests

* **abrassf-generator:** add regression tests to avoid stray space before root &gt; ([6a51e24](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/6a51e24683ff4ebed53981f89b3409c023db3da3))
* enhance mocks for axios and prisma in various test files ([7f8fec4](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/7f8fec43914ee713739a6bb772d09c4d63757c4c))


### Continuous Integration

* **docs:** workflow smoke com artefato nomeado e summary rico; README com seção do Smoke CI ([ad2ca46](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/ad2ca46c5d42fcc0d8b15900759aca03284263d8))
* **release-please:** automate versioning/changelog/tag via PRs on main ([fb668d2](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/fb668d2f516511714c726b6aaba8fae635141889))
* **release:** create GitHub Release automatically on v*.*.* tags ([adf4f40](https://github.com/ggstvfer/emissao-de-nota-automatica/commit/adf4f4093795deb399b49527735b798677bf2f80))

## v0.1.1 - 2025-09-16

Hardening de segurança e pequenas melhorias.

- Segurança: upgrade `xml-crypto` para `6.1.2` (corrige advisories críticos de assinatura XML).
- Gerador ABRASF: refactor na montagem da tag raiz usando join seguro para evitar espaço extra e simplificar leitura.
- Testes: adicionados testes de regressão garantindo que não haja espaço antes de `>` no root (`<Rps>` e `<nfse:Rps>`).

## v0.1.0 - 2025-09-16

Primeiro corte do MVP com gerador ABRASF robusto, API, testes e documentação.

- Gerador ABRASF (`buildRpsXml`):
  - Atributos do root seguros: proteção a `xmlns`, `xmlns:<prefix>`, `xmlns:xsi`, `xsi:schemaLocation`.
  - Ordenação determinística por padrão e opção `preserveExtraOrder`.
  - Suporte a `Record`, `Array<[k,v]>` e `Map` em `extraRootAttributes`.
  - Deduplicação last-wins; nomes validados (attr e NCName); `nsPrefix`/`rootName` com fallback seguro.
  - Escape de `namespaceUri` e `schemaLocation`.
  - Fix: evitar espaço extra no root quando sem atributos.
  - Helper `toExtraPairs` para normalizar/ajustar ordem com `Map`.
- Tipagem e DX:
  - Overloads de `buildRpsXml` por fonte de extras; export de `BuildOptions`, `ExtraAttrPair`, `ExtraAttrValue` via barrel `src/core/xml`.
- Assinatura/Verificação:
  - `xml-crypto` v5; suporte a SHA-256 (SHA-1 opcional); `verifyXmlSignature` validando assinatura e X509.
- Observabilidade/Serviço:
  - Métricas Prometheus; endpoints de saúde/versão/live/ready; logs silenciosos em teste.
- Testes e Docs:
  - Suíte de testes abrangente (normalização, emissão, assinatura/verificação, métricas, DX do gerador).
  - README com opções avançadas, exemplos e recipes.
