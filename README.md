# Proyecto FInal

Este archivo README.md forma parte del proyecto final con css de dev.f para el segundo modulo, en el que elegi el tema relacionado a la banda de metal Baby metal en donde a mi página le puse "Babymetal".


## Organización de mi página
Mi página la organice de la siguiente manera:

1. Heavy Metal | Metal (Introducción)
2. Subgéneros del metal y bandas representativas
3. ¿Quiénes son Babymetal? (Tema Principal)
4. Por qué algunos metaleros no consideran a Babymetal como metal
5. Integrantes de Babymetal
    - Banda de Apoyo (Kami Band)
    - Integrantes
6. Babymetal y su giro al género
7. Características únicas
8. Discografía destacada
9. Mis 10 canciones favoritas de Babymetal (Datos Extras mios |Video o Iframes)
10. Fotos sacadas por mí de Babymetal  (img)
11. Suscríbete para más información (Formulario)

## Caracteristicas de mi página 

En mi pagina hice uso de diferentes etiquetas como:

- `<h1>` a `<h5>` Para el correcto titulado segun su jerarquia.

- `<ul>` y `<ol>` con sus `<li>` para sus elemento.

- `<nav>` para crear una barra de navegación y dezplazarme por el contenido con un clic en donde para ser mas especifico se utilizo un `<ul>` con `style=""`para darle mejor apariencia visual con los siguientes atributos `list-style: none;` sirve para eliminar los marcadores predeterminados de la lista (•, 1., etc.) `margin: 0;` que sirve para eliminar cualquier margen externo que el navegador aplique por defecto al `<ul>`, `padding: 0;`este se asegura que los elementos `<li>` no tengan espacio adicional, `display: flex;` permite alinear y distribuir los `<li>` de manera más eficiente convirtiendo el contenedor `<ul>` en un contenedor flexible, `justify-content: center ;` Centra los `<li>` dentro de la lista `<ul>` centrando la barra de navegacion y `background-color: #444 ;` sirve para ponerle un color de fondo en la barra en este caso gris oscuro o #444.
Dentro de los `<li>` utilize `style=""`para darle mejor apariencia visual a la lista e hiciera mejor contraste visual mediante los siguiente atributos `margin: 0 15px` en este caso el 0: Define el margen superior e inferior del `<li>` como 0 píxeles (sin espacio) y el 15 px Añade un espacio horizontal (15 píxeles) entre los elementos de la lista `<li>` para separarlos visualmente, `color: white;` Cambia el color del texto del enlace a blanco y `text-decoration: none;` quita el subrayado a los enlaces dandole mejor apariencia visual.

- `<section>` para dividir el contenido y poder enlazarla con la barra de navegación`<nav>` mediante el atributo `id="identificador_seccion"`.

- `<p>` para agregar parrafos y utilice el atributo `<strong>` para poner algunas palabras en negritas y en ciertas partes del documentos como el `<footer>` le agregue como atributo `style=""` en donde utilice `text-align: center;` y `margin-top: 20px;` para ponerle un margen superior de 20 pixeles basicamente para darle un espaciado y centrar el texto.

- `<img>` para insertar imagenes mediante varios atributos `src="link"` para colocar el enlace o la fuente de donde sacara la imagen `width=""` para el ancho de la imagen `height=""` para el alto de la imagen y  `alt="descripcion de imagen"` para describir la imagen. 

- `<table>` para hacer tablas con los atributos `<thead>` para la parte superior de la tabla y `<tbody>` para definir que ira en el cuerpo de la tabla y dentro de los atributos anteriores `<tr>` para representar una fila en la tabla y `<td>` para las celdas dentro de las filas.

- `<a>` para agregar enlaces o links mediante el atributo `href="link"` y asi redirigirnos a otra página o si queremos que habra una nueva pestaña se hace  con `target="_blank"` y listo.

- `<iframe>` para agregar videos de youtube  mediante varios atributos `src="link"` para colocar el enlace o la fuente de donde sacara el video `width=""` para el ancho de la imagen `height=""` para el alto del video y  `title="descripcion de video"` para describir el video, `frameborder="0"` elimina el borde alrededor del iframe (en desuso, usa CSS). `allow="accelerometer;` `autoplay;` `clipboard-write;` `encrypted-media;` `gyroscope;` `picture-in-picture;` `web-share"` habilita permisos como accelerometer (permite usar el acelerómetro en el contenido), autoplay (reproduce video o audio automáticamente), clipboard-write (permite escribir datos en el portapapeles), encrypted-media (usa contenido protegido por DRM), gyroscope (permite el uso del giroscopio), picture-in-picture (habilita el modo de video flotante), y web-share (utiliza la API de Web Share para compartir contenido) y `referrerpolicy="strict-origin-when-cross-origin"` controla qué información de referencia se envía para proteger la privacidad. `allowfullscreen` permite que el video o contenido se vea en pantalla completa.

