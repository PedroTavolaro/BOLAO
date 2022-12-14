
<p align="center">
  <a>
    <h1 align='center' color='green'>NLW-COPA</h1>
  </a>
</p>

<h2 id="desc">
💟 Sobre o projeto
</h2>

<p align="justify">
A <b>NLW-COPA</b> é uma aplicação desenvolvida com intuito de conectar pessoas que desejam realizar bolões de jogos, podendo montar grupos, convidar pessoas e amigos para seus bolões ou entrar em bolões espécificos, através do código do bolão.
<br/>

</p>

<h2 id="prototipagem">
✈ Prototipagem
</h2>

<a href="https://www.figma.com/file/k3gfIJ4WKbiqHQOXrf9xds/Bol%C3%A3o-da-Copa">
<img title="WebNLWCopa" src="./githubAssets/Web.png">
</a>
<h6 align="center">Clique na imagem para ver o projeto no figma</h6>

<br>


## :hammer_and_wrench: Features 

-   [x] `Autenticação` com google;
-   [x] `Criar` bolão;
-   [x] `Listar` bolões;
-   [x] `Buscar` bolão por código;
-   [x] `Convidar` para bolão;
-   [x] `Contagem` de pessoas no bolão;
-   [x] `Contagem` de bolões criados;
-   [x] `Contagem` de palpites criados;
-   [x] `Contagem` de pessoas utilizando o app;
-   [x] `exibir avatar` das primeiras 4 pessoas do bolão ;
-   [x] `Criar` palpite sobre os jogos do bolão;
-   [x] `Validações de dados / funcionalidades`;
-   [x] `Busca e tratamento de dados das API's` ;
-   [x] `Rotas` entre as páginas;
-   [ ] `Ranking`;


<h1> Esse projeto foi desenvolvido com as seguintes tecnologias: </h1>

## Back-end

<p align="center">
<img width="720em" height="680em" alt="server" title="#server" src="./githubAssets/table.png" />
</p>

<h3 id="tec">
🛸 Tecnologias
</h3>

