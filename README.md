# 📄 Rellenador y Firmador de PDF, Word e Imágenes Inteligente

Una aplicación web moderna, rápida y 100% cliente (sin servidores ni envíos de datos privados a la nube) para rellenar documentos PDF oficiales, convertir archivos Word (.docx), firmar digitalmente con trazo natural, unir fotocopias de DNI (anverso y reverso) y **crear documentos PDF a partir de múltiples imágenes ordenándolas mediante arrastrar y soltar (Drag & Drop)**.

---

## 🚀 Mejoras y Novedades Implementadas

1. **🎯 Posicionamiento Exacto del Texto**:
   - Al hacer clic en cualquier línea o casilla del documento, el texto se sitúa **exactamente donde has pinchado** (coincidencia perfecta entre el cursor visual, la línea base tipográfica en pantalla y las coordenadas reales del PDF generado).
   - Doble clic en cualquier parte de la hoja para escribir texto directamente en ese punto exacto.
   - Tecla <kbd>Enter</kbd> para insertar o guardar el texto al instante.

2. **🖐️ Selección y Arrastre Fluido (Drag & Drop)**:
   - Se ha solucionado el problema que impedía arrastrar los textos una vez escritos. Ahora puedes hacer clic en cualquier texto o firma y moverlo libremente con el ratón o con el dedo en pantallas táctiles de forma suave y sin retrasos.
   - **Ajuste fino milimétrico**:
     - Con las **flechas del teclado** (<kbd>←</kbd> <kbd>→</kbd> <kbd>↑</kbd> <kbd>↓</kbd>) para mover el elemento píxel a píxel.
     - Con <kbd>Shift</kbd> + flecha para moverlo de 5 en 5 píxeles.
     - Tecla <kbd>Supr</kbd> o <kbd>Retroceso</kbd> para borrar el elemento seleccionado y <kbd>Esc</kbd> para deseleccionar.
     - Botones de flechas de ajuste fino y controles de tamaño (+ / -) en la barra flotante.

3. **🖼️ Crear PDF desde Fotos y Reordenar Arrastrando**:
   - Nuevo botón **"Crear de Fotos"** en la barra superior (o abriendo fotos desde "Abrir Archivo"): selecciona varias imágenes a la vez y la app genera un PDF de alta resolución ajustado a páginas A4.
   - **Reordenación interactiva arrastrando y soltando**: en la cola de fotos/anexos, puedes agarrar cualquier imagen por el icono <i class="fa-solid fa-grip-vertical"></i> y arrastrarla arriba o abajo para colocarla en el orden exacto que quieras. Las páginas se reorganizan automáticamente en el visor en tiempo real.
   - También dispones de botones de flechas (↑ y ↓) para subir o bajar el orden con un solo clic.

4. **📑 Documentos Word (.docx) y DNI 2 Caras**:
   - Permite abrir documentos Word y convertirlos a PDF sin que los textos se corten.
   - Gestor de DNI para colocar anverso y reverso automáticamente en una única página A4 oficial.
   - Memoria local persistente (`localStorage`) para recordar tus datos habituales (Nombre, DNI, Dirección) y reutilizarlos con un toque.

---

## 🌐 Publicar en GitHub Pages (Gratis y accesible desde el móvil)

El proyecto incluye `index.html` listo para ser desplegado en **GitHub Pages**. Para subirlo a tu cuenta de GitHub:

### Paso 1: Configurar tu identidad en Git (si es la primera vez)
Abre tu consola (PowerShell o terminal) y escribe:
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu-email@ejemplo.com"
```

### Paso 2: Crear el repositorio en GitHub
1. Entra en [GitHub](https://github.com/) e inicia sesión.
2. Pulsa en el botón verde **"New"** (Nuevo repositorio).
3. Ponle un nombre (por ejemplo: `rellenador-pdf-inteligente`).
4. Déjalo en **Public** y **NO marques** las casillas de "Add a README file" (ya lo tenemos creado).
5. Pulsa en **"Create repository"**.

### Paso 3: Subir tu código a GitHub
En la carpeta del proyecto (`D:\PDF`), ejecuta los siguientes comandos sustituyendo la URL por la de tu nuevo repositorio:
```bash
git add .
git commit -m "Versión mejorada: posicionamiento exacto, arrastre de texto, creación y reordenación de fotos a PDF"
git branch -M main
git remote add origin https://github.com/isaacbarnuevo/rellenador-pdf-inteligente.git
git push -u origin main
```

### Paso 4: Activar GitHub Pages (Opcional, para usarla online)
1. En tu repositorio de GitHub, ve a **Settings** (Configuración) > **Pages** (en el menú lateral izquierdo).
2. En **Build and deployment** > **Branch**, selecciona `main` y la carpeta `/ (root)`.
3. Pulsa **Save**. En un par de minutos, tendrás tu app disponible en:
   `https://isaacbarnuevo.github.io/rellenador-pdf-inteligente/`
   donde podrás usar la app desde el móvil, tablet o cualquier ordenador sin instalar nada.
