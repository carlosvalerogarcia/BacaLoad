# 🐟 BacaLoad - Descargador Multimedia (Windows & Linux)

**BacaLoad** es una aplicación de escritorio moderna, rápida y muy fácil de usar para descargar música, audios y vídeos de tus plataformas favoritas con la máxima calidad y sin marcas de agua. Compatible tanto con **Windows** como con **Linux**.

Permite guardar tus descargas directamente en tu ordenador o **pasarlas al instante a tu teléfono móvil (iPhone o Android) sin cables**, escaneando un sencillo código QR con la cámara.

---

## ✨ ¿Para qué sirve y qué puedes descargar?

### 🔴 YouTube
- **Vídeo Completo**: Descarga vídeos a máxima resolución (1080p, 4K, 60fps) en formato MP4 limpio con aceleración multihilo.
- **Solo Audio (MP3)**: Extrae el audio a 320 kbps (máxima calidad musical) con metadatos y carátula oficial.
- **Recortar Fragmentos**: Selecciona el minuto de inicio y de fin (por ejemplo de `01:30` a `03:45`) para descargar solo la parte que te interesa con reconexión automática.
- **Letras y Subtítulos**: Extrae letras sincronizadas en formato `.lrc` si el vídeo dispone de ellas.

### 🟢 Spotify
- **Canciones y Listas Completas**: Descarga temas individuales o álbumes completos con descarga rápida en paralelo (4 hilos).
- **Calidad de Estudio**: Audio a 320 kbps con carátula oficial del álbum, nombre del artista y metadatos incrustados automáticamente.
- **Letras Sincronizadas (.lrc)**: Descarga el archivo de letra sincronizada para cantar o ver la letra en tiempo real en reproductores compatibles (móvil, pantalla del coche, etc.).

### 🟣 Twitch (Público y Con Suscripción)
- **Directos y VODs**: Descarga directos completos a máxima velocidad.
- **Recortar Clips**: Descarga solo un fragmento exacto del directo especificando los tiempos.
- **Soporte TwitchNoSub**: Compatible con enlaces directos para recuperar directos de suscriptores sin restricciones.

### 📱 TikTok e Instagram
- **Vídeos sin Marca de Agua**: Descarga vídeos de TikTok y Reels de Instagram con la máxima calidad original.
- **Solo Audio (MP3)**: Extrae el audio de cualquier tendencia o sonido viral para guardarlo como música o tono.

### 📲 Transferencia al Móvil vía Código QR (Sin Cables)
- **Directo a tu teléfono**: Pulsa el botón *"Descargar para Móvil"* y aparecerá un código QR al terminar.
- **Sin instalar nada en el móvil**: Solo tienes que apuntar la cámara de tu smartphone (iPhone o Android) al QR y se abrirá una pantalla web para reproducir y guardar la canción o vídeo en tu móvil.
- **Misma red WiFi**: Solo requiere que el PC y el teléfono estén en la misma red WiFi.

### 🎚️ Normalizador de Sonido Inteligente
- Si activas la casilla de normalización de audio, la aplicación equilibra automáticamente el volumen del archivo para que todas tus canciones suenen al mismo nivel, sin sobresaltos ni canciones más bajas que otras.

### 🔄 Actualizaciones con 1 Clic (Estilo Discord)
- La aplicación comprueba automáticamente si hay nuevas mejoras y te mostrará un botón verde en la barra superior. Con solo un clic, la app se actualiza y se reinicia sola tanto en Windows como en Linux.

---

## 🚀 Cómo se usa

1. **Abre BacaLoad**: Haz doble clic en el acceso directo de tu Escritorio (o ejecuta `./run_linux.sh` en Linux).
2. **Selecciona la pestaña** según lo que quieras descargar (YouTube, Spotify, Twitch o Redes Sociales).
3. **Pega el enlace**: Pulsa el botón **📋 Pegar** para que cargue la vista previa de la canción o vídeo.
4. **Elige las opciones que quieras**:
   - Calidad de vídeo, solo audio MP3 o recortar fragmento.
   - Si quieres letras sincronizadas o normalizar el volumen.
5. **Descarga**:
   - Pulsa **📥 Descargar en PC** para guardarlo en la carpeta de tu ordenador.
   - O pulsa **📲 Descargar para Móvil (QR)** para pasarlo directamente a tu teléfono.

---

## 🐧 Uso en Linux (Ubuntu, Debian, Fedora, Arch...)

BacaLoad cuenta con soporte nativo para distribuciones Linux:

1. **Requisitos previos (Tkinter, venv y FFmpeg)**:
   - Ubuntu / Debian / Linux Mint:
     ```bash
     sudo apt update && sudo apt install -y python3-tk python3-venv ffmpeg
     ```
   - Fedora / RHEL:
     ```bash
     sudo dnf install -y python3-tkinter python3-pip ffmpeg
     ```
   - Arch Linux / Manjaro:
     ```bash
     sudo pacman -S --noconfirm tk python-pip ffmpeg
     ```
2. **Ejecutar BacaLoad**:
   ```bash
   chmod +x run_linux.sh setup_linux.sh
   ./run_linux.sh
   ```
3. **Instalar acceso directo en el Escritorio y Menú de Linux**:
   - Ejecuta `./setup_linux.sh` y se creará automáticamente el lanzador con el icono oficial en tu menú de aplicaciones y en tu Escritorio.

---

## 📁 Organización de Carpetas

- **`Abrir BacaLoad.lnk`**: Acceso directo principal para abrir la aplicación al instante en Windows.
- **`1 - Windows (Ejecutable)`**: Versión portátil para Windows (`BacaLoad.exe`), lista para usar sin necesidad de instalar Python ni librerías.
- **`2 - Linux (Scripts y Ejecución)`**: Versión limpia para Linux con su lanzador automático (`run_linux.sh`), instalador de accesos directos (`setup_linux.sh`), instrucciones y subcarpeta `src/` que guarda los archivos internos.
- **`3 - Para Enviar (ZIP Portátil)`**: Archivo ZIP multi-plataforma organizado con subcarpetas para Windows y Linux.
- **`4 - Código Fuente (Python)`**: Archivos fuente completos (`app.py`, `core.py`, `gui.py`, etc.) para desarrolladores.
- **`5 - Logos e Imágenes`**: Iconos y logotipos oficiales en alta definición.

---

## ⚙️ Ajustes útiles

- **Cambiar carpeta de guardado**: En la esquina superior derecha puedes hacer clic en **📁 Cambiar** para elegir dónde quieres que se guarden tus archivos.
- **Pestaña Herramientas**: Puedes comprobar el estado de los componentes y buscar actualizaciones manualmente en cualquier momento.
