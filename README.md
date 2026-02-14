<h1 align="center"> 💖 San Valentín Interactivo 💖 </h1>

¡Bienvenido/a a este proyecto especial de San Valentín! 👋

Este sitio web interactivo está diseñado para hacer una pregunta muy importante: **¿Serías mi San Valentín?** Con animaciones, imágenes y un toque de humor, este proyecto es perfecto para sorprender a tu persona especial.

## 📸 Vista previa

Modo Claro ☀️:
![Vista previa Modo Claro](img/imgSVClaro.png)

Modo Oscuro 🌑:
![Vista previa Modo Oscuro](img/imgSVOscuro.png)

## 🚀 Características Principales

- **Pregunta Interactiva:** Un botón de "Sí" y un botón de "No" con comportamientos únicos.
  - El botón **"Sí"** muestra una galería de 6 imágenes de gatitos Mochi Peach Cat y un mensaje de amor.
  - El botón **"No"** se escala en el primer click y luego se mueve aleatoriamente por la pantalla, haciéndolo imposible de presionar. Muestra una imagen divertida y un mensaje burlón.
- **Modo Oscuro:** Un botón para cambiar entre modo claro y oscuro.
- **Animaciones:** Efecto `fadeIn` para la galería de imágenes y `slideIn` para el mensaje de respuesta.
- **Diseño Responsivo:** Grid de 2 columnas en móvil y 3 columnas en escritorio (breakpoint en 768px).

## ⚙️ Instalación

1. **Clona el repositorio:**
   ```bash
   git clone <url-del-repositorio>
   ```

2. **Abre `index.html`** directamente en tu navegador.

3. **(Opcional)** Usa la extensión **Live Server** de VS Code (configurado en el puerto 5501).

## 📚 Uso

- Haz clic en **"Sí"** para ver la galería de imágenes y un mensaje especial.
- Intenta hacer clic en **"No"** — en el primer click se escala, después se mueve por toda la pantalla y muestra una imagen divertida.
- Usa el botón **"Modo Oscuro 🌙"** para cambiar entre temas.

![Vista previa de la galería](img/imgSVGalería.png)

## 🛠️ Tecnologías utilizadas

<p align="center">
  <img src="https://img.icons8.com/?size=100&id=20909&format=png&color=000000" alt="HTML5" width="80"/>
  <img src="https://img.icons8.com/?size=100&id=21278&format=png&color=000000" alt="CSS3" width="80"/>
  <img src="https://img.icons8.com/?size=100&id=108784&format=png&color=000000" alt="JavaScript" width="80"/>
</p>

- **HTML5:** Estructura de la página.
- **CSS3:** Estilos responsivos con flexbox, animaciones y modo oscuro.
- **JavaScript:** Lógica de interactividad (botones, galería dinámica, reposicionamiento aleatorio del botón "No").

## 📁 Estructura del proyecto

```
├── index.html       # Página principal
├── script.js        # Lógica de interactividad
├── styles.css       # Estilos y animaciones
├── img/
│   ├── Mi.png       # Imagen mostrada al intentar presionar "No"
│   ├── imgSVClaro.png
│   ├── imgSVOscuro.png
│   └── imgSVGalería.png
└── paratu.html      # Página adicional
```

## 🎨 Personalización

- Cambia las imágenes de la galería en `script.js` (array `images`).
- Modifica los mensajes en `index.html` y `script.js` para hacerlos más personales.
- Ajusta los colores y estilos en `styles.css`.
