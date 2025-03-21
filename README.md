# Guía de Estilos - Portfolio Profesional

## 1. Paleta de Colores

La paleta de colores utilizada en el portfolio se basa en un diseño moderno y minimalista, con un enfoque en la claridad y la legibilidad. Los colores principales son:

- **Negro (#000000):** Utilizado en el encabezado, pie de página y bordes para un aspecto elegante y profesional.
- **Blanco (#FFFFFF):** Usado como color de fondo y texto en contraste con el negro para una lectura clara.
- **Azul (#2196F3):** Aplicado para resaltar elementos clave, como títulos y enlaces, proporcionando un toque de color vibrante.
- **Gris Claro (#F5F5F5):** Utilizado como fondo en secciones secundarias para diferenciarlas visualmente.

## 2. Tipografía

La tipografía seleccionada para el portfolio es **Arial, Helvetica, sans-serif**, una fuente sans-serif moderna y legible en cualquier dispositivo. Se utiliza de la siguiente manera:

- **Títulos (h1, h2, h3):** Fuente en negrita para destacar los encabezados.
  - `h1`: Tamaño 32px (24px en móviles).
  - `h2`: Tamaño 28px (20px en móviles).
  - `h3`: Tamaño 24px (18px en móviles).
- **Texto Normal (p):** Tamaño 16px, con un interlineado adecuado para una lectura cómoda.
- **Botones y Enlaces:** Fuente en negrita para resaltar acciones importantes.

## 3. Logo Personal

El logo personal está compuesto por una imagen (`FAVICON.png`) acompañada del texto **"ÁLVARO ESCUDERO DELGADO"**. El logo se muestra en el encabezado de todas las páginas y tiene las siguientes características:

- **Imagen:** 40px de ancho, con bordes redondeados.
- **Texto:** Fuente en negrita, tamaño 18px (16px en móviles), alineado verticalmente con la imagen.
- **Uso:** Representa la identidad personal y profesional, y se mantiene consistente en todas las secciones del portfolio.

## 4. Librerías Utilizadas

- **Bootstrap 5.3.3:** Utilizado para estilos base y componentes responsivos, como el sistema de grid y utilidades de flexbox.
  - Enlace CDN: [Bootstrap CSS](https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css).
- **Google Fonts (implícito):** Aunque no se utiliza directamente, la tipografía Arial es compatible con Google Fonts y se puede ampliar en el futuro.

## 5. Enlaces a Código Externo

- **GitHub:** Todos los proyectos mostrados en la galería están alojados en GitHub y son accesibles a través de enlaces directos.
  - Ejemplo: [Formulario GitHub](https://alvaroescudero2002.github.io/Formulario_EscuderoDelgadoAlvaro/).
- **LinkedIn:** Enlace al perfil profesional de LinkedIn.
  - [LinkedIn](https://www.linkedin.com/in/%C3%A1lvaro-escudero-delgado-30bb04245/).
- **Instagram:** Enlace al perfil personal de Instagram.
  - [Instagram](https://www.instagram.com/alvaroescudero02/).
- **Google Drive:** Enlace al CV en formato PDF.
  - [Mi CV](https://drive.google.com/file/d/1PDtPyoU8Ytbq6EnG68JMN12XWn7ICY27/view).

## 6. Problemas Técnicos y Soluciones

### **Problema 1: Diseño Responsivo en Dispositivos Móviles**

- **Descripción:** Al implementar el diseño inicial, las imágenes laterales y la galería no se ajustaban correctamente en pantallas pequeñas, lo que generaba un desplazamiento horizontal no deseado.
- **Solución 1:** Se utilizaron media queries para reorganizar el contenido en dispositivos móviles. Las imágenes laterales se ocultaron y la galería se ajustó a dos columnas en pantallas pequeñas.
  ```css
  @media (max-width: 768px) {
    .imagen-lateral {
      display: none;
    }
    .imagenes-habilidades {
      grid-template-columns: repeat(2, 1fr);
    }
  }
