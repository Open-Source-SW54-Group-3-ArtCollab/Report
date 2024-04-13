# Capítulo IV: Product Design
<hr>

## 4.1. Style Guidelines.
<hr>

### 4.1.1. General Style Guidelines.
### Historia de la marca
### Misión
Facilitar un espacio inclusivo y colaborativo que empodere a escritores e ilustradores para compartir sus historias con el mundo, ofreciendo herramientas innovadoras que permitan la creación, distribución y monetización de contenido literario y artístico, al tiempo que se enriquece la experiencia de lectura para una comunidad global de entusiastas de los libros.

### Visión
Ser la plataforma líder y referente en la publicación digital de libros ilustrados, reconocida por su compromiso con la sostenibilidad y el éxito de los creadores, y por ofrecer una experiencia de lectura excepcional que inspire, eduque y entretenga a lectores de todas las edades y culturas.

### Brand Name
El nombre del producto es ArtCollab, el cual cuenta con un logo representado por el icono de un bolígrafo con motivos coloridos a su alrededor haciendo referencia tanto a los escritores como artistas que son parte de los usuarios principales de nuestro aplicativo.
<div style="text-align: center;">
                <img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/logo-artcollab.jpeg?raw=true" alt="ArtCollab" style="max-width: 400px; width: 25%;">
</div>

### Colores
Decidimos elegir la siguiente gama de colores, ya que va acorde al logo y se encuentran relacionados con la temática de nuestra app.
<div style="text-align: center;">
                <img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/Style-Guidelines/Paleta-de-colores.png?raw=true" alt="Color Palette">
</div>

### Tipografía
Elegimos esta fuente porque es legible dentro de todo tipo de entornos, además de no ser una tan frecuentemente usada, por lo que nos genera una mayor diferencia frente a nuestra competencia.
<div style="text-align: center;">
                <img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/Style-Guidelines/Tipografia-1.png?raw=true" alt="Tipografía 1">
</div>

<div style="text-align: center;">
                <img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/Style-Guidelines/Tipografia-2.png?raw=true" alt="Tipografía 2">
</div>

### Espaciado
Siguiendo las recomendaciones de especialistas en diseño de interfaces, se aconseja que el interlineado de los párrafos sea 1.5 veces el tamaño del texto, lo que facilita la lectura al crear una separación adecuada entre las líneas.

Tamaño de letra: 16px

Interlineado: 24px

### Tono de comunicación y lenguaje aplicado
Usaremos un tono divertido, casual, respetuoso y entusiasta, puesto que consideramos que sería adecuado para nuestro tipo de aplicación. Este tono reflejaría la creatividad y el aspecto lúdico de los libros ilustrados, mientras que al mismo tiempo mantendría un nivel de respeto hacia los creadores y la audiencia.

### 4.1.2. Web Style Guidelines.
## 4.2. Information Architecture.
En esta seccción, se va presentarla estructura del software según cada segemento objetivo. Ademas, los elementos que emplearan para la navegacion de esta.
<hr>

### 4.2.1. Organization System.

El Sistema de Organización planteado tiene como objetivo facilitar la
interacción entre el usuario y la aplicación web y garantizar todos los
servicios que ofrece ArtCollab. Respecto a la organización visual del
contenido será de forma jerárquica (visual hierarchy) la landing page
para destacar elementos claves como el publicar o Iniciar sesión.

Además, se utilizarán organización secuencial (step-by-step to
accomplish) en procesos como el registro del usuario y configuración del
perfil.

En cuanto la organización matricial se aplicará filtros de búsqueda
respecto a los géneros literarios o autor.

También se usará esquemas de categorización por ejemplo la búsqueda de
libros o autores donde los usuarios podrán ordenarlo de manera
alfabética. La categorización de audiencias se va a dividir en tres por
los roles del usuario como lector, escritor o ilustrador.
### 4.2.2. Labeling System.

En ArtCollab, el sistema de etiquetas será diseñado para que los usuarios encuentren fácilmente la información que buscan, haciéndolo muy intuitivo y accesible.

### Etiquetas:

Home: Boton invisible que te redirige a la pagina principal en el logo

Populares: Se muestran los libros que están en trending

Suscripciones/Premium: Son una suscripción mensual donde te brindan
diferentes beneficios según tu tipo de usuario

Monetizacion: Únicamente para los Escritores cumpliendo requisitos
previos

Artista: Muestra los mejores artistas del momento en toda la plataforma 

<br>

Además, una vez creada una cuenta y de haber iniciado sesión:

Publicar: Sección disponible luego de iniciar sesión que brinda información de cómo publicar un libro nuevo

