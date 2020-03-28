# React Native
>### Saindo do Level 1


#### Criando o Projeto

Se você vai criar um projeto, aconselho ler esse tópico:
 - https://reactnative.dev/docs/environment-setup 

Eu particularmente, para uma experiencia REAL, aconselho o caminho "React Native CLI Quickstart"

em Resumo:

* para projetos sem firebase: 
```
npx @react-native-community/cli init AwesomeProject
```

* para projetos sem firebase e com typescript:  
```
npx @react-native-community/cli init AwesomeTSProject --template=react-native-template-typescript
```

* para projetos com firebase:
(https://invertase.io/oss/react-native-firebase/quick-start/new-project)

```
npx @react-native-community/cli init --template=@react-native-firebase/template AwesomeFirebaseProject
```


> Na pasta CriandoProjeto, tem um exemplo criado com cada um deles :D

---
### Ferramentas de Debug

Pra debug de rede eu uso o reactotron:

https://github.com/infinitered/reactotron/blob/master/docs/quick-start-react-native.md


```js
import Reactotron from 'reactotron-react-native'
import AsyncStorage from '@react-native-community/async-storage';

Reactotron
  .setAsyncStorageHandler(AsyncStorage) 
  .configure()  
  .useReactNative()  
  .connect()  
  
```

