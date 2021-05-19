# Documentación

[La página](#la-pagina) 

[Tema de Wordpress](#tema-de-worpress)

 - [Layout](#layout)
   - [Header](#header)
     [Para editar el Header](#para-editar-el-header)
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

​	*[Header](#header)

​	*[Footer](#footer)

Mistras que el resto del contenido varía entre:

​	*Galería de imágenes que abarca el ancho de la página

​	*Párrafos de texto simple

​	*Formularios de reserva y contacto

​	*Tienda



#### Elementos de diseño de layout



##### Paleta de color

| Tipo             | Código rgb       | Código HEX | Elementos                               |
| ---------------- | ---------------- | ---------- | --------------------------------------- |
| Color Primario   | rgb(240 240 241) | \#f0f0f1   | background-color                        |
| Color Secundario | rgb(88 89 91)    | \#58595b   | h1, h2, h3, h4, h5, h6, p, a *(textos)* |
| Color Auxiliar   | rgb(234 234 234) | \#eaeaea   | input, textarea, buttons                |



##### Fuentes tipográficas

| Nombre             | Link de descarga                                           |
| ------------------ | ---------------------------------------------------------- |
| FreightDispProBook | https://gitlab.com/jungla-dev/teo-casa/-/tree/master/fonts |
| SofiaPro           | https://gitlab.com/jungla-dev/teo-casa/-/tree/master/fonts |



___



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



##### Header en posición inicial 

![Initial Header](https://raw.githubusercontent.com/jungla-dev/teo.casa.documentation/main/Captura%20de%20Pantalla%202021-05-18%20a%20la(s)%2020.27.25.png)



##### Header despues de hacer scroll 

![Header on scroll](https://github.com/jungla-dev/teo.casa.documentation/blob/main/Captura%20de%20Pantalla%202021-05-18%20a%20la(s)%2020.27.34.png?raw=true)



##### Para editar el Header

Para empezar, ten cuidado ;). 

Si no tienes accesos al archivo **.css** que controla los estilos gráficos del  *menú secundario* bajo el nombre **topMenu** evita editar o borrar este elemento.

Puedes agregar links al *menú primario* bajo el nombre **MenuScroll**, siempre y cuando mantengas el carrito de compras al final de la lista para no romper los estilos.



<img src="https://github.com/jungla-dev/teo.casa.documentation/blob/main/menu-control.png?raw=true" alt="menu" style="zoom:50%;" />



#### Contenido

El contenido de cada página es flexible, aunque el color de los textos y la tipografía están determinados por los estilos creados para este tema. 

Al crear una página usando wordpress, se asignarán automáticamente los elementos [Header](#header) y [Footer](#footer).



### Footer



El footer es un elemento que se despliega en la página a partir de un `widget de texto de wordpress`. Destro de este widget, existe un código html muy simple:

```html
<div class="footer-container">
  <ul class="socialMedia">
    <li>
      <a href="https://www.facebook.com/casateomx/" target="_blank" 	 rel="noopener">Facebook</a>
    </li>
    <li>
      <a href="https://www.instagram.com/casateomx/" target="_blank" rel="noopener">Instagram</a>
    </li>
    <li>
      <a href="https://www.airbnb.es/rooms/47470922?preview_for_ml=true&amp;source_impression_id=p3_1610390457_qihtwLhK8g1lCXi8&amp;guests=1&amp;adults=1" rel="noopener">Airbnb</a>
    </li>
  </ul>
    <div class="tiny-logo"><img class="alignnone size-full wp-image-190" src="https://teo.casa/wp-content/uploads/2021/05/CasaTeo_IconoGris-fav-01.png" alt="" width="228" height="228" />
    </div>
   	<div class="direction">
      <div>Francisco Petrarca 254 Col. Polanco 11560,
      Miguel Hidalgo, Ciudad de México</div>
      <div>www.teo.casa</div>
      <div>By Enrique Olvera</div>
      <div>
    </div>
  </div>
</div>
```



Es posible editar este código con el editor de texto que ofrece WordPress, pero es ideal hacerlo a través del código `html` para evitar romper el código.



<img src="https://github.com/jungla-dev/teo.casa.documentation/blob/main/footer-widget.png?raw=true" alt="footer" style="zoom:50%;" />
