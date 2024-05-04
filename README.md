## RETO N° 3 100 DAYS OF PROYECTS 

### 02-Product-Info

<img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1714098990726/cc531dd1-4cda-4b85-8151-ed007aa05534.png?auto=compress,format&format=webp" alt="Texto alternativo" width="400"/>

### Tecnologias
[![HTML](https://img.shields.io/badge/HTML5-orange?style=flat&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![CSS](https://img.shields.io/badge/CSS3-blue?style=flat&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)

### Ver demo

[Demo](https://lohanao.github.io/03-Product-Info/)

## Desafio
### Los usuarios deberían poder:

Ver el diseño óptimo en pantallas grandes(1200px).

Ver un color diferente(hover) al pasar el mouse sobre el botón principal.

Ver un color diferente(hover) al pasar el mouse sobre los botones secundarios.

Ver un color de sombra(box-shadow) como se muestra en la imagen.

### Importante:

Agrega icono favicon al proyecto.

Agrega una URL fácil de recordar (ej. 03-product-info).

Agrega un título al proyecto (ej. Product Info - Frontend Club).

Bonus: Agrega un archivo readme.md al proyecto.

## Solución
### Resolución con HTML y CSS
En este proyecto, utilicé HTML y CSS para crear una tarjeta de producto que muestra información relevante sobre un producto, como su nombre, precio, descripción y opciones de interacción.

### Estructura HTML
El contenido de la tarjeta de producto se estructuró utilizando elementos HTML semánticos para mejorar la accesibilidad y el SEO del sitio web. A continuación se muestra una vista general de la estructura HTML utilizada:

```html

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tarjeta de Producto</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
   <div class="container">
      <div class="card">
        <div class="card-image">
          <img src="./img/image.png" alt="" />
        </div>
        <div class="card-body">
          <div class="subtitle">
            <p>Free shipping</p>
          </div>
          <h3>Razer Kraken Kitty Edt Gaming <br /> Headset Quartz</h3>
          <div>
            <p class="price">1599,-</p>
            <p class="old-price">799,-</p>
            <span class="description">The offer is valid until April 3 or as long as stock lasts!</span
            >
          </div>
          <div class="btn-container">
          <button class="btn-cart">Add to cart</button>
          </div>
          <div class="stock-container">
            <div class="ellipse"></div>
            <p class="stock">50+ pcs. in stock.</p>
          </div>
          <div class="buttons">
            <button class="btn-toCart">
              <svg
                width="32"
                height="32"
                viewBox="0 0 32 32"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g clip-path="url(#clip0_6_42)">
                  <path
                    d="M9.33333 26.6667H22.6667"
                    stroke="#191847"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M8 7.99999L16 6.66666L24 7.99999"
                    stroke="#191847"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M16 4V26.6667"
                    stroke="#191847"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M12 16L8 8L4 16C4 17.0609 4.42143 18.0783 5.17157 18.8284C5.92172 19.5786 6.93913 20 8 20C9.06087 20 10.0783 19.5786 10.8284 18.8284C11.5786 18.0783 12 17.0609 12 16Z"
                    stroke="#191847"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M28 16L24 8L20 16C20 17.0609 20.4214 18.0783 21.1716 18.8284C21.9217 19.5786 22.9391 20 24 20C25.0609 20 26.0783 19.5786 26.8284 18.8284C27.5786 18.0783 28 17.0609 28 16Z"
                    stroke="#191847"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </g>
                <defs>
                  <clipPath id="clip0_6_42">
                    <rect width="32" height="32" fill="white" />
                  </clipPath>
                </defs>
              </svg>
              Add to cart
            </button>
            <button class="btn-toCart">
              <svg
                width="32"
                height="32"
                viewBox="0 0 32 32"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g clip-path="url(#clip0_6_59)">
                  <path
                    d="M26 18.096L16 28L6 18.096C5.34041 17.4542 4.82086 16.6827 4.47406 15.8302C4.12727 14.9777 3.96075 14.0626 3.98498 13.1426C4.00922 12.2226 4.22368 11.3175 4.61488 10.4845C5.00607 9.65139 5.56551 8.90834 6.25798 8.30211C6.95045 7.69588 7.76094 7.23959 8.63842 6.96198C9.51589 6.68437 10.4413 6.59145 11.3565 6.68907C12.2716 6.78669 13.1567 7.07274 13.9558 7.52921C14.755 7.98568 15.451 8.60267 16 9.34133C16.5514 8.60803 17.2482 7.99643 18.0468 7.54481C18.8454 7.09319 19.7287 6.81127 20.6412 6.7167C21.5538 6.62212 22.4761 6.71693 23.3504 6.99519C24.2246 7.27345 25.032 7.72917 25.7221 8.33382C26.4121 8.93847 26.9699 9.67905 27.3606 10.5092C27.7512 11.3393 27.9663 12.2412 27.9924 13.1583C28.0185 14.0754 27.855 14.988 27.5122 15.839C27.1693 16.69 26.6545 17.4611 26 18.104"
                    stroke="#191847"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </g>
                <defs>
                  <clipPath id="clip0_6_59">
                    <rect width="32" height="32" fill="white" />
                  </clipPath>
                </defs>
              </svg>
              Add to wishlist
            </button>
          </div>
        </div>
      </div>
    </div>
</body>
</html>



Para lograr el diseño deseado de la tarjeta de producto, sigue estos pasos:

Definir estilos básicos para el contenedor y la tarjeta:
El contenedor debe tener un estilo para centrar su contenido verticalmente y horizontalmente. Puedes lograr esto usando display: flex, justify-content: center y align-items: center.
La tarjeta debe tener un fondo blanco y algún relleno para separar su contenido del borde. Puedes aplicar esto usando background-color: white y padding.
Estilizar la imagen del producto:
La imagen debe ocupar todo el espacio disponible en la tarjeta. Puedes lograr esto usando width: 100% y height: 100% junto con object-fit: cover para mantener la proporción de la imagen.
Agregar efectos de sombra a la tarjeta:
Puedes agregar una sombra suave a la tarjeta para hacerla destacar del fondo. Esto se puede lograr utilizando la propiedad box-shadow.
Estilizar los otros elementos de la tarjeta según sea necesario:
Define estilos para el título, precio, descripción, botón de "Agregar al carrito", etc., según el diseño específico que desees lograr. Ajusta los tamaños de fuente, márgenes, colores, etc., según sea necesario.