### 4.2.3. SEO Tags and Meta Tags.

En esta sección, se describen las etiquetas SEO y Meta que se utilizarán para identificar y posicionar el sitio web y landing page de ArtCollab de manera única en internet. Estas etiquetas son fundamentales para que el sitio sea fácilmente encontrado por los usuarios a través de los motores de búsqueda como Google, Bing y otros. Al optimizar estas etiquetas, se aumenta la visibilidad del sitio y se mejora su posicionamiento en los resultados de búsqueda, lo que puede atraer más visitantes interesados en nuestro aplicativo.

### Para la landing page.

\<meta charset="UTF-8"\>

\<meta name="viewport" content="width=device-width, initial-scale=1.0"\>

\<link href="./src/css/styles.css" rel="stylesheet"\>

\<title\>ArtCollab - ImaginaTales Oficial Landing Page\</title\>

\<meta name="description" content="ArtCollab Landing Page where you can
find a presentation of all the main features of our app."\>

\<meta name="keywords" content="illustrated books, creative
collaboration, writers, illustrators, digital platform"\>

\<meta name="author" content="ImaginaTales"\>

### Para la aplicación web:

\<meta charset="UTF-8"\>

\<meta name="viewport" content="width=device-width, initial-scale=1.0"\>

\<link href="./src/css/styles.css" rel="stylesheet"\>

\<title\>ArtCollab - Illustrated book platform for writers and illustrators\</title\>

\<meta name="description" content="Discover and collaborate on creative projects with talented writers and illustrators on ArtCollab. Explore a vast collection of digital picture books and share your own works."\>

\<meta name="keywords" content="illustrated books, creative
collaboration, writers, illustrators, digital platform, visual narrative, online publising"\>

\<meta name="author" content="ImaginaTales"\>

### 4.2.4. Searching Systems.

El Sistema de navegación de ArtCollab nos ayudara a ver las preferencias
del usuario. La búsqueda digitada le va a redireccionar al libro o autor
escrito del que esté interesado.

Luego de la búsqueda se va a poder filtrar como el usuario lo desee ya
sea por genero literario o autores. Además, de poder ordenar los
resultados de manera alfabética.

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/Search.png?raw=true" alt="Search System" style="margin-bottom: 5px;" width="500"/>

### 4.2.5. Navigation Systems.
En el caso de la navegación en la aplicación web será de una manera
sencilla y minimalista debido a que tiene diversas opciones de interés
para el usuario.
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/Navigation.png?raw=true" alt="Search System" style="margin-bottom: 5px;" width="1000"/>
Tampoco nos olvidamos del lado Mobile en este caso tienes un menú
desplegable donde tienes diversas opciones a elegir para volver a la
página principal basta con apretar en el logo de ArtCollab
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/NavigationMobile.png?raw=true" alt="Search System" style="margin-bottom: 5px;" width="800"/>

## 4.3. Landing Page UI Design.
<hr>

### 4.3.1. Landing Page Wireframe.
Enlace a los Wireframes de la Landing Page en Figma: https://www.figma.com/file/P2GY9CsLT82DzIiZEnxhm6/Mockup-Landing-Page-(Vista)?type=design&node-id=2030-156&mode=design

Versión Desktop:

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Wireframes/Hero.png?raw=true" alt="Landing Page Hero Wireframe">
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Wireframes/DESCUBRE.png?raw=true" alt="Landing Page DESCUBRE Wireframe">
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Wireframes/COLABORA.png?raw=true" alt="Landing Page COLABORA Wireframe">
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Wireframes/Footer.png?raw=true" alt="Landing Page Footer Wireframe">

Versión Mobile:

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/267972bfe26e82cf41c7bca2350823b0e2c310ff/assets/images/landing-page/Wireframes/Hero-Mobile.png?raw=true" alt="Landing Page Mobile Hero Wireframe">
<br>
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/267972bfe26e82cf41c7bca2350823b0e2c310ff/assets/images/landing-page/Wireframes/DESCUBRE-Mobile.png?raw=true" alt="Landing Page Mobile DESCUBRE Wireframe">
<br>
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/267972bfe26e82cf41c7bca2350823b0e2c310ff/assets/images/landing-page/Wireframes/COLABORA-Mobile.png?raw=true" alt="Landing Page Mobile COLABORA Wireframe">
<br>
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/267972bfe26e82cf41c7bca2350823b0e2c310ff/assets/images/landing-page/Wireframes/Footer-Mobile.png?raw=true" alt="Landing Page Mobile Footer Wireframe">

