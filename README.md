# electron-autoupdate
 Código para atualizar automaticamente um app feito com Electron
 
Baseado em: https://github.com/iffy/electron-updater-example

Necessário criar um token em: https://github.com/settings/tokens

Altere o package.json para informar seu token e seu repositório

Caso seu repositório seja privado é necessário criar uma variável de ambiente chamada **GH_TOKEN**

```
{
  "provider": "github",
  "repo": "<name of your repository>",
  "owner": "<your name>",
  "token": "<personal access token>",
  "private": true,
  "releaseType": "release",
  "publishAutoUpdate": true
}
```

Altere o version dentro de **package.json** e rode **npm run publish** para publicar no github, ai só fechar e abrir o programa para baixar a instalação.