- `<footer>`para colocar un pie de página y le agregue como atributo `style=""` en donde utilice `text-align: center;` y `margin-top: 20px;` para ponerle un margen superior de 20 pixeles basicamente para darle un espaciado y centrar el texto.
---
### Estilo o Css

Replique el las pantallas que nos dejo el profe con los queries solo que yo agregue algunas cosas mas como el footer y otro elemento para colocar un video, obteniendo el siguiente código o estilo:

```
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap');

html {
    font-size: 16px;
}

body {
    margin: 0; /* Elimina márgenes predeterminados */
    padding-top: 90px; /* Añade espacio para el nav fijo */
    font-style: normal;
    font-family: "DM Sans", serif;
    color: black;
    background: white;
}

h1 {
    font-size: 2.2rem;
    text-align: center;
    font-weight: bold;
}

h3{
    text-align: justify;
    font-size: 1.375rem;
}

h4{
    font-size: 1rem;
    text-align: center;
    font-weight: bold;
}

p {
    margin-top: 10px;
    margin-bottom: 10px;
    font-size: 1em;
    text-align: center;
    
}

.text-color-white {
    color: white;
}

.text-color-black {
    color: #122130;
}

.nav{
    justify-content: space-between;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background: rgba(8, 7, 6,0.94); /* Fondo sólido oscuro */
    padding: 10px;
}

.wrapper-top{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 20px;
}

.wrapper-top-left img {
    margin-top: 10px ;
    max-width: 120px; /* Ajusta el ancho máximo de la imagen */
    max-height: auto; /* Ajusta la altura máxima de la imagen */
    
}

.wrapper-top-right{
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 30px; /* Espaciado entre íconos */
    display: none;
    margin-right: 40px;
}

.wrapper-top-right ul li {
   list-style: none;/* Elimina las viñetas de la lista */
   font-size: 1rem; /* Ajusta el tamaño de la fuente */
   cursor: pointer; /* Cambia el cursor al pasar el mouse */
   text-align: center; /* Alinea el texto a la derecha */
   align-items: center;
}
.wrapper-top-right a{
    text-decoration: none; /* Elimina el subrayado */
    color: #FFFFFF; /* Texto blanco */
    font-weight: 600;
    font-size: 1rem;
    transition: color 0.3s ease;
}

.wrapper-top-right a:hover {
    color: red; /* Amarillo dorado al pasar el mouse */
}

.wrapper-main {
    margin: 30px;
    display: flex;
    flex-direction: column; /* por  defecto */
    justify-content: center; /* Centra horizontalmente */
    align-items: center;
    gap: 20px;
}

.wrapper-column-left {
    display: flex;
    flex-direction: column; /* Apila los elementos verticalmente */
    justify-content: center; /* Centra horizontalmente */
    align-items: center;
    gap: 5px;
}

.wrapper-column-right {
    display: flex;
    flex-direction: column; /* Apila imagen y text-3 */
    justify-content: center; /* Centra horizontalmente */
    align-items: center;
    gap: 5px;
}

.wrapper-text-1{
    background: white;
    border-radius: 20px;
   
    /* padding-left: 10px;
    padding-right: 10px; */
}
 
.wrapper-text-2{
    background: #5F4BF9;
    border-radius: 20px;
    padding-left: 25px;
    padding-right: 25px; 
    display: none;
}


.responsive-iframe {
    display: flex;
    position: relative; /* Establece un contenedor relativo */
    width: 100%; /* Ocupa todo el ancho disponible */
    padding-bottom: 56.25%; /* Mantiene la proporción 16:9 */
    height: 0; /* Altura inicial en 0 */
    overflow: hidden; /* Oculta el contenido desbordado */
}

.responsive-iframe iframe {
    position: absolute; /* Posiciona el iframe dentro del contenedor */
    border-radius: 20px;
    width: 100%; /* Ajusta el ancho al contenedor */
    height: 100%; /* Ajusta la altura al contenedor */
}

.wrapper-image {
    display: flex; /* Activa el modelo de caja flexible */
    justify-content: center; /* Centra horizontalmente */
    align-items: center; /* Centra verticalmente */
    width: 100%; /* La imagen ocupa el 100% del ancho disponible */
    height: auto; /* La altura se ajustará automáticamente */
    
}

.wrapper-image img {
    margin-top: 42px;
    width: 100%; /* La imagen se ajusta al ancho del contenedor */
    height: auto; /* Mantiene la proporción de la imagen */
    max-height: 50vh; /* Opcional: límite máximo de altura */
    border-radius: 20px; /* Esquinas redondeadas */
    object-fit: cover; /* Asegura que la imagen cubra el espacio disponible sin distorsión */
}

.wrapper-text-3{
    width: 100%;
    background: rgba(151, 148, 148,20%);
    padding: 20px;
    border-radius: 20px;
    text-align: justify;
    box-sizing: border-box;
    text-align: justify;
    justify-content: center; /* Centra horizontalmente */
    align-items: center;

}

.button {
    background: black;
    border-radius: 5px;
    padding: 5px 5px 5px 5px;
    display: inline-flex;
    align-items: center;
    text-decoration: none;
}

.wrapper-button-svg{
    padding: 5px;
    border-radius: 5px;
    margin-left: 10px;
    background: #DFDBFD;
    display: flex;
    align-items: center;
    justify-content: center;
}

.button-text{
    margin-left: 5px;
}

.button-svg{
    width: 20px;
    height: auto;
}

.container {
    width: 90%;
    margin: auto;
}

.wrapper-bottom{
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.wrapper-bottom-left h5 {
    font-weight: 500;
    font-size: 12px;
    color: #666; /* Texto gris */
    text-decoration: none;
}

.wrapper-bottom-right{
    display: flex;
    align-items: center;
    gap: 20px; /* Espaciado entre íconos */
}

.social-icons {
    display: flex;
    gap: 4px; /* Espaciado entre íconos */
}

.social-icons a img{
    width: 36px;
    height: 36px;
}



@media screen and (min-width: 0px){
    .responsive-iframe {
        display: none;
    }
   
}

@media screen and (min-width: 480px){
    .responsive-iframe {
        display: block;
    }
    
}

@media screen and (min-width: 768px){

    .wrapper-top{
        display: flex;
        justify-content: space-between;
    }

    .wrapper-top-right {
        display: flex; /* Activa Flexbox */
        align-items: center; /* Alinea las columnas al final (opcional) */
        gap: 5px; /* Agrega espacio entre los elementos */
    }
    .wrapper-top-right ul {
        display: flex;
        gap: 15px; /* Espaciado reducido en pantallas pequeñas */
    }

    .wrapper-top-left img {
        width: 150px; /* Reduce el logo en pantallas pequeñas */
    }

    .wrapper-top-right a {
        text-decoration: none;
        color: #FFFFFF;
        font-weight: 600;
        font-size: 1rem;
        transition: color 0.3s ease;
    }
    
    .wrapper-top-right a:hover {
        color: #F5A623;
    }

   
    .wrapper-main {
        display: flex; /* Activa Flexbox */
        flex-direction: row;
        justify-content: space-around; /* Espacio entre columnas izquierda y derecha */
        align-items: flex-start; /* Alinea los elementos verticalmente al inicio */
        gap: 20px; /* Espaciado uniforme entre elementos */
        padding: 20px;
    }

    /* Contenedor para la columna izquierda (text-1 y text-2) */
    .wrapper-column-left {
        display: flex;
        flex-direction: column; /* Apila los elementos verticalmente */
        gap: 24px; /* Espaciado entre text-1 y text-2 */
        flex: 1; /* Ocupa un ancho proporcional */
        max-width: 50%; /* Limita el ancho máximo de la columna izquierda */ 
        align-items: center; /* Centra los elementos horizontalmente */
    }

    
    .responsive-iframe iframe {
        display: block;
        width: 100%;
        height: 50%; 
    }

    .wrapper-column-right {
        display: flex;
        flex-direction: column; /* Apila imagen y text-3 */
        gap: 24px; /* Espaciado entre imagen y text-3 */
        flex: 1; /* Ocupa un ancho proporcional */
        max-width: 50%; /* Limita el ancho máximo de la columna derecha */
        align-items: center; /* Centra los elementos horizontalmente */
    }

    .wrapper-text-1{
        display: block;
    }

    .wrapper-text-2 {
        display: block;
        
    }


} 
```