### 4.3.2. Landing Page Mockup.
Enlace a la mockup de la Landing Page en Figma: https://www.figma.com/file/P2GY9CsLT82DzIiZEnxhm6/Mockup-Landing-Page-(Vista)?type=design&node-id=0%3A1&mode=design&t=aMu3gnaeqnM4xQgo-1

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/7aea00ae377ffed000f1efd7462952f131256f83/assets/images/Hero.png?raw=true" alt="Landing Page Desktop Hero">
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/7aea00ae377ffed000f1efd7462952f131256f83/assets/images/DESCUBRE.png?raw=true" alt="Landing Page Desktop DESCUBRE">
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/7aea00ae377ffed000f1efd7462952f131256f83/assets/images/COLABORA.png?raw=true" alt="Landing Page Desktop COLABORA">
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/7aea00ae377ffed000f1efd7462952f131256f83/assets/images/Footer.png?raw=true" alt="Landing Page Desktop Footer">

Versión Mobile:

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Mockup/Hero-Mobile.png?raw=true" alt="Landing Page Mobile Hero">
<br>
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Mockup/DESCUBRE-Mobile.png?raw=true" alt="Landing Page Mobile DESCUBRE">
<br>
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Mockup/COLABORA-Mobile.png?raw=true" alt="Landing Page Mobile COLABORA">
<br>
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/f772ecd60eb11fc1133cb643a10c784ecb3272aa/assets/images/landing-page/Mockup/Footer-Mobile.png?raw=true" alt="Landing Page Mobile Footer">


## 4.4. Web Applications UX/UI Design
### 4.4.1. Web Applications Wireframes
### 4.4.2. Web Applications Wireflow Diagrams

Enlace a traves de la herramienta LucidChart: https://lucid.app/lucidchart/1f8c4e0b-8101-4166-9a44-dca738736ddd/edit?viewport_loc=2076%2C-7%2C1953%2C988%2C0_0&invitationId=inv_7fd31580-59fc-4cd2-bee3-fc3d15fcfde4

<h4> <strong> User goal, usuario inicia sesion, se registra y recupera su contraseña </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/InicioSesion.png" />

<h4> <strong> Descripcion: </strong> </h4>

Al iniciar la aplicación, el usuario se encuentra en la página de opciones, donde puede iniciar sesión mediante correo electrónico o las plataformas de Google y Facebook.
El usuario también puede registrar una nueva cuenta utilizando su correo electrónico o las plataformas mencionadas anteriormente. En caso de olvidar su contraseña, el usuario tiene la opción de recuperarla utilizando su correo electrónico.


<h4> <strong> User goal, usuario edita el contenido de una historia, como el contenido y las series. </strong> </h4>

<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/EditarLibro.png" />

<h4> <strong> Descripcion: </strong> </h4>
 Cuando el usuario visualiza sus historias en su portafolio personal, puede editarlas. Al hacer clic en "editar", puede modificar el contenido de las historias, incluyendo el texto, las imágenes y otros elementos. Las historias se organizan en series. El usuario puede editar las series de una historia, añadiendo, eliminando o modificando las existentes. Una vez realizados los cambios, el usuario puede guardarlos y se actualizarán en su portafolio personal.


<h4> <strong> User goal, usuario publica una nueva historia y agrega series a la historia </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/PublicarLibro.png"/>

<h4> <strong> Descripcion: </strong> </h4>
El usuario puede crear una nueva historia desde su portafolio personal.Al crear una nueva historia, el usuario debe proporcionar los detalles correspondientes, como el título, la descripción, el género, etc.Una vez que la historia tenga los detalles básicos, el usuario puede agregar series a la misma. Cada serie representa una parte o capítulo de la historia. El usuario puede editar las series de la historia, añadiendo, eliminando o modificando las existentes. Una vez que la historia esté completa, el usuario puede publicarla para que otros usuarios puedan verla y leerla.

<h4> <strong> User goal, usuario busca artistas, contacta con ellos e inicia una sala de chats  </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/IniciarSala.png" />
<h4> <strong> Descripcion: </strong> </h4>

La plataforma ofrece una función de recomendación de artistas segun los intereses del usuario. Una vez que el usuario encuentra un artista que le interesa, puede contactarlo directamente desde la plataforma. Al establecer contacto con un artista, se crea una sala de chats privada donde ambos usuarios pueden comunicarse.

<h4> <strong> User goal, usuario del tipo ilustrador edita su perfil  </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/EditarPerfilArtista.png"/>
<h4> <strong> Descripcion: </strong> </h4>

