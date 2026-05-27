🤾 ¡Aprende Balonmano! — Infografía PWA Interactiva

Infografía digital interactiva diseñada para enseñar los fundamentos del balonmano a niños de 8 a 12 años, basada en los principios de diseño instruccional de Mayer.

HTML5CSS3JavaScriptPWA

📋 Tabla de Contenidos

🎯 Propósito Pedagógico
✨ Características Principales
🎮 Efectos Interactivos Especiales
🛠️ Tecnologías Utilizadas
🚀 Cómo Ejecutar el Proyecto
📱 Instalación como PWA
 ♿ Accesibilidad
📁 Estructura del Archivo
📄 Licencia y Créditos
🎯 Propósito Pedagógico

Basado en los criterios de Mayer para el diseño multimedia educativo:

Idea central única: El objetivo del balonmano es marcar goles.
3 a 5 datos clave: 7 jugadores, 3 pasos, 30 minutos, zona de 6 metros.
Narrativa guiada: La mascota "Leo" 🦁 guía al niño con preguntas y tono lúdico.
Estructura lineal: Navegación vertical simple, sin menús complejos.
Principio de coherencia: Solo elementos con función didáctica, cero decoración innecesaria.
✨ Características Principales

🦁 Mascota animada: "Leo" salta y se mueve guiando al usuario.
📊 Datos clave interactivos: Cards con efecto flip para descubrir más información.
🎯 Pasos secuenciales: Cubos 3D rotantes que explican cómo anotar.
🏟️ Campo deportivo SVG: Representación visual del campo con zonas y medidas.
🧠 Quiz interactivo: 4 preguntas con feedback visual inmediato (correcto/incorrecto).
📱 PWA Instalable: Funciona offline y se puede instalar en móviles y escritorio.
🎮 Efectos Interactivos Especiales

Se implementaron tres efectos hover avanzados pensados para sorprender y engagement a niños:

🟢 Liquid Morph (Idea Central): La tarjeta principal del "¡GOL!" cambia de forma orgánica continua usando @keyframes morph en el border-radius, y reacciona al hover escalando y elevándose.
🔵 Double-Sided Card (Datos Clave): Las 4 tarjetas de datos giran 180° en el eje Y (rotateY) al pasar el cursor o tocar, revelando información extra en la cara trasera.
🟡 Rotating Cube (Pasos para Anotar): Los 3 pasos están en cubos 3D con 4 caras (preserve-3d). Cada toque rota el cubo 90° para descubrir un nuevo detalle del paso.
🛠️ Tecnologías Utilizadas

Tecnología	Uso
HTML5 Semántico	Estructura accesible (<header>, <main>, <section>, <footer>)
CSS3	Animaciones (@keyframes), 3D Transforms, Grid, Flexbox
JavaScript Vanilla	Lógica del quiz, rotación de cubos, PWA inline
Google Fonts	Baloo 2 (títulos) + Nunito (cuerpo)
SVG	Dibujo vectorial del campo deportivo
Web App Manifest	Manifest embebido como Data URI
Service Worker	SW inline vía Blob URL para caché offline
🚀 Cómo Ejecutar el Proyecto

Opción 1: Apertura directa

Simplemente descarga el archivo balonmano-ninos.html y ábrelo en cualquier navegador moderno.

# Haz doble clic en el archivo o:open balonmano-ninos.html      # macOSstart balonmano-ninos.html     # Windowsxdg-open balonmano-ninos.html  # Linux
Opción 2: Servidor local (Recomendado para PWA)

Para que el Service Worker y el Manifiesto funcionen correctamente, sirve el archivo desde un servidor local:

bash

# Con Python 3
python3 -m http.server 8080

# Con Node.js (npx)
npx serve .

# Con VS Code
# Instala la extensión "Live Server" y haz clic en "Go Live"
Luego abre http://localhost:8080/balonmano-ninos.html en tu navegador.

📱 Instalación como PWA

La aplicación incluye un Service Worker y un Web App Manifest embebidos, lo que permite:

Instalarla en la pantalla de inicio de dispositivos móviles.
Usarla sin conexión a internet (offline).
Experiencia de app nativa (sin barra de navegación del navegador).
 💡 Nota: El banner de instalación aparece automáticamente en navegadores compatibles (Chrome, Edge, Samsung Internet). También puedes usar el icono "Instalar" del navegador.

♿ Accesibilidad

El proyecto cumple con estándares de accesibilidad digital:

 ✅ Jerarquía de encabezados (h1 → h2 → h3)
 ✅ aria-label en elementos interactivos
 ✅ aria-live="polite" en feedback del quiz (lectores de pantalla)
 ✅ role="button" y role="img" donde corresponde
 ✅ tabindex="0" para navegación por teclado
 ✅ Navegación con Enter/Space en cubos y cards
 ✅ alt text descriptivo en SVG
 ✅ prefers-reduced-motion respeta la configuración del usuario
 ✅ Touch targets ≥ 44x44px para uso móvil
📁 Estructura del Archivo

Al ser un archivo único autocontenido, toda la aplicación se divide internamente en:

text

balonmano-ninos.html
├── <head>
│   ├── Meta tags (viewport, theme-color, PWA)
│   ├── Google Fonts (Baloo 2, Nunito)
│   ├── <style> — CSS completo (variables, keyframes, layout, responsive)
│   └── <link rel="manifest"> — Data URI embebido
│
├── <body>
│   ├── <header> — Hero con mascota
│   ├── <main>
│   │   ├── <section> Burbuja guía
│   │   ├── <section> Idea central (Liquid Morph)
│   │   ├── <section> Datos clave (Double-Sided Cards)
│   │   ├── <section> Pasos (Rotating Cubes)
│   │   ├── <section> El campo (SVG)
│   │   ├── <section> El portero
│   │   └── <section> Quiz interactivo
│   ├── <footer> — Créditos y datos académicos
│   ├── PWA Install Banner
│   └── <script> — JS (quiz, cubos, Service Worker, Manifest)
📄 Licencia y Créditos

CAMPO
DETALLE
Autor	Cesar Nuñez Carranza
Institución	UTP — Universidad Tecnológica del Perú
Asignatura	INFOGRAFÍA
Año	2026
Contenido basado en	Infografía de balonmano publicada por EL MUNDO (Coordina: F.A. Anguís · Textos: Carolina G. Miranda)
 
 🤾 "¡El balonmano te espera, atrapa el balón y juega!" 🦁