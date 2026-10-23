# Placar do Duelo (Android)

## Opção A: gerar o APK sem instalar nada (GitHub)
1. Crie um repositório no GitHub e envie todo o conteúdo desta pasta (inclusive .github).
2. Aba Actions > "Gerar APK" > Run workflow.
3. Ao terminar (uns 5 min), baixe o artefato "placar-duelo-apk", extraia e instale o app-debug.apk no celular
   (permita "instalar apps de fontes desconhecidas").

## Opção B: Android Studio
npm install
npx cap add android
npx cap sync android
npx cap open android   # Run no emulador/celular ou Build > Build APK(s)

Para publicar na Play Store, gere um AAB assinado (Build > Generate Signed Bundle).
Depois de editar www/index.html, rode: npx cap sync android
