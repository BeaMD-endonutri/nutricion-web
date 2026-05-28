# 🥗 Guía de Alimentación — Web para Pacientes de Nutrición

## 📁 Estructura de carpetas

```
nutricion-web/
├── index.html               ← Página principal (con las 4 categorías)
├── generar-qr.html          ← Herramienta para crear tu código QR
├── _gallery-template.html   ← Plantilla (no toques este archivo)
│
├── desayunos/
│   └── index.html           ← Galería de desayunos
├── almuerzos/
│   └── index.html           ← Galería de almuerzos
├── meriendas/
│   └── index.html           ← Galería de meriendas
└── cenas/
    └── index.html           ← Galería de cenas
│
└── img/
    ├── desayunos/           ← Pon aquí las fotos de desayunos
    ├── almuerzos/           ← Pon aquí las fotos de almuerzos
    ├── meriendas/           ← Pon aquí las fotos de meriendas
    └── cenas/               ← Pon aquí las fotos de cenas
```

---

## 🚀 INSTALACIÓN PASO A PASO (GitHub Pages — GRATIS)

### Paso 1 — Crea una cuenta en GitHub
1. Ve a https://github.com
2. Haz clic en "Sign up" y crea tu cuenta gratuita

### Paso 2 — Crea un repositorio nuevo
1. Una vez dentro, haz clic en el botón verde **"New"**
2. Nómbralo: `nutricion-web` (sin espacios)
3. Marca la opción **"Public"**
4. Haz clic en **"Create repository"**

### Paso 3 — Sube todos los archivos
1. En la página del repositorio, haz clic en **"uploading an existing file"**
2. Arrastra TODA la carpeta `nutricion-web` (incluyendo subcarpetas)
3. Haz clic en **"Commit changes"**

### Paso 4 — Activa GitHub Pages
1. Ve a **Settings** (arriba del repositorio)
2. En el menú izquierdo, haz clic en **"Pages"**
3. En "Source" selecciona **"Deploy from a branch"**
4. En "Branch" elige **"main"** y carpeta **"/ (root)"**
5. Haz clic en **"Save"**

### Paso 5 — Tu URL estará lista en ~2 minutos
Tu web estará en:
```
https://TU-USUARIO.github.io/nutricion-web/
```
(Reemplaza TU-USUARIO por tu nombre de usuario de GitHub)

---

## 📸 CÓMO AÑADIR NUEVAS IMÁGENES

### Opción A — Directamente desde GitHub (más fácil)
1. Ve a tu repositorio en github.com
2. Entra a la carpeta `img/desayunos/` (o la que corresponda)
3. Haz clic en **"Add file" → "Upload files"**
4. Sube las fotos
5. Haz clic en **"Commit changes"**

### Opción B — Desde tu ordenador
1. Copia las imágenes a la carpeta `img/desayunos/` (o la que corresponda)
2. Vuelve a subir los archivos a GitHub

### Después de subir imágenes — REGISTRO OBLIGATORIO
Abre el archivo de la categoría correspondiente (ej: `desayunos/index.html`)
con un editor de texto (Bloc de Notas, TextEdit, VS Code, etc.)

Busca esta sección (está al inicio del `<script>`):

```javascript
desayunos: {
    images: [
      // Ejemplo: 'tostadas-aguacate.jpg',
    ]
  },
```

Añade el nombre de cada imagen nueva:

```javascript
desayunos: {
    images: [
      'tostadas-aguacate.jpg',
      'bowl-frutas.jpg',
      'avena-platano.jpg',
    ]
  },
```

⚠️ El nombre debe ser EXACTAMENTE igual al nombre del archivo (mayúsculas/minúsculas importan).

---

## 📱 GENERAR EL CÓDIGO QR

1. Abre el archivo `generar-qr.html` en tu navegador
   (o accede a `https://TU-USUARIO.github.io/nutricion-web/generar-qr.html`)
2. Introduce la URL de tu web
3. Haz clic en **"Generar código QR"**
4. Descarga el QR en PNG
5. Imprímelo o compártelo con tus pacientes

Si cambias de URL (por ejemplo, cambias de GitHub a otro hosting), solo vuelve a abrir esta herramienta, introduce la nueva URL y descarga un nuevo QR.

---

## 💡 CONSEJOS PARA LAS IMÁGENES

- **Tamaño recomendado**: 800×600 px o similar (no más de 2MB por foto)
- **Formatos soportados**: JPG, PNG, WebP, GIF
- **Nombres de archivo**: Usa guiones en lugar de espacios
  ✅ `tostadas-aguacate.jpg`
  ❌ `tostadas aguacate.jpg`
- **Orientación**: Las fotos verticales (retrato) se ven especialmente bien en la galería

---

## 🔧 PERSONALIZACIÓN BÁSICA

### Cambiar el nombre del nutricionista (título de la web)
Abre `index.html` y busca:
```html
<div class="logo-pill">... Tu nutricionista</div>
<h1>Guía de<br/><span>Alimentación</span></h1>
```
Reemplaza el texto por el tuyo.

### Cambiar los colores
Abre cualquier `index.html` y busca `:root {` al inicio del CSS.
Cambia los valores de color, por ejemplo:
```css
--sage:    #7a9e7e;   /* Color principal (verde sage) */
--sage-dk: #4d7a53;   /* Color oscuro (botones y acentos) */
--cream:   #faf8f3;   /* Color de fondo */
```

---

## ❓ PREGUNTAS FRECUENTES

**¿Es gratis para siempre?**
Sí. GitHub Pages es gratis para repositorios públicos sin límite de tiempo.

**¿Puedo usar un dominio propio?**
Sí. En GitHub Pages > Settings > Custom domain puedes añadir tu propio dominio.

**¿Mis pacientes necesitan cuenta de GitHub?**
No. Solo necesitan escanear el QR o acceder a la URL.

**¿Cuántas imágenes puedo subir?**
GitHub Pages soporta repositorios de hasta 1GB, suficiente para cientos de fotos.

---

¡Cualquier duda, abre el archivo en un editor de texto y los comentarios te guiarán! 🌿
