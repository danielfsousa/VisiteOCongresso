#  Visite O Congresso
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)

O aplicativo foi desenvolvido durante o [Desafio VisitApp](http://www1.congressonacional.leg.br/desafio/), com o objetivo de guiar e oferecer a mesma experiência aos visitantes presenciais e virtuais do Congresso Nacional.

## Configurando

1. Instale o React Native e suas depencências: [Siga o tutorial "Building Projects with Native Code"](https://facebook.github.io/react-native/docs/getting-started)
2. [Instale o cli do Ignite](https://github.com/infinitered/ignite#arrow_down-install)

## Iniciando

1. Faça o download do repositório: `git clone https://github.com/danielfsousa/visite-o-congresso`
2. Instale as dependências: `npm i` ou `yarn`
3. Inicie a Build do SO desejado
  * iOS
    * `npm run ios`
  * Android
    * `npm run android`

## Boilerplate

Utilizamos o [Ignite](https://infinite.red/ignite) para fazer o bootstrap do projeto. Com o Ignite é possível criar componentes, telas, listas, reducers e sagas utilizando o comando `ignite generate` e adicionar plugins como internacionalização, redux-persist, entre outros utilizando o comando `ignite add`. Tudo o que o ignite pode fazer por você está bem explicado na sua [documentação](https://github.com/infinitered/ignite/blob/master/docs/README.md).

## Bibliotecas

Seguem as documentações de algumas bibliotecas importantes que utilizamos no projeto:

* [Lodash](https://lodash.com/)
* [Ramda](https://ramdajs.com/)
* [React Navigation](https://reactnavigation.org/)
* [Redux](https://redux.js.org/)
* [Redux Saga](https://github.com/redux-saga/redux-saga)
* [Redux Persist](https://github.com/rt2zz/redux-persist)
* [Redux Sauce](https://github.com/infinitered/reduxsauce)
* [Apisauce](https://github.com/infinitered/apisauce)
* [React Native Elements](https://github.com/react-native-training/react-native-elements)
* [React Native Vector Icons](https://github.com/oblador/react-native-vector-icons)
* [React Native i18n](https://github.com/AlexanderZaytsev/react-native-i18n)
* [React Native Animatable](https://github.com/oblador/react-native-animatable)

## Storybook

Utilize o comando `npm run storybook` para visualizar os componentes do projeto individualmente

## Linter

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)
Esse projeto utiliza o padrão Standard

**Executar o linter antes dos commits**

O linter é executado antes de cada commit, sem precisar configurar nada. Utilizamos o [husky](https://github.com/typicode/husky) para isso.

**Ignorar o linter**

Se você precisar fazer um commit rápido em uma branch separada (que você irá voltar e limpar o código em uma outra hora) então você poderá ignorar o linter adicionando a flag `--no-verify` ao comando `git commit`.

**Entendendo os erros do linter**

As regras do linter são do JS Standard e React-Standard.  [Erros comuns do javascript podem ser encontrados aqui](http://eslint.org/docs/rules/), enquanto [erros relacionados ao React podem ser encontrados aqui](https://github.com/yannickcr/eslint-plugin-react).

## Variáveis de Ambiente

Esse projeto utiliza o [react-native-config](https://github.com/luggit/react-native-config) para expor as variáveis de ambiente de confinguração do projeto. Você pode guardar chaves de API e outras informações sensíveis em um arquivo `.env`:

```
API_URL=https://myapi.com
GOOGLE_MAPS_API_KEY=abcdefgh
```

E acessá-las diretamente no seu código:

```javascript
import Secrets from 'react-native-config'

Secrets.API_URL  // 'https://myapi.com'
Secrets.GOOGLE_MAPS_API_KEY  // 'abcdefgh'
```

O arquivo `.env` é ignorado pelo git para manter as informações sensíveis fora do seu repositório.

### Configurando as variáveis de ambiente:
1. Copie o .env.example para .env
2. Adicione as suas variáveis
3. Siga as instruções: [https://github.com/luggit/react-native-config#setup](https://github.com/luggit/react-native-config#setup)
4. Pronto!

## Debugging

**Código do React Native:**
* Para debugar com o Chrome Developer Tools [siga as instruções no site oficial](https://facebook.github.io/react-native/docs/debugging)
* Se você usa o Visual Stuio Code, instale o plugin [React Native Tools](https://marketplace.visualstudio.com/items?itemName=vsmobile.vscode-react-native)

**Código Nativo:**
* Se for necessário debugar módulos nativos, você pode abrir o aplicativo pelo Android Studio ou Xcode e obter todas as vantagens para depuração (breakpoints, etc.) como se estivesse desenvolvendo um aplicativo nativo.

Utilizamos também o [React Developer Tools](https://facebook.github.io/react-native/docs/debugging#react-developer-tools) para debugar a hierarquia dos componentes do React e o [Reactotron](https://github.com/infinitered/reactotron) para inspecionar o estado da aplicação e as requisições e respostas das APIs

## Tutoriais

* [Documentação oficial do React Native](https://facebook.github.io/react-native/docs/tutorial)
* [React Native Express](http://www.reactnativeexpress.com/)
* [React Native Training](https://unbug.gitbooks.io/react-native-training/content/)
* [React Native Katas](https://github.com/jondot/ReactNativeKatas)
* [Building the F8 App](https://makeitopen.com/)
* [Flexbox Froggy](https://flexboxfroggy.com/)

## Vídeos

* [Construindo layouts no React Native](https://www.youtube.com/watch?v=Q7gT462aBU0)
* [Building a React Native App in Under 15 Minutes with Ignite](https://www.youtube.com/watch?v=lv00UOXxy0g)
* [UI: Flexbox, Animações e Clones de Apps Famosos](https://www.youtube.com/channel/UCiNWv52iO_OAdZ12kslG4Cg/playlists)
* [Ben Awad: Fullstack React and React Native Videos](https://www.youtube.com/user/99baddawg/playlists)
* [React Native Training](https://www.youtube.com/channel/UC8ivCOllOAo7MfPT9k3Hs-Q/videos)
* [Tyler Mcginnis: React Native Course](https://tylermcginnis.com/courses/react-native-udacity/)
* [Egghead.io](https://egghead.io/browse/frameworks/react-native)
* [Minicurso React Native](https://rocketseat.com.br/minicurso-react-native-para-iniciantes)
* [codedamn: React Native Calculator](https://www.youtube.com/watch?v=EMoXvr0Q9LE&list=PLYxzS__5yYQlHANFLwcsSzt3elIbYTG1h)

## Referências

* [Official Chain React Conf App](https://github.com/infinitered/ChainReactApp)
* [Official Facebook F8 App](https://github.com/fbsamples/f8app)
* [Unofficial Dribbble client](https://github.com/catalinmiron/react-native-dribbble-app)
* [Unofficial Gitter.im client](https://github.com/apiko-dev/GitterMobile)
* [22 Amazing open source React projects](https://medium.mybridge.co/22-amazing-open-source-react-projects-cb8230ec719f)
* [React Native Apps](https://github.com/ReactNativeNews/React-Native-Apps)

## Outros

* [Awesome React Native](https://github.com/jondot/awesome-react-native)
* [Awesome React Native Education](https://github.com/hsavit1/Awesome-React-Native-Education)
* [JSCoach: Procure componentes, boilerplates e generators](https://js.coach/)
* [React Native Snippets para o VSCode](https://marketplace.visualstudio.com/items?itemName=jundat95.react-native-snippet)


