# IEQ Cachoeira

Painel web de gestão e cuidado da comunidade, desenvolvido com React e Create React App.

## Executar localmente

Na raiz do repositório:

```powershell
npm install
Copy-Item .env.example .env
npm start
```

O arquivo `.env.example` define `VITE_API_URL`. O script de desenvolvimento/build adapta essa variável ao formato `REACT_APP_API_URL` exigido pelo Create React App. Também é possível definir `REACT_APP_API_URL` diretamente.

## API

O backend Express/Prisma fica na pasta `projectieqcachoeira`, em um repositório Git separado. Para executá-lo localmente:

```powershell
Set-Location .\projectieqcachoeira
npm install
npm start
```

A URL padrão da API é `https://backend-projectieqcachoeira.onrender.com`.

No Render, publique o frontend como Static Site a partir deste repositório, com `npm install && npm run build` como comando de build e `build` como diretório de publicação. O backend é publicado a partir do repositório `backend-projectieqcachoeira`, com `npm install && npm run build` e `npm start`.

## Verificação

```powershell
npm test -- --watchAll=false
npm run build
```