Al iniciar sesion y encontrase dentro de la pantalla principal, el usuario del tipo ilustrador visualiza la opción de editar perfil. Al darle click puede editar su perfil profesional, posteriormente al guardar los cambios estos se actualizan en su perfil.



<h4> <strong> User goal, usuario del tipo escritor edita su perfil  </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/EditarPerfilEscritor.png"/>

<h4> <strong> Descripcion: </strong> </h4>
Los usuarios del tipo escritor también pueden editar su perfil profesional desde la pantalla principal de la aplicación.Al editar su perfil, el usuario puede modificar su información profesional, como su nombre, biografía, portafolio, etc. Una vez realizados los cambios, el usuario puede guardarlos y se actualizarán en su perfil.


<h4> <strong> User goal, usuario busca un libro segun su popularidad y género  </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/BuscarLibros.png"/>

<h4> <strong> Descripcion: </strong> </h4>
 Al iniciar la aplicación, el usuario se encuentra en la pantalla principal. La pantalla principal muestra una selección de los libros más populares de la plataforma. El usuario puede utilizar filtros de búsqueda para encontrar libros según su género de preferencia. La plataforma muestra una lista de resultados de búsqueda que coinciden con los criterios del usuario.

<h4> <strong> User goal: usuario edita el perfil de cuenta </strong>  </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/EditarCuenta.png"/>
<h4> <strong> Descripcion: </strong> </h4>
El usuario puede editar su perfil de cuenta desde la pantalla principal de la aplicación. Al editar su perfil de cuenta, el usuario puede modificar su información personal, como su nombre, correo electrónico, contraseña, etc. Una vez realizados los cambios, el usuario puede guardarlos y se actualizarán en su cuenta.

<h4> <strong> User goal, usuario visualiza las comisiones obtenidas por cada historia </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/IngresosObtenidos.png"/>
<h4> <strong> Descripcion: </strong> </h4>
Al encontrarse dentro de su portafolio personal el usuario visualiza sus obras publicadas, al seleccionar la opción
de editar la historia visualiza los detalles de su historia, posteriormente visualiza tres opciones, editar detalles de la historia, editar tabla de contenido y visualizar los ingresos obtenidos. Al seleccionar la opción de ver ingresos obtenidos, donde puede visualizar los ingresos obtenidos por una historia en particular.


<h4> <strong> User goal: usuario visualiza los planes de suscripción </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/Suscripcion.png"/>
<h4> <strong> Descripcion: </strong> </h4>
Al iniciar sesion se encuentra dentro de la pantalla principal, el usuario visualiza la opción de ver planes de suscripción, luego selecciona la opción mencionada previamente y visualiza todos los planes disponibles.



<h4> <strong> User goal: usuario visualiza el sistema de monetización </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/wireflow-diagrams/Monetizacion.png"/>
<h4> <strong> Descripcion: </strong> </h4>
Al iniciar sesion se encuentra dentro de la pantalla principal, el usuario visualiza la opción de ver los sistemas de monetización, posteriomente selecciona la opción mencionada previamente y visualiza todas las opciones que ofrece la aplicación.

### 4.4.3. Web Applications Mock-ups

### Mock-ups versión Desktop:
#### Mock-ups de la página principal
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Pagina-principal.png?raw=true" alt="Web App Page Desktop Main page">

#### Mock-ups de la sección Géneros
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Generos.png?raw=true" alt="Web App Desktop Generos">

#### Mock-ups de la sección Populares
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Populares.png?raw=true" alt="Web App Desktop Populares">

#### Mock-ups de la sección Suscripciones
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Suscripciones.png?raw=true" alt="Web App Desktop Suscripciones">

#### Mock-ups de la sección Monetización
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Monetizacion.png?raw=true" alt="Web App Desktop artistas monetización">

#### Mock-ups de la sección Artistas
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Artistas.png?raw=true" alt="Web App Desktop Artistas">

#### Mock-ups de la sección inicio de sesión
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/iniciar-sesion-web.png?raw=true" alt="Web App Desktop Inicio de sesión">

#### Mock-ups de la sección registro
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/registro-web-app.png?raw=true" alt="Web App Desktop Registro">

#### Mock-ups de la sección perfiles
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/perfiles.png?raw=true" alt="Web App Desktop Perfiles">

#### Mock-ups de la sección chat artista
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/chat-artista.png?raw=true" alt="Web App Desktop Chat artista">

#### Mock-ups de la sección historia
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/historia.png?raw=true" alt="Web App Desktop Historia">

#### Mock-ups de la sección publicar libro
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/publicar-libro.png?raw=true" alt="Web App Desktop Publciar libro">

