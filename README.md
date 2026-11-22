# Perchon TV — archivos de actualizacion para GitHub Pages

Repo destino (A CREAR): Coque6966/perchon-tv-updates (publico)
GitHub Pages: https://coque6966.github.io/perchon-tv-updates/

## Archivos
- coque-tv-tv-update.json  -> TV, v1.9.6 (code 17), APK coque-tv-tv-v1.9.6.apk
- coque-tv-update.json     -> telefono, v1.5.5 (code 11), APK coque-tv-v1.5.5.apk

## Publicar (cuando el repo exista y haya credencial con escritura)
cd ~/perchon-tv-pages && git init -b main && git add . && git commit -m "Perchon TV v1.9.6 TV + v1.5.5 telefono" && git remote add origin <remote-del-repo> && git push -u origin main
Luego en GitHub: Settings > Pages > Source: Deploy from a branch, main / (root).
Verificar: curl -sI https://coque6966.github.io/perchon-tv-updates/coque-tv-update.json

## PROHIBIDO
NUNCA subir remote-kit.json aqui: contiene el acceso al portal. Solo estos 4 archivos.

## Actualizar una version nueva
Copiar el APK nuevo a este directorio y reescribir su apkUrl en el JSON
correspondiente a https://coque6966.github.io/perchon-tv-updates/<apk>, commit y push.
