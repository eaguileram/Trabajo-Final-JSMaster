# Tiempo de desarrollo: 4 semanas.
Fecha límite entrega:  25 de Septiembre 2021<br/>
Forma de entrega: Link a repositorio Github con el proyecto, el link debe ser entregado mediante Classroom en la actividad creada para este fin.<br/>


## Descripción general del proyecto<br />

Se debe realizar en modo SPA (Single Page Application) una tienda de comercio electrónico con las siguientes características:<br />
~~Se debe utilizar HTML, CSS y Javascript o Typescript, no se permitirá el uso de frameworks (React, Angular u otro).~~<br />
~~En caso de estar realizado en Typescript no debe incluir los archivos compilados a JS.~~<br />
~~El proyecto solo debe contener 1 archivo html (index.html).~~<br />
~~El usuario debe ser capaz de ver una variedad de productos y añadirlos a un carro de compra.~~<br />
~~El usuario debe poder autenticarse, la validación debe ser estática y se debe aclarar cuál será el usuario y contraseña para uso del ejercicio.~~<br />
~~La posibilidad de iniciar sesión no debe estar disponible si el usuario ha iniciado sesión, y en ese caso debe mostrar el nombre del usuario.~~<br />
~~La cuenta de usuario no debe persistir cuando el usuario sale del sitio (cierra la pestaña o cierra el navegador).~~<br />
~~Cada producto debe tener 1 imagen, 1 título, 1 precio y stock disponible (entre 1 y 5 unidades).~~<br />
~~Cada producto debe indicar si ese producto se encuentra  en el carro de compras y en qué cantidad, permitiendo añadir más del mismo ítem.~~<br />
~~El usuario no debe ser capaz de solicitar una cantidad mayor a la disponible.~~<br />
El stock de productos debe persistir ante la recarga de la página y si el usuario sale del sitio.<br />
~~El carro de compra debe persistir sus datos aún cuando el usuario realice una recarga de la página o si el usuario sale del sitio.~~<br />
~~El carro de compra debe calcular el total de la compra en base al valor de los productos seleccionados, añadir un costo de $1500CLP por envío (US$ 2) y $350CLP (US$0,5) por cada producto.~~<br />
~~El carro de compra debe tener un botón de compra, que solo debe estar habilitado si el usuario ha iniciado sesión.~~<br />
Al realizar la compra, se debe simular una petición asíncrona que se demore 3 segundos en responder.<br />
Se debe notificar al usuario que la compra está siendo realizada, mientras esto sucede, el usuario no debe ser capaz de añadir nuevos productos ni realizar otra compra.<br />
Cuando se realiza la compra, el carro de compra debe ser vaciado y mostrar un mensaje de compra exitosa, pero permitiendo que el usuario sea capaz de volver a realizar una compra.<br />
El descuento de productos del stock general debe realizarse una vez realizada la compra<br />
~~Se debe añadir un botón al pie que permita restaurar los valores por defecto de la cantidad de productos.~~<br /><br />


## Para la evaluación se considerarán las siguientes áreas:<br />

(20 puntos) Limpieza del código, orden y fácil lectura/comprensión. <br />
(10 puntos) Uso de ECMAScript 6 para declaración de variables, métodos de alto nivel, destructuración, entre otros.<br />
(30 puntos) Separación de labores del código, ya sea mediante clases o programación funcional, cada parte del código debe tener una labor específica y única.<br />
(20 puntos) Código a prueba de terceros, se realizará prueba simulando ser otro desarrollador que intentará añadir nuevos productos, modificar valores y cantidades de los ya existentes. El código debe estar preparado para estas labores y evitar que el nuevo desarrollador modifique otras variables que no correspondan, además se deben considerar estás modificaciones para el botón de restauración de las cantidades.<br />
(60 puntos) Cumplimiento del listado de requerimientos.<br />

Máximo puntaje posible a obtener 140 puntos<br />
Nivel de exigencia para aprobación 60%<br />
Puntaje mínimo para aprobación 83 puntos<br />