#### Mock-ups de la sección editar historia
<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/develop/assets/images/mockups-desktop/Editar-detalles-historia.png?raw=true" alt="Web App Desktop Editar historia">

Enlace a la mockup de la App Web en Figma: https://www.figma.com/file/llRxY8xD9zTHhYNwSaoRHP/ArtCollab-WebApp?type=design&node-id=0%3A1&mode=design&t=Z0sYOEHMCMKvy3wN-1

### 4.4.4 Web Applications User Flow Diagrams.

Enlace de los User Flow Diagrams en LucidChart: https://lucid.app/lucidchart/3042a7f1-cfbd-49ad-bb1d-7d5b1e8f9c67/edit?viewport_loc=248%2C38%2C5260%2C2976%2C0_0&invitationId=inv_faedf934-db22-495f-9b16-9d38cb444726


<h4> <strong> User goal, usuario inicia sesion, se registra y recupera su contraseña </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/InicioSesion.png"/>

<h4> <strong> UUser goal, usuario publica una nueva historia y agrega series a la historia </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/PublicarLibro.png"/>

<h4> <strong> User goal, usuario edita el contenido de una historia, como el contenido y las series. </strong> </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/EditarLibro.png"/>

<h4> User goal, usuario busca artistas, contacta con ellos e inicia una sala de chats  </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/652db5f0d26cd0c9384cba2b532d6f306af7ec45/assets/Userflow-diagrams/IniciarSala.png"/>

<h4> User goal, usuario del tipo ilustrador edita su perfil </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/EditarPerfilArtista.png"/>

<h4> User goal, usuario del tipo escritor edita su perfil</h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/EditarPerfilEscritor.png"/>

<h4> User goal, usuario busca un libro segun su popularidad y género  </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/BuscarLibros.png"/>

<h4> User goal: usuario edita el perfil de cuenta </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/EditarCuenta.png"/>

<h4>  User goal, usuario visualiza las comisiones obtenidas por cada historia </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/ComisionesObras.png"/>

<h4> User goal: usuario visualiza los planes de suscripción </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/Suscripcion.png"/>

<h4> User goal: usuario visualiza el sistema de monetización </h4>
<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Userflow-diagrams/Monteizacion.png"/>



## 4.5. Web Applications Prototyping.
<hr>

A continuación se presentan los prototipos de la aplicación web de ArtCollab, los cuales fueron realizados en Figma. Además,
se adjunta el enlace al video completo de la presentación del prototipo: https://upcedupe-my.sharepoint.com/:v:/g/personal/u202213983_upc_edu_pe/ERxd8dcIJ_RNuuE2NKI5LokBzgR-IeQRRlekPx7_ksMBXg?e=mrKqUY

Enlace a los prototipos de la App Web en Figma versión Desktop: https://www.figma.com/proto/llRxY8xD9zTHhYNwSaoRHP/ArtCollab-WebApp?page-id=0%3A1&type=design&node-id=153-733&viewport=504%2C535%2C0.05&t=vnFXzvafyXOAzCvf-1&scaling=scale-down&starting-point-node-id=153%3A733&show-proto-sidebar=1&mode=design

Asimismo, se presentan capturas del video de presentación del prototipo y los timings de cada sección en los que se cumplen los
user goals.

<strong> User goal: usuario inicia sesion, se registra y recupera su contraseña </strong>

Timing: 0:00

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal1.png?raw=true" alt="Web App Prototype User goal 1">
<br>
<strong> User goal: usuario publica una nueva historia y agrega series a la historia </strong>

Timing: 1:32

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal2.png?raw=true" alt="Web App Prototype User goal 2">
<br>
<strong> User goal: usuario edita el contenido de una historia, como el contenido y las series. </strong>

Timing: 2:40

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/ce9ec3bf9b9b20dbd95b91eb62fabd2545965ac8/assets/prototyping/Goal11.png?raw=true" alt="Web App Prototype User goal 3">
<br>
<strong> User goal: usuario busca artistas, contacta con ellos e inicia una sala de chats  </strong>

Timing: 3:30

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal3.png?raw=true" alt="Web App Prototype User goal 4">
<br>
<strong> User goal: usuario del tipo ilustrador edita su perfil </strong>

Timing: 4:50

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal4.png?raw=true" alt="Web App Prototype User goal 5">
<br>
<strong> User goal: usuario del tipo escritor edita su perfil </strong>

Timing: 5:27

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal5.png?raw=true" alt="Web App Prototype User goal 6">
<br>
<strong> User goal: usuario busca un libro segun su popularidad y género  </strong>

