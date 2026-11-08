# Discord Bot

Bot de Discord para um servidor de estudos de programação, feito com [discord.js](https://discord.js.org) v14 e slash commands.

## Arquivos

- `index.js`: conecta o bot e carrega os comandos da pasta `commands/`.
- `deploy-commands.js`: registra os slash commands no servidor (guild).
- `.env.example`: modelo das variáveis `TOKEN`, `CLIENT_ID` e `GUILD_ID`.

## Como rodar

```bash
npm install
cp .env.example .env
node deploy-commands.js
node index.js
```

Antes, preencha o `.env` (ele fica fora do git) com o token do bot e os IDs da aplicação e do servidor, e crie a pasta `commands/` com um arquivo `.js` por comando, cada um exportando `data` e `execute`. Essa pasta não está no repositório.
