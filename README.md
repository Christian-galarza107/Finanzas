# Mis Finanzas

Aplicación de finanzas personales: saldo disponible, vencimientos, deudas, tarjetas y proyección mensual.
Funciona en el navegador, sin servidor y sin conexión. Se puede instalar en el celular como app.

## Privacidad

- Este repositorio **no contiene datos personales**. Es solo la aplicación.
- Tus datos se guardan en el navegador de cada dispositivo (localStorage). No se envían a ningún lado.
- **Nunca subas** respaldos `.json` ni archivos con tus datos: el `.gitignore` ya los excluye.
- localStorage no es un respaldo seguro. Exportá una copia desde **Configuración → Exportar respaldo** cada semana.

## Publicar en GitHub Pages

1. Entrá a <https://github.com/new>, poné de nombre `mis-finanzas`, elegí **Public** y creá el repositorio, sin README.
2. Hacé clic en **uploading an existing file** y arrastrá todo el contenido de esta carpeta, incluida la carpeta `icons`. Después tocá **Commit changes**.
3. Andá a **Settings → Pages**. En **Source** elegí **Deploy from a branch**, y en rama elegí `main` con carpeta `/ (root)`. Guardá.
4. En uno o dos minutos la app queda en `https://TU-USUARIO.github.io/mis-finanzas/`.

Con Git, desde esta carpeta:

```bash
git init -b main
git add .
git commit -m "Mis Finanzas: primera versión"
git remote add origin https://github.com/TU-USUARIO/mis-finanzas.git
git push -u origin main
```

## Instalar en el celular

- **Android (Chrome):** abrí el link, después menú ⋮ y **Instalar aplicación**.
- **iPhone (Safari):** abrí el link, después **Compartir** y **Agregar a pantalla de inicio**.

## Cargar tus datos

En la pantalla de bienvenida elegí **Tengo un respaldo** y seleccioná tu archivo `.json`.
Cada dispositivo guarda sus propios datos. Para pasarlos de uno a otro, exportá el respaldo en uno e importalo en el otro.

## Actualizar la app

Reemplazá `index.html` en el repositorio y hacé commit. La próxima vez que abras la app con conexión, ya carga la versión nueva.
Tus datos no se borran al actualizar.

## Archivos

| Archivo | Para qué |
|---|---|
| `index.html` | La aplicación completa |
| `manifest.webmanifest` | Permite instalarla como app |
| `sw.js` | Hace que funcione sin conexión |
| `icons/` | Íconos de la app |