Se añade vista esquemática del proyecto, esto es solo a modo de recomendación y aclaración.<br /><br/>

![Screenshot](./layout.png)

## TODO
## HTML5 / CSS3

- [x] ~~Documento HTML5~~
  - [x] ~~FONTS~~
  - [x] ~~Estructura GRID~~
    - [x] ~~ARTICLE~~
    - [x] ~~ASIDE~~
- [x] ~~DIV GRID Article~~
  - [x] ~~Productos GRID~~ 
  - [x] ~~Imagen~~
  - [x] ~~Título~~
  - [x] ~~Precio~~
  - [x] ~~Stocḳ~~
  - [x] ~~Botón de compra~~
    - [x] ~~Alerta de añadido al carrito~~
  - [x] ~~Estado pedido~~
- [x] ~~ASIDE~~
  - [x] ~~Crear Caja Login~~
    - [x] ~~Crear usuario logueado~~
    - [X] ~~Crear Login~~
  - [x] ~~Crear Caja Carrito Vacío~~
    - [x] ~~Crear Empy Cart~~
  - [x] Crear Caja Carrito Compra
    - [x] ~~Crear Cart~~
    - [x] ~~Crear detalle compra~~
    - [x] ~~Crear botón eliminar artículo~~
      - [x] ~~Crear botones aumentar, disminuir cantidad~~
    - [x] ~~Crear Botón Comprar~~
    - [x] ~~Crear mensaje compra~~
  - [x] Crear Caja Desarrollo
    - [x] ~~Crear datos desarrollo~~
    - [x] ~~Agregar datos desarrollo~~
    - [x] ~~Crear botón restaurar productos~~

## CSS3
- [x] ~~GRID~~
  - [x] ~~Grid Cajas Aside~~
- [x] ~~COLORES~~
  - [x] ~~Bordes Input~~
  - [x] ~~Bordes Icon~~
  - [x] ~~Eliminar border input selected~~
  - [x] ~~Agregar clase color azul icon input selected~~
  - [x] ~~transición más lenta al desaparecer toast~~
  - [x] ~~aparecer title encima del basurero indicando quitar artículo del carrito~~
- [x] ~~Media Responsive~~

## JS
- [x] Eventos
  - [x] ~~Cambiar color icon user y pass onclick~~
  - [X] ~~setear default color si hace click fuera de los input~~
  - [x] ~~Llenerar usuario y clave al hacer clic en imagen o clave datos desarrollo~~
  - [x] ~~Aparecer alerta si se presiona en cualquier botón Añadir a compra~~
  - [x] ~~Deshabilitar botón de compra después de presionar~~
  - [x] ~~Login~~
    - [x] ~~function login~~
      - [x] ~~si no está logueado, ocultar box nombre~~
      - [x] ~~validar usuario y pass~~
      - [x] ~~si es correcto, ocultar login y mostrar nombre~~
      - [x] ~~persistir sesión de usuario al refrescar la página~~
      - [x] ~~hacer que el botón realizar compra, sólo esté visible si está logueado~~
   - [ ] Articulos
      - [x] ~~Crear JSON de Articulos~~
      - [x] ~~Crear objetos de la clase articulos desde el JSON~~
      - [x] ~~cargar objetos en vista usuario~~
      - [x] ~~funcion para añadir eventos al carrito~~
   - [ ] Carrito
      - [x] ~~Crear objeto carrito~~
      - [x] ~~Crear variable total~~
      - [x] ~~Crear constante total del DOM~~
      - [x] ~~Crear constante restaurar del DOM~~
      - [x] ~~Crear constante localStorage~~
      - [x] ~~Añadir producto seleccionado al carrito~~
      - [x] ~~limitar la cantidad de items agregados al total disponible~~
      - [x] ~~quitar producto del carrito~~
      - [ ] limitar la cantidad de items dinámicamente, usando stock de la DB
      - [ ] mostrar unidades en el carrito en el DOMProductos

