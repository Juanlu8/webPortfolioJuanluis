# Portfolio Web - Juan Lu

Portfolio web personal moderno y responsive, desarrollado con HTML, CSS y JavaScript vanilla.

## 🎨 Características

- **Diseño Moderno**: Interfaz limpia y profesional inspirada en portfolios de alto nivel
- **Responsive**: Adaptado a todos los dispositivos (móvil, tablet y desktop)
- **Animaciones Suaves**: Transiciones y efectos visuales cuidados
- **Navegación Fluida**: Scroll suave entre secciones
- **Interactividad**: Efectos de hover, parallax y cursor personalizado
- **Optimizado**: Código limpio y rendimiento optimizado
- **Accesible**: Diseño pensado para todos los usuarios

## 📁 Estructura del Proyecto

```
portfolioweb-juanlu/
│
├── index.html          # Estructura principal del sitio
├── styles.css          # Estilos y diseño responsive
├── script.js           # Interactividad y animaciones
└── README.md           # Este archivo
```

## 🚀 Cómo Usar

### Opción 1: Abrir directamente

1. Abre el archivo `index.html` en tu navegador favorito
2. ¡Listo! El portfolio ya está funcionando

### Opción 2: Servidor local (recomendado para desarrollo)

Si estás usando VS Code, puedes usar la extensión "Live Server":

1. Instala la extensión "Live Server" en VS Code
2. Click derecho en `index.html`
3. Selecciona "Open with Live Server"

O usa Python para crear un servidor simple:

```bash
# Python 3
python -m http.server 8000

# Luego abre en tu navegador
# http://localhost:8000
```

## ✏️ Personalización

### 1. Información Personal

Edita el archivo `index.html` para actualizar:

- **Línea 37-39**: Tu nombre y título
- **Línea 42-45**: Descripción personal
- **Línea 267-272**: Información de contacto
- **Línea 281-299**: Enlaces a redes sociales

### 2. Proyectos

En `index.html`, sección "Proyectos Destacados" (líneas 135-228):

- Modifica los títulos, descripciones y tecnologías
- Actualiza los enlaces a tus proyectos y GitHub
- Agrega tus propias imágenes en `.project-placeholder`

### 3. Habilidades

En `index.html`, sección "Habilidades" (líneas 236-262):

- Actualiza las listas de tecnologías según tu experiencia
- Añade o elimina categorías según necesites

### 4. Colores y Estilo

Edita `styles.css`, variables CSS (líneas 6-21):

```css
--color-accent: #3b82f6;        /* Color principal */
--color-accent-hover: #2563eb;  /* Color hover */
--color-bg: #0a0a0a;            /* Fondo principal */
--color-text: #e4e4e7;          /* Color de texto */
```

### 5. Fuentes

Las fuentes actuales son:
- **Inter**: Para texto general
- **Space Grotesk**: Para títulos

Puedes cambiarlas editando el `<link>` en el `<head>` de `index.html` (líneas 9-11)

## 🎯 Secciones del Portfolio

1. **Hero**: Presentación inicial con tu nombre y título
2. **Sobre mí**: Descripción personal y filosofía de trabajo
3. **Proyectos**: Muestra de trabajos destacados
4. **Habilidades**: Tecnologías y herramientas que dominas
5. **Contacto**: Información de contacto y redes sociales

## 🔧 Funcionalidades Implementadas

### JavaScript:
- ✅ Menú de navegación responsive con hamburger menu
- ✅ Scroll suave entre secciones
- ✅ Resaltado de navegación activa
- ✅ Animaciones de entrada con Intersection Observer
- ✅ Efecto de escritura (typing effect)
- ✅ Cursor personalizado
- ✅ Efecto parallax en el hero
- ✅ Efecto tilt en tarjetas de proyectos
- ✅ Botón de scroll to top
- ✅ Notificaciones

### CSS:
- ✅ Variables CSS para fácil personalización
- ✅ Diseño responsive con media queries
- ✅ Animaciones y transiciones suaves
- ✅ Grid y Flexbox para layouts modernos
- ✅ Efectos hover interactivos
- ✅ Dark mode optimizado

## 📱 Compatibilidad

- ✅ Chrome/Edge (últimas versiones)
- ✅ Firefox (últimas versiones)
- ✅ Safari (últimas versiones)
- ✅ Dispositivos móviles (iOS y Android)

## 🎨 Recursos para Imágenes de Proyectos

Cuando quieras agregar imágenes reales a tus proyectos, puedes usar:

- [Unsplash](https://unsplash.com/) - Fotos de alta calidad gratuitas
- [Pexels](https://www.pexels.com/) - Videos e imágenes gratuitas
- Capturas de pantalla de tus proyectos reales

## 📝 Próximos Pasos Recomendados

1. **Personaliza el contenido** con tu información real
2. **Agrega imágenes** a los proyectos
3. **Actualiza los enlaces** a tus redes sociales y repositorios
4. **Añade tu email** real en la sección de contacto
5. **Opcional**: Integra un formulario de contacto con servicios como:
   - [Formspree](https://formspree.io/)
   - [EmailJS](https://www.emailjs.com/)
   - [Netlify Forms](https://www.netlify.com/products/forms/)

## 🌐 Despliegue

Puedes desplegar tu portfolio gratuitamente en:

### Netlify
1. Crea una cuenta en [Netlify](https://www.netlify.com/)
2. Arrastra tu carpeta al área de despliegue
3. ¡Listo! Tu sitio está en línea

### GitHub Pages
1. Sube tu código a un repositorio de GitHub
2. Ve a Settings > Pages
3. Selecciona la rama main
4. Tu sitio estará en `https://tuusuario.github.io/repositorio`

### Vercel
1. Crea una cuenta en [Vercel](https://vercel.com/)
2. Importa tu repositorio de GitHub
3. Despliegue automático

## 📄 Licencia

Este proyecto es de código abierto y está disponible para uso personal y comercial.

## 🤝 Inspiración

Este portfolio está inspirado en los trabajos de:
- [Robb Owen](https://robbowen.digital/) - Diseño limpio y profesional
- [Seyi](https://www.seyi.dev/) - Creatividad y presentación moderna

## 💡 Consejos

- Mantén el contenido conciso y relevante
- Usa imágenes de alta calidad para tus proyectos
- Actualiza regularmente con nuevos proyectos
- Asegúrate de que todos los enlaces funcionen
- Prueba el sitio en diferentes dispositivos
- Optimiza las imágenes para web (usa WebP si es posible)

---

**¡Buena suerte con tu portfolio! 🚀**

Si tienes preguntas o necesitas ayuda, no dudes en buscar recursos en la comunidad de desarrollo web.