--- 
## Comandos de Git que utilice para el Proyecto Final Segundo Modulo
Primero que nada antes de pasar con los comandos que utlice, cree una carpeta con el nombre `ProyectoFinal` usando la estructura de texto Kamelcase, posteriormente esa carpeta la abri desde `VS code`, una vez abierta la carpeta cree mi archivo `index.html` y guarde los cambios, abri la terminal desde `VS code` para inicializar git y asi poder llevar un control de versiones adecuado en donde utilice el siguiente comando :

### `git init`
Este comando lo utilice para inicializar un nuevo repositorio de Git en mi proyecto. Git crea un subdirectorio oculto `.git` en tu proyecto que contiene toda la información necesaria para el control de versiones.

**Uso:**
```bash
git init
```
**Posteriormente**
### `git add`
Este comando lo utilice para agregar los cambios realizados en mis archivos. Esto incluye nuevos archivos, cambios realizados o archivos eliminados, para que puedan ser incluidos en el siguiente commit.

**Uso:**
Para agregar un solo archivo:
```bash
git add index.html 
git add style.css 
git add readme.md
```
Para agregar todos los archivos:
```bash
git add .
```
En mi caso se me hace más comodo utilizae `git add .` así que utilice ese.

**Despues**
### `git commit -m "descripción del commit"`
Este comando guarda los cambios y la opción `-m` nos permite añadir un mensaje descriptivo que explique los cambios realizados.

