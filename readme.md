## Primeiro Projeto

### Criando a estrutura

Execute o comando

```
react-native init NomeProjeto
```

Configure o Eslint e o Prettier

```
yarn add eslint -D
yarn eslint --init
rm package-lock.json
yarn
yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D
```

Crie os arquivos

- [.editorconfig](/.editorconfig)

- [.prettierrc](/.prettierrc)

Altere o arquivo **[.eslintrc.js](/.eslintrc.js)**

#### Captura de logs

Iremos utiliar o [Reactotron](https://github.com/infinitered/reactotron).

Execute o comando

```
yarn add reactotron-react-native
```

Crie o arquivo **src/index.js** e copie todo conteudo do App.js para ele; Exclua o arquivo App.js e altere a linha _import App from './App'_ para _import App from './src'_.

Crie o arquivo [src/config/ReactotronConfig.js](/src/config/ReactotronConfig.js)

> Caso esteja usando Android (usb ou emulador) execute o comando adb reverse tcp:9090 tcp:9090

## Navegação

Execute o comado

```
yarn add react-native-reanimated react-native-gesture-handler react-native-screens

cd ios
pod install
cd ..
```

> Para Android tem mais um passo, verifique em https://kmagiera.github.io/react-native-gesture-handler/docs/getting-started.html

Agora crie os arquivos:

- [src/routes.js](/src/routes.js)
- [src/pages/Main/index.js](/src/pages/Main/index.js)

Execute o comando

```
yarn add styled-components
```

Crie o arquivo [src/pages/Main/styles.js](/src/pages/Main/styles.js)

> Para usar icones

```
yarn add react-native-vector-icons
react-native link react-native-vector-icons
```

### Outras dicas

> Para consumir api

```
yarn add axios
```

> Storage

```
yarn add @react-native-community/async-storage
react-native link @react-native-community/async-storage
```

> PropTypes

```
yarn add prop-types
```

> WebView

```
yarn add react-native-webview
react-native link react-native-webview
```
