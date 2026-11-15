# GLYSTVULTRA — actualización TV-first

Archivos modificados:
- `index.html`: marca GLYSTVULTRA, tema premium azul, navegación D-pad/OK y foco visible.
- `capacitor.config.json`: nombre de aplicación GLYSTVULTRA (se conserva `appId` para permitir actualizar la instalación existente).
- `patch_tv.py`: nombre visible GLYSTVULTRA y registro de launcher Android TV/Google TV.
- `.github/workflows/build.yml`: nombres de compilación GLYSTVULTRA.
- `package.json`: nombre/versión del proyecto.

## Compilar
Sube los archivos al repositorio manteniendo sus rutas y ejecuta el workflow **Build GLYSTVULTRA Android**.

## Control remoto
Las tarjetas y controles reciben foco con las flechas. El foco solo resalta; no abre contenido. Para abrir se pulsa OK/Enter. Atrás/Escape conserva el comportamiento de cierre/retroceso de la aplicación.

## Reproductores
El proyecto original incluye Media3/ExoPlayer nativo con decodificador FFmpeg, HLS.js y reproducción HTML5 del WebView. Son rutas/motores de reproducción disponibles según plataforma y formato; no se han agregado APKs externos de VLC o MX Player ni se debe afirmar que estén instalados. La app debe seleccionar el motor compatible y probarse con las listas reales del proveedor.
