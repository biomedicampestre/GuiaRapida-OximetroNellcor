Guía de Uso: Página Web para Guía Rápida de Equipo Médico
Esta guía te explicará cómo funciona el código HTML y CSS que conforma la página web de la Guía Rápida de un Oxímetro Nellcor.
--CREACION DEL ARCHIVO HTML y CSS--
-- Abrir visual studio
-- Archivo, abrir nuevo folder.(aquí se puede crear la carpeta o si ya existe se selecciona)
-- Se abre un nuevo FILE, el cual se va a nombrar "index.html"
-- Se abre otro FILE, el cual se llamara "styles.css".
--ARCHIVO HTML (index.html)--
Estructura del Archivo HTML
El código se divide en dos partes:
HTML: Es la estructura del contenido de la página.
CSS: Define los estilos y cómo se ve la página (colores, fuentes, tamaños, etc.).
Archivo HTML (index.html)
El HTML es el esqueleto de la página.
1.-Encabezado (header):
Aquí se encuentra el logo y el título de la página.
Modificar texto: Puedes cambiar el título que aparece en la página dentro de las etiquetas <h1>. 
2.-Secciones de Contenido:
Descripción del Equipo: Una breve explicación del equipo que aparece bajo el título "Descripción del Equipo".
Para cambiar este texto, busca dentro de la sección <p> que sigue al título.
3.-Partes del equipo: Aquí se describen las partes del equipo, como los botones y la pantalla. El texto y las imágenes pueden modificarse buscando el área 
correspondiente y cambiando las etiquetas <li> para el texto o <img> para las imágenes.
Guía de Uso: Una lista de instrucciones de cómo operar el equipo. Puedes editar las instrucciones en las etiquetas <li> bajo esta sección.
Anexo: Fallas Comunes: Contiene imágenes que muestran posibles fallas. Para reemplazar estas imágenes, cambia la ruta dentro de las etiquetas <img>.
4.-Pie de Página (footer): Aquí aparece un mensaje que puedes modificar, como el texto que dice "Departamento de Biomédica | Médica Campestre". 
Este texto está dentro de las etiquetas <p>.
--ARCHIVO CSS (styles.css)--
El archivo CSS controla la apariencia de la página (colores, tamaños, etc.). 

**Colores:
Todos los colores se puede definir al principio del archivo para facilitar la identificación de los colores.
ejemplo 
:root {
    --rosa: #ea787e;
    --gris-oxford: #3a3a3a;
    --azul-: #504F61;
    --fondo-rosado-suave: #ffd3d3;
    --blanco: #e6e7e8;
    --fucsia: #7e0642;
}
**Tamaño del texto: Para cambiar el tamaño del título principal (h1), busca esta parte en el CSS:
header .titulo h1 {
    font-size: 19px;
}
Puedes cambiar el número 19px a un número mayor para hacer el título más grande, o menor para hacerlo más pequeño.
Imágenes:

Si deseas cambiar el tamaño de las imágenes, puedes ajustar el ancho máximo de las imágenes en esta sección del CSS:
css
Copiar código
img {
    max-width: 100%;
    height: auto;
}
Por ejemplo, si quieres que las imágenes ocupen menos espacio, puedes cambiar el max-width a 80%.
Estilo de Cuadros y Bordes:

Los bordes que rodean algunas secciones, como la "Guía Rápida de Operación", tienen un estilo específico. Para cambiar el color o el grosor de estos bordes, busca esta parte en el CSS:
css
Copiar código
.guia-uso {
    border: 7px double beige;
}
Cambia el 7px por un número más pequeño o grande para modificar el grosor del borde, y el color beige por otro nombre de color o código hexadecimal.
*DIV Y CLASS
Un div es un contenedor para agrupar contenido.
Una class es una etiqueta que se usa para aplicar estilos con CSS.
Para identificar un div busca etiquetas <div class="nombre-de-clase">.
Para cambiar su estilo, edita las propiedades en el archivo styles.css usando el nombre de la clase precedido por un punto, como .logo.

