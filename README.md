# casernaHub

Monorepo com o front-end e o back-end do casernaHub.

| Pasta    | Stack                        | Porta |
| -------- | ---------------------------- | ----- |
| `front/` | React + TypeScript + Vite    | 5173  |
| `back/`  | Node + Express + TypeScript  | 3000  |

## Requisitos

- Node.js 20.19+ (recomendado: a versão atual via nvm)

## Rodando localmente

Back-end:

```bash
cd back
cp .env.example .env
npm install
npm run dev
```

Front-end (em outro terminal):

```bash
cd front
npm install
npm run dev
```

O front chama a API em `/api/...`. Em desenvolvimento, o Vite repassa essas
requisições para `http://localhost:3000` (veja `front/vite.config.ts`).