Timing: 6:05

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal 6.png?raw=true" alt="Web App Prototype User goal 7">
<br>
<strong> User goal: usuario edita el perfil de cuenta </strong>

Timing: 7:15

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal7.png?raw=true" alt="Web App Prototype User goal 8">
<br>
<strong>  User goal: usuario visualiza las comisiones obtenidas por cada historia </strong>

Timing: 7:50

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal8.png?raw=true" alt="Web App Prototype User goal 9">
<br>
<strong> User goal: usuario visualiza los planes de suscripción </strong>

Timing: 8:23

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal9.png?raw=true" alt="Web App Prototype User goal 10">
<br>
<strong> User goal: usuario visualiza el sistema de monetización </strong>

Timing: 8:54

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/461867300eebdf5ed6c15e81784db2f2167fb69b/assets/prototyping/Goal10.png?raw=true" alt="Web App Prototype User goal 11">


## 4.6. Domain-Driven Software Architecture.
<hr>

### 4.6.1. Software Architecture Context Diagram.

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/652db5f0d26cd0c9384cba2b532d6f306af7ec45/assets/C4/context-diagram.png?raw=true" alt="ArtCollab Context Diagram">

### 4.6.2. Software Architecture Container Diagram.

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/652db5f0d26cd0c9384cba2b532d6f306af7ec45/assets/C4/component-diagram.png?raw=true" alt="ArtCollab Container Diagram">

### 4.6.3. Software Architecture Component Diagram.

API Rest Component Diagram:

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/652db5f0d26cd0c9384cba2b532d6f306af7ec45/assets/C4/api-rest-component-diagram.png?raw=true" alt="API Rest Component Diagram">

User Bounded Context Component Diagram:

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/842c94958bf7962e32880a5c1f6a5a8bd2a0d89a/assets/images/C4/userbc-component-diagram.png?raw=true" alt="User BC Component Diagram">

Content Bounded Context Component Diagram:

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/842c94958bf7962e32880a5c1f6a5a8bd2a0d89a/assets/images/C4/contentbc-component-diagram.png?raw=true" alt="Content BC Component Diagram">

Collaboration Bounded Context Component Diagram:

<img src="https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report/blob/842c94958bf7962e32880a5c1f6a5a8bd2a0d89a/assets/images/C4/collaborationbc-component-diagram.png?raw=true" alt="Collaboration BC Component Diagram">

Monetization Bounded Context Component Diagram:

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/652db5f0d26cd0c9384cba2b532d6f306af7ec45/assets/C4/monetizationbc-component-diagram.png?raw=true" alt="Monetization Bounded Context Class Diagram">


## 4.7. Software Object-Oriented Design
### 4.7.1. Class Diagrams

User Bounded Context

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/fd4f4679a05d29400210de66003a7640041f480b/assets/Class%20Diagrams/ArtCollab_UserContext.png?raw=true" alt="User Bounded Context Class Diagram">

Content Bounded Context

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/fd4f4679a05d29400210de66003a7640041f480b/assets/Class%20Diagrams/ArtCollab-Content-Context.png?raw=true" alt="Content Bounded Context Class Diagram">

Collaboration Bounded Context

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/fd4f4679a05d29400210de66003a7640041f480b/assets/Class%20Diagrams/ArtCollab-colaboration-context.png?raw=true" alt="Collaboration Bounded Context Class Diagram">

Monetization Bounded Context

<img src="https://github.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/blob/fd4f4679a05d29400210de66003a7640041f480b/assets/Class%20Diagrams/ArtCollab-monetization-context.png?raw=true" alt="Monetization Bounded Context Class Diagram">

### 4.7.2. Class Dictionary
<hr>
<br>

