## CRIANDO O PRIMEIRO APP EM REACT NATIVE

- sudo npx react-native init app
- npm install styled-components
- npm install @react-navigation/native

https://reactnavigation.org/docs/getting-started

- expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view

- npm install @react-navigation/stack
- npm install @react-navigation/bottom-tabs

> para usar o token jwt, precisamos da dependencia abaixo
- npm install @react-native-community/async-storage

> pegar localização do usuário
- npm install @react-native-community/geolocation

> permissao extra para pegar a localização do usuário (versões mais novas do android)
- npm install react-native-permissions

- npm install react-native-swiper

> ajudar a trabalhar com svg por conta dos ícones
- npm install react-native-svg
- npm install react-native-svg-transformer


> Instalar Expoclient no emulado android
- expo client:install:android
- npm i metro-config --save-dev


> Listar Emuladores Criados no Android Studio
- ~/Android/Sdk/tools$ ./emulator -list-avds
> Rodar o emulador fora do android studio
- ./emulator -avd React_Native_Teste


* Deu um erro :: PANIC: Missing emulator engine program for 'x86' CPU.
* Preciso colocar as pastas do Android nas variáveis de ambiente
- https://medium.com/@khairold/setting-up-react-native-on-linux-without-android-studio-a65f3e011bbb

> configuração do proxy para gradle 
- https://stackoverflow.com/questions/41507037/how-to-set-proxy-server-for-gradle/41507323

* Não esquecer de instalar o JDK/JRE

> WINDOWS
> Se der erro de "Unable to load script. Make sure you're either running.....index.android.bundle"
> run the command in the root folder
> Reference: https://medium.com/@adityasingh_32512/solved-unable-to-load-script-from-assets-index-android-bundle-bdc5e3a3d5ff
- react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res

> LINUX
> Reference: https://stackoverflow.com/questions/55441230/unable-to-load-script-make-sure-you-are-either-running-a-metro-server-or-that-yo
You haven't started the bundler yet. Run ```npm start``` or ```react-native start``` in the root directory of your project before ```react-native run-android```.


## Pra rodar o projeto

- npm start
- npx react-native run-android