- [Node.js](https://nodejs.org/en/)
- [Fastify](https://www.fastify.io/docs/latest/Guides/Getting-Started/)
- [Prisma](https://www.prisma.io/)
- [TypeScript](https://www.typescriptlang.org/)
- [Zod](https://www.npmjs.com/package/zod)
- [ShorUniqueID](https://www.npmjs.com/package/short-unique-id)
- [Diagrama ERD](https://www.npmjs.com/package/prisma-erd-generator/)
- [Mermaid-js](https://mermaid-js.github.io/mermaid/#/)
- [Country Codes](https://countrycode.org/)
- [Sqlite](https://github.com/mapbox/node-sqlite3)

🎲 Rodando o Back End (servidor)

```bash 
# Clone este repositório
$ git clone https://github.com/PedroTavolaro/NLW-COPA.git
# Acesse a pasta do projeto no terminal/cmd
$ cd nlwcopa
# Vá para a pasta server
$ cd server
# Instale as dependências
$ npm install
# Execute a aplicação em modo de desenvolvimento
$ npm run dev
# O servidor inciará na porta:3333 - acesse <http://localhost:3333> 
```
-------------------------------------------------------------------
## Frontend

<p align="center">
<img alt="web" title="#web" src="./githubAssets/Web.png" />
</p>

<h3 id="tec">
🛸 Tecnologias
</h3>

- [React](https://pt-br.reactjs.org/)
- [NextJS](https://nextjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwindcss](https://tailwindcss.com/)
- [Axios](https://github.com/axios/axios)


🔭 Rodando o Frontend (web)
```bash 

# Acesse a pasta do projeto no terminal/cmd
$ cd NLW-COPA
# Vá para a pasta web
$ cd web
# Instale as dependências
$ npm install
# Execute a aplicação em modo de desenvolvimento
$ npm run dev
# O servidor inciará na porta:3000 - acesse <http://localhost:3000> 
```
## Mobile


<p align="center">
<img alt="web" title="#web" src="./githubAssets/mobile/aplicacao-trilha-ignite.png" />
</p>

<h3 id="tec">
🛸 Tecnologias
</h3>

- [Expo](https://expo.io/)
- [React Native](https://reactnative.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [React Native Svg-Transformer](https://github.com/kristerkari/react-native-svg-transformer)
- [Expo Auth Session](https://docs.expo.dev/versions/latest/sdk/auth-session/)
- [Expo Web Browser](https://docs.expo.dev/versions/v46.0.0/sdk/webbrowser/)
- [API GOOGLE](https://console.cloud.google.com)
- [PhosphorIcons](https://phosphoricons.com/)
- [Axios](https://www.npmjs.com/package/axios)
- [Country-List](https://www.npmjs.com/package/country-list)
- [DayJS](https://www.npmjs.com/package/dayjs)
- [dotENV](https://www.npmjs.com/package/dotenv)

📱 Rodando o Mobile (mobile)

```bash 
# Acesse a pasta do projeto no terminal/cmd
$ cd NLW-COPA
# Vá para a pasta mobile
$ cd mobile
# Instale as dependências
$ npm install
```
## Criar / Alocar variável ambiente

#### - Criar projeto no google cloud(console)
#### - Dcumentação (https://docs.expo.dev/guides/authentication/#google)
#### - Entrar no menu de navegação - APIs e serviços - Tela de permissão OAuth  (\/*user*\/)
#### - Type Externo, add escopo (não confidenciais) - auth/userInfo (email, profile), publicar
#### - No menu de navegação - Crendenciais - Criar credenciais (ID do cliente OAuth)
#### - (Aplicatiov da web)
#### - JavaScript URI = https://auth.expo.io
> **⚠ Atenção !** <br> Importante, é necessário está logado com uma conta expo para 2ºopção (para logar ```$ npx expo login```) (para visualizar usuário ```$ npx expo whoami```.
#### - Redirecionamento URI = 

##### opção 1º => ( https://auth.expo.io/@your-username/your-project-slug ) - (your-name = nome da conta expo) + (slug = nome definido na criação do projeto) 

##### opção 2º => no arquivo AuthContext.tsx digite dentro da função AuthContextProvider ``` console.log(AuthSession.makeRedirectUri({ useProxy: true }));```  copie a mensagem / link no terminal e adicione na URL de redirecionamento. <br /> Criar 

#### - Copiar ID do cliente e colocar na variável ambiente no arquivo NLW-COPA/mobile/.env

```bash 
# Execute a aplicação em modo de desenvolvimento
$ npx expo start
# O servidor inciará na porta:3000 - acesse <exp://10.50.3.50:19000> 
```


## 🤔 Como contribuir

- Faça um fork desse repositório;
- Cria uma branch com a sua feature: `git checkout -b minha-feature`;
- Faça commit das suas alterações: `git commit -m 'feat: Minha nova feature'`;
- Faça push para a sua branch: `git push origin minha-feature`.

Depois que o merge da sua pull request for feito, você pode deletar a sua branch.

<h2 id="lic">
📃 Licença
</h2>

Este projeto esta sobe a licença [MIT](./LICENSE)

### Autor
---

<a href="https://pedrotavolaro.com">
 <img style="border-radius: 50%;" src="https://github.com/PedroTavolaro.png"  width="100px;" alt=""/>
 <br />
 <sub><b>PedroTavolaro</b></sub></a> <a href="https://www.pedrotavolaro.ccom" title="PedroTavolaro">🚀</a>

Feito com ❤️ por Pedro Tavolaro 👋🏽 Entre em contato!

[![Twitter Badge](https://img.shields.io/badge/-@pedrotavolaro-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/pedrotavolaro)](https://twitter.com/pedrotavolaro) [![Linkedin Badge](https://img.shields.io/badge/-PedroTavolaro-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/pedrotavolaro/)](https://www.linkedin.com/in/pedrotavolaro/) 
[![Hotmail Badge](https://img.shields.io/badge/-email-0078D4?style=flat-square&logo=microsoft-outlook&logoColor=white&link=mailto:phtc-pedro@hotmail.com)](mailto:phtc-pedro@hotmail.com)