**User Bounded Context** 

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">User</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase User representa a los usuarios de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Writer</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Writer representa a los escritores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Illustrator</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Illustrator representa a los ilustradores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Reader</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Reader representa a los lectores de la aplicación</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">UserFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase UserFactory es una clase hija de UserManager y se encarga de la creación de los usuarios del sistema.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createUser()</td>
    <td colspan="2" valign="top">Método que crea nuevos objetos de tipo User.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">WriterFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase WriterFactory es una clase hija de UserFactory. Se encarga de la creación de los usuarios escritores en la aplicación.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createUser()</td>
    <td colspan="2" valign="top">Método que crea nuevos objetos de tipo Writer.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">IllustratorFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase IllustratorFactory es una clase hija de UserFactory. Se encarga de la creación de los usuarios ilustradores en la aplicación.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createUser()</td>
    <td colspan="2" valign="top">Método que crea nuevos objetos de tipo Illustrator.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ReaderFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ReaderFactory es una clase hija de UserFactory. Se encarga de la creación de los usuarios lectores en la aplicación.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createUser()</td>
    <td colspan="2" valign="top">Método que crea nuevos objetos de tipo Reader.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">UserManager</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase UserManager se encarga de la gestión de los usuarios en el sistema.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createUser()</td>
    <td colspan="2" valign="top">Método que crea nuevos objetos de tipo User.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top">getUser()</td>
    <td colspan="2" valign="top">Método que obtiene el identificador de un usuario.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top">updateUser()</td>
    <td colspan="2" valign="top">Método que actualiza los atributos de un usuario.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top">deleteUser()</td>
    <td colspan="2" valign="top">Método que elimina a un usuario del sistema.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Account</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Account representa la cuenta de los usuarios de la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Subscription</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Subscription representa la suscripción a un plan de la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Plan</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Plan representa a los planes de suscripción de la aplicación.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">Observer</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Observer es una clase abstracta que se encarga de definir el comportamiento de UserObserver y SuscriptionObserver </td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">update()</td>
    <td colspan="2" valign="top">Método que define el comportamiento cuando ocurren cambios de estado en los sujetos observados.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">SuscriptionObserver</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase SuscriptionObserver es una clase hija de Observer. Se encarga de gestionar el estado de las suscripciones del sistema.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">update()</td>
    <td colspan="2" valign="top">Método que recibe la notificación y responde al cambio en el estado de Subscription.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">UserObserver</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase UserObserver es una clase hija de Observer. Se encarga de gestionar los estados de los usuarios en el sistema.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">update()</td>
    <td colspan="2" valign="top">Método que recibe la notificación y responde al cambio en el estado de UserManager.</td>
  </tr>
<table>

<br>

**Content Bounded Context**

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Book</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Book representa las obras que se encuentran en la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Review</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Review representa los comentarios acerca de un libro o una ilustración.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Chapter</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Chapter representa los capítulos que conforman un libro.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Illustration</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Illustration representa las ilustraciones que se encuentran en la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Review</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Review representa los comentarios acerca de un libro o una ilustración.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ContentFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ContentFactory es una clase abstracta encargada de definir la creación de distintos tipos de contenido de la aplicación.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createContent()</td>
    <td colspan="2" valign="top">Método que crea objetos de un tipo de contenido.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">BookFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase BookFactory es una clase hija de ContentFactory. Se encarga de crear nuevos libros en la plataforma.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createBook()</td>
    <td colspan="2" valign="top">Método que crea objetos del tipo Book</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">IllustrationFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase IllustrationFactory es una clase hija de ContentFactory. Se encarga de crear nuevas ilustraciones en la plataforma.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createIllustration()</td>
    <td colspan="2" valign="top">Método que crea objetos del tipo Illustration</td>
  </tr>
<table>


<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Portfolio</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Portfolio representa el portafolio de un usuario y los trabajos que ha realizado.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ViewStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ViewStrategy es una clase abstracta que define las estrategias para visualizar el contenido del portafolio. </td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">viewContent()</td>
    <td colspan="2" valign="top">Método que define la estrategia en la que se visualiza el contenido del portafolio.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">PortfolioViewStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase PortfolioViewStrategy es una clase hija de ViewStrategy. Es una interfaz la cual permite visualizar el contenido del portafolio mediante estrategias.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">viewContent()</td>
    <td colspan="2" valign="top">Método que define la estrategia en la que se visualiza el contenido del portafolio, más no su lógica.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ListViewStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ListViewStrategy es una clase hija de PortfolioViewStrategy. Es una de las estrategias de visualización del portafolio.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">viewContent()</td>
    <td colspan="2" valign="top">Método que permite ver el contenido del portafolio como una lista.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">DetailedViewStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase DetailedViewStrategy es una clase hija de PortfolioViewStrategy. Es una de las estrategias de visualización del portafolio.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">viewContent()</td>
    <td colspan="2" valign="top">Método que permite visualizar de manera más detallada el contenido presente en el portafolio.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ThumbnailViewStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ThumbnailViewStrategy es una clase hija de PortfolioViewStrategy. Es una de las estrategias de visualización del portafolio.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">viewContent()</td>
    <td colspan="2" valign="top">Método que permite visualizar en forma de miniaturas el contenido del portafolio.</td>
  </tr>
<table>

<br>

