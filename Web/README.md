# Página Web Musical del Artista

Una página web dinámica y moderna para presentar a un artista con reproductor de audio y galería de imágenes de conciertos.

## 🎵 Características

- **Diseño moderno y responsive**: Se adapta a diferentes tamaños de pantalla
- **Reproductor de audio**: Con controles de reproducción, volumen y lista de canciones
- **Galería de imágenes**: Muestra fotos de conciertos con efectos visuales
- **Información del artista**: Sección para biografía y detalles

## 📁 Estructura de Archivos

```
Web/
├── index.html          # Página principal
├── audio/             # Carpeta para archivos de audio (crear esta carpeta)
│   ├── cancion1.mp3
│   ├── cancion2.mp3
│   └── cancion3.mp3
└── images/            # Carpeta para imágenes (opcional, puedes usar URLs)
    └── conciertos/
```

## 🎨 Personalización

### 1. Cambiar el nombre del artista
Edita en `index.html`:
- Línea con `id="artist-name"`: Cambia "Nombre del Artista"
- Línea con `id="current-track-artist"`: Cambia el nombre del artista

### 2. Agregar tus canciones
1. Crea una carpeta llamada `audio` en la misma carpeta que `index.html`
2. Coloca tus archivos MP3 en esa carpeta
3. Edita las líneas en `index.html` donde dice `data-src="audio/cancion1.mp3"` y cambia:
   - `data-src`: La ruta a tu archivo de audio
   - `data-title`: El nombre de la canción
   - `data-artist`: El nombre del artista

Ejemplo:
```html
<div class="playlist-item" data-src="audio/mi-cancion.mp3" data-title="Mi Canción Favorita" data-artist="Nombre del Artista">
```

### 3. Agregar imágenes de conciertos
Tienes dos opciones:

**Opción A: Usar imágenes locales**
1. Crea una carpeta `images` o `img` en tu proyecto
2. Coloca tus imágenes allí
3. Cambia las URLs en las etiquetas `<img>`:
```html
<img src="images/concierto1.jpg" alt="Concierto 1">
```

**Opción B: Usar URLs de internet**
Simplemente reemplaza la URL en el atributo `src`:
```html
<img src="https://tudominio.com/imagen.jpg" alt="Concierto 1">
```

### 4. Cambiar la biografía
Edita el texto dentro de la sección `.artist-info` en `index.html`

### 5. Cambiar colores
Los colores principales están en el CSS:
- Gradiente de fondo: `background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);`
- Puedes cambiarlos por otros colores que prefieras

## 🚀 Cómo Subir tu Página a Internet

### Opción 1: GitHub Pages (GRATIS y FÁCIL) ⭐ RECOMENDADO

1. **Crear cuenta en GitHub**
   - Ve a [github.com](https://github.com) y crea una cuenta gratuita

2. **Crear un repositorio**
   - Haz clic en el botón "+" en la esquina superior derecha
   - Selecciona "New repository"
   - Nómbralo (ej: "pagina-artista")
   - Marca "Public"
   - Haz clic en "Create repository"

3. **Subir tus archivos**
   - Descarga GitHub Desktop o usa la web
   - Sube tu carpeta `Web` con todos los archivos
   - Haz commit y push

4. **Activar GitHub Pages**
   - Ve a Settings → Pages
   - En "Source" selecciona "main" branch
   - Haz clic en "Save"
   - Tu página estará disponible en: `https://tuusuario.github.io/pagina-artista`

### Opción 2: Netlify (GRATIS y MUY FÁCIL)

1. Ve a [netlify.com](https://netlify.com) y crea una cuenta gratuita
2. Arrastra y suelta tu carpeta `Web` en la página de Netlify
3. ¡Listo! Tu página estará online en segundos
4. Obtendrás una URL como: `https://tu-pagina.netlify.app`

### Opción 3: Vercel (GRATIS)

1. Ve a [vercel.com](https://vercel.com) y crea una cuenta
2. Conecta tu repositorio de GitHub o sube los archivos directamente
3. Tu página estará online automáticamente

### Opción 4: Firebase Hosting (GRATIS)

1. Instala Firebase CLI: `npm install -g firebase-tools`
2. Inicia sesión: `firebase login`
3. Inicializa: `firebase init hosting`
4. Despliega: `firebase deploy`

### Opción 5: Servidor Web Tradicional

Si tienes un hosting tradicional:
1. Sube todos los archivos vía FTP
2. Asegúrate de que `index.html` esté en la raíz
3. Crea las carpetas `audio` e `images` si las usas

## 📝 Notas Importantes

- **Archivos de audio**: Asegúrate de tener los derechos para usar las canciones
- **Tamaño de archivos**: Los archivos grandes pueden tardar en cargar. Considera comprimir imágenes y audio
- **Formatos soportados**: El reproductor funciona con MP3, OGG, WAV
- **Navegadores**: Funciona en Chrome, Firefox, Safari, Edge (navegadores modernos)

## 🎯 Próximos Pasos

1. Personaliza el contenido con la información de tu artista
2. Agrega tus canciones en formato MP3
3. Agrega tus imágenes de conciertos
4. Sube todo a GitHub Pages, Netlify o Vercel
5. Comparte el enlace con tus amigos

## 💡 Consejos

- Prueba la página localmente antes de subirla (abre `index.html` en tu navegador)
- Usa nombres de archivo sin espacios ni caracteres especiales
- Optimiza las imágenes antes de subirlas (usa herramientas como TinyPNG)
- Mantén los archivos de audio en formato MP3 para mejor compatibilidad

¡Disfruta compartiendo tu página musical! 🎵