**En mi caso el primer commit le puse así:**
```bash
git commit -m "Creacion del archivo index.html"
```
---
Continuando con el proceso, ahora lo que hice fue ir a mi github y crear un repositorio online le puse como nombre `ProyectoFinal` una vez creado copie el enlace que me genero GitHub en mi caso `https://github.com/Raccoon0G/PreyectoFinal.git` una vez obtenido el link dle repositorio en github me dispuse a colocar el siguiente comando en la terminal de `Vs Code` :

### `git remote -v`
Este comando se utiliza para mostrar las URL de los repositorios remotos si es que existen para el repositorio local. Lo utilice más que nada para comprobar que no halla ningun repositorio en linea guardado.

**Uso :**
```bash
git remote -v
```
**Posteriormente :**

Una vez que comprobre que no habia nada en la variable `origin` me dispuse a guardar en esa variable el link del reposistorio online que obtuvimos hace un momento `https://github.com/Raccoon0G/PreyectoFinal.git` con el siguiente comando :

### `git remote add origin "link de repositorio"`
Este comando se utiliza para añadir un nuevo repositorio remoto y vincularlo al repositorio local. Es esencial para poder usar comandos como `git push` o `git pull` con ese repositorio remoto.

**En mi caso lo use así:**
```bash
git remote add origin "https://github.com/Raccoon0G/Nav-Footer-responsive-design.git"
```
 
 Y volvi a comprobar que se haya guardado correctamente con  `git remote -v` y me salio esto:

 ```
origin  https://github.com/Raccoon0G/Nav-Footer-responsive-design.git (fetch)
origin  https://github.com/Raccoon0G/Nav-Footer-responsive-design.git (push)
 ```
 Una vez que me salio lo anterior supe que mi directorio local ya estaba vinculado con el directorio remoto de GitHub.

 Ahora faltaba enviarle la informacion a mi repositorio de GitHub por lo que utilice el siguiente comando para comprobar el nombre de la rama principal ya sea `main` o `master` en mi caso fue `main` asi qe utilice el siguiente comando :

 ### `git push`
Este comando se utiliza para enviar los commits realizados en el repositorio local al repositorio remoto, permitiendo sincronizar los cambios con otros colaboradores.

**Uso:**
```bash
git push origen rama
```
En mi caso utilice el siguiente comando :
```bash
git push origin main
```
En donde la terminal me arrojo o me desplego la siguiente información comprobando que se realizo el push correctamente:

```
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 471 bytes | 471.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Raccoon0G/Nav-Footer-responsive-design.git
   ca5ac47..dbd378b  main -> main

```
Con esto fue la manera en que conecte correctamente mi repositorio local con el remoto, tambien comprobe que estuviera conectado y le envie la informacion para poder hacer el paso de `GitHub Pages`.

## Desplegar mi página en GitHub Pages

Una vez hecho lo anterior, desde inicializar `git` hasta hacer el `git push origin main`, me fui a mi repositorio de `GitHub` con el siguiente link `https://github.com/Raccoon0G/Nav-Footer-responsive-design` para desplegar mi proyecto en donde hice los siguiente pasos :

1. Le di click en `settings` o ajustes.
2. Una vez en settings le di clic en la sección `Pages`.
3. Una vez en GitHub `Pages` me diriji a `Branch` en donde seleccione mi rama en mi caso `main` y le di en `Save` o guardar.
4. Ahora solo espere un momento hasta que me dio el enlace de la página que acababa de desplegar en mi caso `https://raccoon0g.github.io/Nav-Footer-responsive-design/`.
5. Una vez que me dio el link solo quedaba comprobar que mi página estuviera en linea cosa que sucedio,por lo que aquí acaba la explicación para desplegar la página.

---
### Enlace a mi Repositorio
GitHub: [Raccon0G](https://github.com/Raccoon0G/)

Enlace al repositorio de este trabajo : https://github.com/Raccoon0G/Nav-Footer-responsive-design

Enlace a la página (GitHub Pages) de este trabajo : https://raccoon0g.github.io/Nav-Footer-responsive-design/