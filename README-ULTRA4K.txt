# ULTRA4K PREMIUM

Aplicación Android / Android TV / Google TV con interfaz premium en negro, verde biche y blanco.

## Archivos principales
- `index.html`: renovación visual integral premium; mantiene la lógica, navegación, listas, favoritos, historial, perfiles, ajustes y controles existentes.
- `capacitor.config.json`: nombre ULTRA4K y `appId` original `com.glystv.app` conservado para permitir actualizar la instalación existente.
- `build-glystv-v3.sh`: genera el proyecto Android y conserva los motores de reproducción integrados.
- `patch_tv.py`: registra la etiqueta y el launcher de Android TV / Google TV.
- `glystv-res.zip`, `icon.png`, `banner.png`, `banner-hd.png`: recursos gráficos de la aplicación y launcher.
- `.github/workflows/build.yml`: compilación automática de APK mediante GitHub Actions.

## Funciones conservadas según el código del proyecto
- Inicio de sesión por servidor y carga manual de listas M3U.
- TV en vivo, películas, series, categorías y búsqueda.
- Favoritos, historial, continuar viendo y perfiles.
- Configuración, modo infantil y bloqueo de contenido mediante PIN.
- Control remoto con foco visible para navegación Android TV / Google TV.
- Reproductor ExoPlayer (Media3 + FFmpeg) y VLC (libVLC), con selección automática o manual del motor.
- Opciones de audio, subtítulos, relación de aspecto, velocidad, saltos y reanudación disponibles según el reproductor.

## Compilar
1. Sube los archivos del proyecto conservando sus rutas al repositorio GitHub.
2. Ejecuta el workflow `Build ULTRA4K Android` desde Actions o realiza un push a `main`.
3. Descarga el APK generado en la publicación `apk-<número de ejecución>`.

Nota: esta entrega actualiza el diseño visual y documentación; no reemplaza servicios del proveedor, credenciales, URLs ni contenido de las listas. La compilación final debe ejecutarse en GitHub Actions para verificar el entorno Android completo.
