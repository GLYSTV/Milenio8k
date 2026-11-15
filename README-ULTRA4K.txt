# ULTRA4K — antes GLYSTVULTRA

Colores de marca: verde biche #8CC63F · verde profundo #5E9E2A · blanco #FFFFFF · fondo #0A0C08

Archivos modificados:
- index.html: marca ULTRA4K, tema verde biche + blanco, navegación D-pad/OK y foco visible.
- capacitor.config.json: appName ULTRA4K (el appId com.glystv.app se conserva para poder actualizar la instalación existente).
- patch_tv.py: etiqueta ULTRA4K y registro de launcher Android TV / Google TV con banner.
- glystv-res.zip: iconos del launcher (mipmap) nuevos en verde biche.
- icon.png (1024x1024), banner.png (320x180, Android TV), banner-hd.png (1280x720).
- .github/workflows/build.yml y package.json: nombres ULTRA4K.

Compilar: sube todo al repositorio manteniendo las rutas y ejecuta el workflow "Build ULTRA4K Android".

## Reproductores (v3.1)
- VLC (libVLC 3.6.0, org.videolan.android:libvlc-all): pantalla propia VlcPlayerActivity con audio/subtítulos/aspecto/velocidad, saltos de 10 s, reanudar y cola de episodios. Solo arm64-v8a y armeabi-v7a.
- ExoPlayer (Media3 1.4.1 + decodificador FFmpeg): reproductor original.
- Configuración > Motor de reproducción: Automático (ExoPlayer y, si falla, VLC) · VLC · ExoPlayer.
- La vista previa embebida de TV en vivo sigue usando ExoPlayer; la pantalla completa usa el motor elegido.
- Control remoto en VLC: OK pausa/menú, ←/→ saltar, ↑/↓ menú, CH+/CH- siguiente/anterior.
