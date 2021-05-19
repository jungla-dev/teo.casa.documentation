# Documentación

[La página](#la-pagina) 

[Tema de Wordpress](#tema-de-worpress)

 - [Layout](#layout)
   - [Header](#header)
   - [Contenido](#contenido) 
   - [Footer](#footer)
- [Páginas](#paginas)
  - [Nosotros](#nostros)
  - [El Espacio](#el-espacio)
  - [Talleres](#talleres)
  - [Reservas](#Reservas)
  - [Tienda](#tienda)
    - [Producto](#producto)
    - [Cart](#cart)
- Plugins
  - [Smart Slider 3](#smart-slider-3)
  - [WP Shopify](#wp-shopify) 
  - [Contact Form 7](#contact-form-7)
  - [TranslatePress - Multilingual](#translatePress-multilingual)



## La Página



La página de Casa Teo, está alojada en el dominio [teo.casa](https://teo.casa).

Está contruida a partir del sistema de wordpress adminsitrado por cpanel.

El diseño fue elabodado por grupoolvera y la contrucción del tema fue elabodado por el estudio jungla.cc.

| Repositio                              | Versión | Última Actualización |
| -------------------------------------- | ------- | -------------------- |
| https://github.com/jungla-dev/teo.casa | 1.3.0   | 18/05/2021           |



## Tema de Wordpress

El sitio teo.casa, está utilizando el tema **teo.casa by jungla** creado específicamente para la página.

Está basado en el tema de wordpress **Twenty Twenty-One** con el objetivo de matener las buenas prácticas del sistema y  poder seguir el esquema de actualiaciones de este tema.



### Layout 



El layout de la página está construido por elementos minimalistas.

Al crear una nueva página dentro de administrador de contenidos (Wordpress), existen dos lementso constantes en el diseño:

​	*[El Header]('#header')

​	*El Footer

Mistras que el resto del contenido varía entre:

​	*Galería de imágenes que abarca el ancho de la página

​	*Párrafos de texto simple

​	*Formularios de reserva y contacto

​	*Tienda

#### Elementos de diseño de layout



##### Paleta de color

| Tipo             | Código rgb | Código HEX | Elementos |
| ---------------- | ---------- | ---------- | --------- |
| Color Primario   | 1.3.0      |            |           |
| Color Secundario |            |            |           |



##### Fuentes tipográficas

| Nombre             | Link de descarga |      | Elementos |
| ------------------ | ---------------- | ---- | --------- |
| FreightDispProBook |                  |      |           |
| SofiaPro           |                  |      |           |

#### Header



El código del header está compuesto por dos partes para lograr una animación fluida.

Parte 1: 

 + **Logo**: creado dentro de *Site Identity*, 
   con la opción  ```Display Site Title & Tagline```  desabilitada :
   - [ ] Display Site Title & Tagline 
 + **Switch de idioma**: creado como un *menú secundario* bajo el nombre **topMenu** en la subsección de menú dentro de la sección de apariencia en WordPress.

Parte 2:

 + Listado de páginas: creadas com un *menú primario* bajo el nombre **MenuScroll** en la subsección de menú dentro de la sección de apariencia en WordPress. 
   `El ultimo elemento de esta lista debe ser el carrito de compras`



Presenta un efecto que se activa al hacer *scroll* al contenido, éste efecto es generado por un archivo de javascript integrado al tema de WordPress, ubicado en la siguiente dirección [teo.casa/assets/js/junglaJs/header.js](https://github.com/jungla-dev/teo.casa/blob/main/assets/js/junglaJs/header.js) *(sólo visible con permisos de acceso)*.

Puedes editar las páginas y los idiomas en el administrador de contenidos (wordpress), sin embargo de no romper algún estilo.