**Collaboration Bounded Context**

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Chat</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase chat representa el medio de comunicación entre los escritores y dibujantes.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Writer</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Writer representa a los escritores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Illustrator</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Illustrator representa a los ilustradores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">ChatHistory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ChatHistory representa el historial de mensajes del chat.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Activity</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Activity representa las interacciones, el estado y eventos en el chat.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">ChatMessage</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ChatMessage representa los mensajes que se encuentran en el chat.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Notification</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Notification representa las notificaciones acerca del chat.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">Observer</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Observer es una clase abstracta que define el comportamiento de ChatObserver.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">update()</td>
    <td colspan="2" valign="top">Método que define el comportamiento cuando ocurren cambios de estado en el sujeto observado.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ChatObserver</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ChatObserver es una clase hija de Observer. Se encarga de observar los cambios en ChatMessage y Notification.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">update()</td>
    <td colspan="2" valign="top">Método que recibe la notificación y responde al cambio en el estado del chat.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">ColaborationFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ColaborationFactory es una clase abstracta que define la creación de objetos de colaboración </td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ChatFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ChatFactory es una clase hija de ColaborationFactory. Se encarga de la creación de nuevos chats en la aplicación.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createChat()</td>
    <td colspan="2" valign="top">Método que crea objetos de tipo Chat.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">ChatMessageFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ChatMessageFactory es una clase hija de ColaborationFactory. Se encarga de crear mensajes para los chats dentro de la aplicación.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createChat()</td>
    <td colspan="2" valign="top">Método que crea objetos de tipo Message.</td>
  </tr>
<table>

<table border="1" width="50%">
  <tr>
    <td colspan="2" valign="top">NotificationFactory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase NotificationFactory es una clase hija de ColaborationFactory. Se encarga de crear las notificaciones de los chats.</td>
  </tr>
  <tr>
    <td colspan="1" valign="top" width="30%">Método</td>
    <td colspan="2" valign="top">Descripción</td>
  </tr>
   <tr>
    <td colspan="1" valign="top">createChat()</td>
    <td colspan="2" valign="top">Método que crea objetos de tipo Notification.</td>
  </tr>
<table>

<br>

**Monetization Bounded Context**

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">Subscription</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Subscription representa la suscripción a un plan de la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">SubscriptionHistory</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase SubscriptionHistory representa el historial de Subscription.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Plan</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Plan representa los planes de suscripción de la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Payment</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Payment representa la información de los pagos de la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">PaymentFacade</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase PaymentFacade facilita la interacción con los componentes y servicios que conforman los pagos en la plataforma.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">Observer</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Observer es una clase abstracta que define el comportamiento de SubscriptionObserver y PaymentObserver.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">SubscriptionObserver</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Observer es una clase hija de Observer. Se encarga de observar los cambios de estado de Subscription</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">PaymentObserver</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Observer es una clase hija de Observer. Se encarga de observar los cambios de estado de Payment.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">Commission</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Commission representa las comisiones que se pueden realizar en la aplicación.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Writer</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Writer representa a los escritores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Illustrator</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Illustrator representa a los ilustradores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="1" valign="top">Reader</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase Reader representa a los lectores de la aplicación</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">SubscriptionManager</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase SubscriptionManager realiza la gestión de los objetos tipo Subscription.</td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">SuscriptionStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase SuscriptionStrategy es una interfaz la cual permite visualizar las suscripciones por usuario mediante distintas estrategias.</<td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">IllustratorSuscriptionStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ReaderSuscriptionStrategy es una clase hija de SuscriptionStrategy. Es una de las estrategias de visualización de suscripción
    para los ilustradores.</<td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">WriterSuscriptionStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ReaderSuscriptionStrategy es una clase hija de SuscriptionStrategy. Es una de las estrategias de visualización de suscripción
    para los escritores.</<td>
  </tr>
<table>

<table border="1" width="30%">
  <tr>
    <td colspan="2" valign="top">ReaderSuscriptionStrategy</td>
  </tr>
    <tr>
    <td colspan="2" valign="top">La clase ReaderSuscriptionStrategy es una clase hija de SuscriptionStrategy. Es una de las estrategias de visualización de suscripción
    para los lectores.</td>
  </tr>
<table>

## 4.8. Database Design

### 4.8.1. Database Diagram
<div style="display:flex; justify-content:center; flex-direction:column;">
   <p>A continuación se detalla el modelo físico realizado para esta entrega, donde se consideró los requerimientos necesarios para el negocio.</p>
   <img src="https://raw.githubusercontent.com/Open-Source-SW54-Group-3-ArtCollab/Report/develop/assets/images/Data-Base-Design/ArtCollab_DataBase.png"> 
</div>