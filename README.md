# Capítulo V: Product Implementation, Validation & Deployment
## 5.1. Software Configuration Management.
En la siguiente sección, detallaremos las herramientas, convenciones, referencias y configuraciones empleadas a lo largo del desarrollo del proyecto, que contribuyeron a mantener la consistencia en el trabajo realizado.

### 5.1.1. Software Development Environment Configuration.
En este apartado, se mencionarán los distintos productos de software empleados por el equipo de desarrollo, para llevar acabo las actividades relacionadas con la elaboración del proyecto.

<br>

**Project Management**
1.	Google Docs:  https://docs.google.com/

    Google Docs es una plataforma web que facilita la creación de documentos para compartir y editar de forma conjunta con otros usuarios de manera sincrónica. Se utilizo para designar, organizar y hacer un seguimiento de las actividades de trabajo, así como para establecer plazos de entrega.

2.	Google Meet: https://meet.google.com/

    Google Meet es una plataforma de videoconferencias que permite realizar videollamadas con multiples participantes y programar sesiones de trabajo. Se usó como herramienta para llevar a cabo las reuniones del equipo, facilitando la comunicación entre los integrantes del proyecto.

**Requirements Managements**
1.	Trello: https://trello.com/ 

    Es un software de gestión de proyectos, que facilita asignar y organizar las tareas a realizar. Fue utilizado para el Product Backlog.

**Product UX/UI Design** 

1.  UXPressia: https://uxpressia.com/ 

    Es una herramienta en línea que permite a los equipos de trabajo identificar y comprender los problemas, necesidades y comportamiento del usuario en relación a la solución de software que se está desarrollando, con el uso de plantillas. Se usó para la elaboración de los User Personas, Empathy Maps, Journey Maps e Impact Maps.

2.	Figma: https://www.figma.com/ 

    Figma es una herramienta de edición gráfica, en donde se puede diseñar y prototipar páginas web y aplicaciones de manera colaborativa en tiempo real. Se utilizó para crear los wireframes, mock-ups y los desktop and mobile application prototype del proyecto.

3.	Miro: https://miro.com/ 

    Es una plataforma colaborativa el cual permite crear y usar pizarras digitales personalizadas en tiempo real. Miro cuenta con distintas herramientas y plantillas para la elaboración de mapeos, diagramas, flujos de trabajo, etc. En el desarrollo del proyecto, se empleó para la creación de los As-Is y Tob-Be Scenario Maps.


**Software Development** 
1.	Landing Page
    
    Para la creación de la landing page, se utilizaron las tecnologías base del desarrollo web: HTML5, CSS3 y JavaScript. También se usó los frameworks Tailwind CSS y Alpine.js para facilitar el desarrollo del proyecto.

2.	Frontend Web Applications

    En el caso de la aplicación web, además de HTML5, CSS3 y JavaScript. En el caso de los componentes, se usó Angular Material.

3. Web Services

    Para el servicio web, se empleó Java junto al framework Spring Boot. En el caso de la arquitectura, se optó por un RESTful API style.

**Software Deployment**
1. Netlify: https://www.netlify.com/

    Netlify es una plataforma de despliegue de páginas y aplicaciones web, integrandose con repositorios en Git. Se usó para hospedar la landing page del proyecto.

**Software Documentation**
1.	Vertabelo: https://vertabelo.com/

    Es una herramienta online que facilita el diseño, creación y gestión de bases de datos de manera colaborativa. Se usó para diseñar la base de datos del proyecto.

2.	LucidChart: https://lucid.app/   
    
    LucidChart es una plataforma que cuenta con opciones para la creación de diagramas, mapas mentales, flujos y más, con el uso de plantillas y tableros con edición en tiempo real. Fue utilizado en el desarrollo del diagrama de clases UML, así como los Wireflows y User Flows.

3.	Structurizr: https://www.structurizr.com/ 

    Es una plataforma que permite modelado de diagramas de arquitectura de software por medio de código. Structurizr fue utilizado para crear el modelo C4 de nuestro proyecto.         

### 5.1.2. Source Code Management.
Para el desarrollo y gestión del proyecto, fue creado una organización mediante GitHub, donde se registró todas las modificaciones realizadas a lo largo de su ciclo de vida. Este fue estructurado de la siguiente manera:
- **Organization**: https://github.com/Open-Source-SW54-Group-3-ArtCollab 
- **Landing Page Repository**: https://github.com/Open-Source-SW54-Group-3-ArtCollab/Landing-Page 
- **Report Repository**: https://github.com/Open-Source-SW54-Group-3-ArtCollab/Report 

Por otra parte, para controlar de manera efectiva los cambios en el código de la aplicación y gestionar las ramas por cada repositorio, se ha implementado GitFlow para definir y estructurar nuestro flujo de trabajo. Esto involucra la creación de dos ramas principales:
- **main**: También denominada "master", es la rama donde se encuentra la versión más estable y lista del proyecto que van a pasar a producción.
- **develop**: Es la rama donde se integra el contenido de las features. Va paralela al main. 

**Ramas auxiliares:**

- **feature**: Son las ramas donde se desarrollan las funcionalidades del proyecto. Luego de completarlas, se fusionan con la rama develop.

    El formato de nomenclatura usado para las ramas ha sido la siguiente: feature/feature-name. Aquí, "feature" indica la rama y "feature-name" el nombre de la funcionalidad que se está desarrollando. Por ejemplo, feature/log-in, se refiere a la login de la web application.

- **release**: Son las ramas donde se prepara la próxima versión del programa. En esta, se realizan las pruebas finales y se corrigen pequeños errores antes del lanzamiento definitivo. Finalizado este proceso, los cambios se fusionan con la rama develop, y luego a la rama main. 

    Se utilizó el formato "Semantic Versioning 2.0.0" para la nomenclatura de las versiones del proyecto, por ejemplo: "release/x.y.z". En donde:

    - X, Y y Z son números enteros positivos, donde cada uno se incrementa de manera numérica. 
    - X: Es la versión mayor. Cada incremento elimina la compatibilidad con versiones anteriores. Esto implica reiniciar a 0 las versiones menores y parche. 
    - Y: Es la versión menor. Cada incremento implica que se ha introducido funcionalidades que sí son compatibles con versiones anteriores. Cada vez que Y se incremente, la versión parche se reiniciará a 0.
    - Z: Es la versión parche. Solo se incrementa cuando se realizan correciones que son compatibles con versiones anteriores.

- **hotfix**: Son las ramas que se utilizan corregir errores críticos ocurridos en producción y que necesitan ser resueltos urgencia. Se originan de la rama main y se fusionan tanto con esta como con la rama develop.
</br>

**Commit Conventions**

Para el formato de los commits se siguió la estructura de Conventional Commits 1.0.0, la cual tiene la siguiente estructura:
    
    < type > [optional scope]: < description >

    [optional body]

    [optional footer(s)]

Donde:
- type: Indica el tipo de cambio realizado. Entre los valores permitidos se tienen: fix, feat, build, chore, ci, docs, style, refactor, perf, test, entre otros.
- scope: Indica dónde se realizó el commit en el proyecto. Ayuda a dar dar el contexto y alcance del cambio. Es opcional.
- description: Menciona de manera breve los cambios en el código. 

### 5.1.3. Source Code Style Guide & Conventions.
Para el desarrollo del código en HTML y CSS se decidió seguir la convención de Google HTML/CSS Style Guide. Entre las más importantes destacan:
- Se debe declarar el tipo de documento al principio del archivo con <!DOCTYPE html>.
- Indicar los meta tags 
- El elemento &lt;title&gt; se debe ubicar entre las etiquetas < head >.
- La identación es de dos espacios a la vez.
- Usar solo minúsculas para los elementos HTML, atributos, propiedades, valores y selectores CSS.
- Encerrar entre comillas a los atributos de los elementos HTML.
- Cada elemento HTML debe tener su etiqueta de cierre.
- Evitar largas líneas de código.
- Indicar el ancho y alto de las imágenes, así como el texto alternativo (*alt*).

Para el desarrollo del código en JavaScript, se eligió la convención Google Java Style Guide. Algunas de estas convenciones son: 
- Cada línea de código debe terminar con un punto y coma (;).
- Tanto las variables como funciones deben estar en Camelcase.
- Los valores strings deben estar entre comillas simples.
- La identación del contenido es de +2.
- Se debe evitar definir variables con la sentencia *var*. En su lugar, se recomienda *let* y *const*.

Para el desarrollo de los aceptance test con el leguaje Gherkin, se seleccionó “Gherkin Conventions for Readable Specifications”. Entre ellas están:
- Para describir los pasos del escenario, utilizar las palabras "Give", "When", "Then" y "And".
- Identar los pasos que comienzan con "And".
- Agregar líneas entre pasos.
- Encerrar entre comillas simples los parámetros.
- Usar un comentario separador y dos líneas en blanco entre cada escenario.

Para el desarrollo del código en Java, se seleccionó como convención estándar el Google Java Style Guid. Entre las más importantes destacan:
- Los nombres de los paquetes deben estar en minúsculas, las clases se escriben usando UpperCamelCase y lo métodos con lowerCamelCase.
- No se tabula para las indentaciones. Debe haber 2 o 4 espacios.
- Dividir las líneas de código de más de 100 caracteres.
- Los archivos Java deben tener el mismo nombre de la clase que contienen y está debe ser única y pública. 
- Luego de cada declaración, se hace un salto de línea.


### 5.1.4. Software Deployment Configuration.
En este apartado, detallaremos los pasos realizados para el despliegue de la Landing Page utilizando el servicio Netlify.

1. Luego de acceder a https://www.netlify.com/ e iniciar sesión o crear una cuenta, nos dirigimos al apartado "Sites", ubicado en el panel de control lateral.
<div align=center>
    <img src="./assets/Sites-Netlify.png" width=200px alt="Barra lateral de Netlify con la opción 'Sites' seleccionada">
    <h4> Barra lateral de Netlify con la opción 'Sites' seleccionada </h4>
</div>

2. Dentro de la sección Sites, tendremos tres opciones diferentes. En nuestro caso, seleccionamos la opción "Import from git" para importar la landing page directamente desde nuestro repositorio.

<div align=center>
    <img src="./assets/Import-Git-Netlify.png" width=500px alt="Sección 'Add your site to Netlify' con la opción Import from Git seleccionada">
    <h4> Sección 'Add your site to Netlify' con la opción Import from Git seleccionada </h4>
</div>

3. Ahora nos pedirá elegir nuestro proveedor de Git. Para este trabajo, el equipo ha manejado GitHub, por lo que seleccionaremos "Deploy with GitHub". 

<div align=center>
    <img src="./assets/Deploy-Netlify.png" width=500px alt="Sección de 'Let's deploy' your project de Netlify con la opción Deploy with GitHub seleccionada">
    <h4> Sección de 'Let's deploy' your project de Netlify con la opción Deploy with GitHub seleccionada </h4>
</div>

4. Netlify pedirá permisos en GitHub. Luego seleccionaremos la organización donde queremos instalar Netlify y qué repositorio queremos vincular.

<div align=center>
    <img src="./assets/Install-Netlify-GitHub.png" width=500px alt="Pantalla en GitHub para seleccionar la organización para instalar Netlify">
    <h4> Pantalla en GitHub para seleccionar la organización para instalar Netlify </h4>
</div>

5. Por último, indicamos el nombre con el que se desplegará la landing page y la rama para el deploy (develop). Finalmente le damos click a "Deploy artcollab"
<div align=center>
    <img src="./assets/Configuration-Part1-Netlify.PNG" width=300px alt="Primera parte de la configuración del deploy de la Landing Page en Netlify">
     <h4> Primera parte de la configuración del deploy de la Landing Page en Netlify </h4>
    <img src="./assets/Configuration-Part2-Netlify.png" width=300px alt="Segunda parte de la configuración del deploy de la Landing Page en Netlify con la opción de 'Deploy artcollab' seleccionada">
     <h4> Segunda parte de la configuración del deploy de la Landing Page en Netlify con la opción de 'Deploy artcollab' seleccionada </h4>
</div>

## 5.2. Landing Page, Services & Applications Implementation.
<hr>

### 5.2.1. Sprint 1

### 5.2.1.1. Sprint Planning 1 

<table>
     <tr> 
        <th>  Sprint #  </th>
        <th> Sprint 1 </th>
     </tr>
     <tr> 
        <td style="font-weight: bold;" colspan="7"> Sprint Planing Background</td>
     </tr>
     <tr>
       <td style="font-weight: bold;"> Date </td>
       <td> 27/03/2024 </td>
     </tr>
     <tr>
       <td style="font-weight: bold;"> Time </td>
       <td> 14:00 horas (GMT-5) </td>
     </tr>
     <tr>
       <td style="font-weight: bold;"> Location </td>
       <td> Modalidad remota a traves de la plataforma Google Meets <td>
     </tr>
      <tr>
        <td style="font-weight: bold;"> Prepared By </td>
        <td> Amaro Villanueva, Camila Elena <td>
     </tr>
        <tr>
        <td style="font-weight: bold;"> Attendees (to planning meeting) </td>
        <td> Amaro Villanueva, Camila Elena
        <br>
          Jave Diaz, Mathias Alejandro 
           <br>
         Cuadros Rodriguez, Juan Alejandro 
          <br>
           Luna Capuñay, Italo D'Alessandro
          <br>
         Huilca Chipana, Gustavo 
              <br>
         Alvarez Araguache, Samira Jetzabel
         <td>
     </tr>
     <tr>
        <td style="font-weight: bold;"> Sprint 0 Review Summary </td>
        <td> Dado que es nuestro primer sprint de desarrollo no existe 
        un review summary del sprint <td>
     </tr>
     <tr>
        <td style="font-weight: bold;"> Sprint 0 Retrospective Summary </td>
        <td> Dado a que nos encontramos en nuestro primer sprint aun no identifcamos planes de mejora.<td>
     </tr>
     <tr> 
        <td style="font-weight: bold;" colspan="7"> Sprint Goal & User Stories</td>
     </tr>
       <tr>
          <td style="font-weight: bold;"> Sprint 1 Goal</td>
          <td>  En este sprint se espera implementar el landing page con las secciones de login de inicio, hero y secciones de orientacion para el usuario, como por ejemplo footer y conocemos. En el grupo acordamos usar el framework de Tailwind.css para mejorar el maquetado y estilos de nuestra landing page, como tambien las librerias de Alpine.js y Swiper.js para facilitar la implementacion de las secciones de navbar y conocenos. Al finalizar este sprint la landing page debe estar desplegado en Netlifly y cualquier usuario deberia poder acceder y visualizar la pagina a traves de un link. <td>
      </tr>
       <tr>
          <td style="font-weight: bold;"> Sprint 1 Velocity </td>
          <td>  19  <td>
      </tr>
      <tr>
          <td style="font-weight: bold;"> Sum of Story Points </td>
          <td> 19 <td>
      </tr>


  </table>


### 5.2.1.2. Sprint backlog 1

En esta sección se muestran los tasks que se realizaron en el presente sprint y se adjunta una captura en Trello y el link del Trello.

Link de Trello: https://trello.com/invite/b/jhlFVuLG/ATTIcee340e6d0336619634d5d5ec2ff75ec31FE4502/artcollab-sprint1

<img src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/Sprint-Backlog/SprintBacklog.png"/>

<table style="width:400px; height:100px;"> 
   <tr>
      <th colspan="4"> Sprint # </th>
      <th colspan="7"> Sprint 1 </th>
   </tr>
   <tr >
     <th colspan="4"> User Story </th>
     <th colspan="7"> Work-Item /Task</th>
   </tr>
   <tr>
     <th > Id </th>
     <th colspan="3"> Title </th>
     <th> Id </th>
     <th > Title </th>
     <th> Description </th>
     <th> Estimation (Hours) </th>
     <th> Assigned To </th> 
     <th> Status (To-do / In-Process / To- Review / Done) </th>
   </tr>
     <tr>
      <th> EP1-US01 </th>
     <th colspan="3"> Barra de navegación en la Landing Page </th>
      <th> W01  </th>
     <th> Navbar Section  </th>
     <th> Implementar la navbar con direcciones a la landing page de Artcollab   </th>
     <th> 0.3  </th>
     <th> Mathias Jave </th> 
     <th> Done </th>
   </tr>
    <tr>
      <th> EP1-US01 </th>
     <th colspan="3">  Barra de navegación en la Landing Page  </th>
      <th> W02  </th>
     <th> Responsive Navbar Section </th>
     <th> Adaptar la navbar en dispositivos mobiles usando el enfoque mobile first   </th>
     <th> 0.5  </th>
     <th> Mathias Jave </th> 
     <th> Done </th>
   </tr>
    <tr>
      <th> EP1-US02 </th>
     <th colspan="3"> E1-US02 Visualización de las redes sociales mediante footer </th>
      <th> W03  </th>
     <th> Footer Section </th>
     <th> Implementar la sección footer con las direcciones a las redes sociales   </th>
     <th> 0.3  </th>
     <th> Gustavo Huilca </th> 
     <th> Done </th>
   </tr>
     <tr>
      <th> EP1-US02 </th>
     <th colspan="3"> E1-US02 Visualización de las redes sociales mediante footer </th>
      <th> W04  </th>
     <th> Responsive Footer Section </th>
     <th> Adaptar el footer en dispositivos móviles usando el enfoque mobile first   </th>
     <th> 0.3  </th>
     <th> Gustavo Huilca/Mathias Jave </th> 
     <th> Done </th>
   </tr>
     <tr>
      <th> EP1-US03 </th>
     <th colspan="3"> E1-US03  Sección de Explora </th>
      <th> W05  </th>
     <th> Explora Section </th>
     <th> Implementar la sección de explora con la información de nuestra startup   </th>
     <th> 2  </th>
     <th> Juan Cuadros/Italo Luna </th> 
     <th> Done </th>
   </tr>
     <tr>
      <th> EP1-US04</th>
     <th colspan="3"> E1-US04 Sección Colabora</th>
      <th> W06  </th>
     <th> Colabora Section </th>
     <th> Implementar la sección Colabora con la finalidad de orientar al usuario sobre nuestros servicios   </th>
     <th> 2  </th>
     <th> Samira Alvarez </th> 
     <th> Done </th>
   </tr>
     </tr>
     <tr>
      <th> EP1-US05</th>
     <th colspan="3"> E1-US05 Sección Hero</th>
      <th> W07  </th>
     <th> Hero Section </th>
     <th> Implementar la sección hero donde ofrecemos una breve descripción sobre nuestra startup.   </th>
     <th> 2  </th>
     <th> Camila Amaro </th> 
     <th> Done </th>
   </tr>
   
   

  <tr>
      <th> EP1-US17</th>
     <th colspan="3"> E1-US017   Compatibilidad con diferentes dispositivos </th>
      <th> W08  </th>
     <th> Landing Page </th>
     <th> Adaptar la comptabilidad del landing page a diferentes dispositivos.   </th>
     <th> 2.5  </th>
     <th> Mathias Jave/Italo Luna </th> 
     <th> Done </th>
   </tr>
     <tr>
      <th> EP1-U18 </th>
     <th colspan="3"> E1-US18 Accesibilidad en el Landing page</th>
      <th> W09  </th>
     <th> Landing Page </th>
     <th> Mejorar la accesibilidad en la landing page pensando en un diseño inclusivo.   </th>
     <th> 2  </th>
     <th> Camila Amaro/Samira Alvarez </th> 
     <th> Done </th>
   </tr>




</table>


### 5.2.1.3. Development Evidence for Sprint Review.

<table>

 <tr>
    <th> <strong> Repository </strong> </th>
    <th> <strong> Branch </strong> </th>
    <th> <strong> Commit ID</strong> </th>
    <th> <strong> Commit Message </strong> </th>
     <th> <strong> Commit Message (Body) </strong> </th>
     <th> <strong> Commited on (Date) </strong> </th>
 </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 3587ed1b0361c3262db1f2bba4bf2630e390d28e </th>
   <th> Initial commit </th>
   <th> </th>
   <th> 30/03/2024 </th>
  </tr>

   <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> a369c6e8bfb657ea04107fa397946f1a3b877c59 </th>
   <th> feat: add files via commit </th>
   <th> </th>
   <th> 30/03/2024 </th>
  </tr>

   <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> fa36e5ee1ec4d92e811075823e9c1bce0da09ec0 </th>
   <th> fix: size elements for small screens fixed </th>
   <th> </th>
   <th> 30/03/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> d350eae6a7d2eb2453e676a4b4859bf8e33aca72 </th>
   <th> Merge pull request #1 from Open-Source-SW54-Group-3-ArtCollab/feature/landingpage </th>
   <th> </th>
   <th> 30/03/2024 </th>
  </tr>


<tr>
   <th> Landing-Page </th> 
   <th> feature/log-in </th>
   <th> bd9ad1929dc82d3287624b362353c89819368db4 </th>
   <th> fix: screen size fixed </th>
   <th> </th>
   <th> 02/04/2024 </th>
  </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> feature/log-in </th>
   <th> d05a81f4b9d5219481e0160b3e41256ad80ac7fc </th>
   <th> fix: changed styles for small sizes </th>
   <th> </th>
   <th> 02/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> feature/log-in </th>
   <th> d05a81f4b9d5219481e0160b3e41256ad80ac7fc </th>
   <th> fix: changed styles for small sizes </th>
   <th> </th>
   <th> 02/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 2429795b0c807507dce3fda724bbeb49c87be104 </th>
   <th> feat: Added hero image </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 22363accf19395050b2318ad25cab3627855ef77 </th>
   <th> feat: Added Hero section to homepage </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 144d5d5b2ee74e8c7bd643c4949000663c5282d8 </th>
   <th> fix: refactor code and size screen fixed </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 7988e12c3dd0de54453c378e058cc0354d1d1dcc </th>
   <th> feat: add register button </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 5c5a0f2f86c48fe464cfa777fe7583f2452c456e </th>
   <th> feat: add search input and login buttons </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 46d24a5f66e83b71daae52d60cf122fc7d2345e1 </th>
   <th> fix: input button fixed </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 33b7d718738303ad32a312fd2bc499efd72e3e1a </th>
   <th> fix: refactor code </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> b4db4c54b4731c157bc5788d8df9a86fee41dfc0 </th>
   <th> fix: irelevant reference deleted and hovers fixed </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 2639cf23c0cb7839cc9ca1d37d44e7ac6b29d050  </th>
   <th> feat: Added reference to Homepage </th>
   <th> </th>
   <th> 04/04/2024 </th>
  </tr>


 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> fd937272d01bd972e95b07a257d60fcc85d39b48  </th>
   <th> fix: layouts for small screens fixed </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> e4fa23af33341ee6ada0d4d95d6f95a34212106a  </th>
   <th> fix: container size fixed </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 8be8e2938ec4120d3098c216011ff16e468c8ade  </th>
   <th> fix: container borders fixed </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 9e7b4e8ca147c90194fa6868d0a53e9cf73a1e65  </th>
   <th> fix: input type button hover fixed </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> f9749aeabed864c39fb6ab2312fa6fc37da643cf  </th>
   <th> feat: Update responsive and add fixes </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 393adf84a327e190b9d82d4d519d6f09ca8fb194  </th>
   <th> feat: test changes </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 5efc80f2801d5fe951f575508d5779fef4fa761f  </th>
   <th> fix: changed into branch </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 7b54fc3073a66eded4afd94f8b50d4bdaacfb25a  </th>
   <th> fix: update gap into nav-bar content </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> f68a90608525218a26fe14776d1ca21d35058965  </th>
   <th> fix: clear feature/footer </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 5b2d5df4019c1dee162068b099709b17d98f32bf  </th>
   <th> feat: added footer html </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 6b434b4115c8125db4a8560e3298178e99c98daa </th>
   <th> fix: Corrected icon in md size </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> fa7146de039aff90833e11a83c735cd129c8cb64 </th>
   <th> fix: Corrected icons in md size again </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 88e5073df0cc1c7c3f1a1da1a6dbb31b882c6fbe </th>
   <th> fix: Corrected social icons yet again </th>
   <th> </th>
   <th> 05/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> c233195488e28c76c1be49d7652b303163f3f67a </th>
   <th> fix: Corrected gramatical errors </th>
   <th> </th>
   <th> 07/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 7bd7040c559bcc42ea421ad5c19b9e327a08318d </th>
   <th> feat: Added pointer effect for links </th>
   <th> </th>
   <th> 07/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> d0a429776e503dd847a36104e925c3248bc14092 </th>
   <th> fix: Cleaned codes </th>
   <th> </th>
   <th> 07/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 3e0d0bd7fbcafd14f47b1ce85b5b849ef7faa5da </th>
   <th> fix: Corrected pointer effect for links </th>
   <th> </th>
   <th> 07/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 6296c32cbf1859e4de16190b91fb03ffc210b0b3 </th>
   <th> feat: add 'colabora' section </th>
   <th> </th>
   <th> 07/04/2024 </th>
  </tr>


  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> f9fadceddf9bf04f7c1c9ae881bc476dea6c5816 </th>
   <th> feat: carousel </th>
   <th> </th>
   <th> 08/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 76e0ad2518a5467a5d1e354e18bea4f3ee7bb15f </th>
   <th> fix: name js </th>
   <th> </th>
   <th> 08/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 5ddc0a6a38e08b46829ce499b18d142dfa9f1c2e </th>
   <th> fix: responsive </th>
   <th> </th>
   <th> 08/04/2024 </th>
  </tr>

 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> a201ca381e7c183fcb050ed1664ceabd6f204e61 </th>
   <th> feat: Add Artists </th>
   <th> </th>
   <th> 08/04/2024 </th>
  </tr>

 <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> cd20d390e3e3c7553e4fe7b7cfaa39a93badcb85 </th>
   <th> Merge branch 'feature/explora' of https://github.com/Open-Source-SW54-Group-3-ArtCollab/Landing-Page into feature/exploras </th>
   <th> </th>
   <th> 08/04/2024 </th>
  </tr>

  <tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 871a09d561091606651be57b644cbb312295877a </th>
   <th> feat: Add carousel artists </th>
   <th> </th>
   <th> 09/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 921956615a29006a83928f3ead07bf91acb16a45 </th>
   <th> feat: Merge to develop </th>
   <th> </th>
   <th> 10/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 8270d3af9cb71b9dae532c9fa36d55524be9cc5f </th>
   <th> feat: Merge to Feature/explora </th>
   <th> </th>
   <th> 10/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 7d1681dffa6926eb7eea55a375973f6d3bdb2afc </th>
   <th> Merge branch 'feature/colabora' into develop </th>
   <th> </th>
   <th> 10/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> c38aa5452145346cbc10a9d3c353ff54506c381f </th>
   <th> Merge branch 'feature/footer' into develop </th>
   <th> </th>
   <th> 10/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 71edef66a60ba9c639bab393f56cae8245e770f2 </th>
   <th> Merge branch 'feature/log-in' into develop </th>
   <th> </th>
   <th> 10/04/2024 </th>
  </tr>

<tr>
   <th> Landing-Page </th> 
   <th> develop </th>
   <th> 55a34ec3f76fde4b723541a87acb4ac00309ece7 </th>
   <th> feat: merge with feature/footer and feature/hero </th>
   <th> </th>
   <th> 12/04/2024 </th>
  </tr>


  </table>

### 5.2.1.4. Testing Suite Evidence for Sprint Review. 

### 5.2.1.5 Execution Evidence for Sprint Review.
<p> Para esta entrega, el equipo ArtCollab logró implementar exitosamente el landing page, en la cual se brindarán información especifica para conocer nuestra misión como startup, asi como también los servicios que ofrecemos en nuestra aplicación web. </p>

Enlace del deploy de la landing page mediante Netlify: https://stalwart-peony-7df718.netlify.app/


<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
   <h4> Hero en versión desktop </h4>
   <img style="width:500px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/hero-desktop.png"/>
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Hero en versión mobile (dropdown desactivado) </h4>
   <img style=" width:400px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/hero-mobile-1.png"/>
</div>


<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Hero en versión mobile (dropdown activado) </h4>
   <img style=" width:400px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/hero-mobile-2.png"/>
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Explora en versión desktop </h4>
   <img style=" width:600px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/explora-desktop.png"/>
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Explora en versión mobile </h4>
   <img style=" width:600px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/explora-mobile.png"/>
</div>


<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Colabora en versión desktop </h4>
   <img style=" width:600px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/colabora-desktop.png"/>
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Colabora en versión mobile </h4>
   <img style=" width:600px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/colabora-mobile.png"/>
</div>


<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Colabora en versión desktop </h4>
   <img style=" width:600px; height:70px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/footer-desktop.png"/>
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Colabora en versión mobile </h4>
   <img style=" width:300px; height:300px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/footer-mobile.png" />
</div>


<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Login versión desktop (Orientativo para el usuario, no funcional) </h4>
   <img style=" width:600px; height:300px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/login-desktop.png" />
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Login versión mobile sin dropdown (Orientativo para el usuario, no funcional) </h4>
   <img style=" width:200px; height:400px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/login-mobile-1.png" />
</div>

<div style="display:flex; justify-conten:center; flex-direction:column; align-items:center; gap:1rem;">
    <h4 style=" padding-top:10px;" > Login versión mobile con dropdown (Orientativo para el usuario, no funcional) </h4>
   <img style=" width:200px; height:400px" src="https://raw.githubusercontent.com/Aplicaciones-Web-WX53-Group2-ArtCollab/Report/develop/assets/landingpage-test/login-mobile-2.png" />
</div>



### 5.2.1.6 Services Documentation Evidence for Sprint Review.

En el alcance del sprint 1 se ha priorizado el desarrollado la landing page, por lo que para este sprint no se evidencia el empleo de web services.

### 5.2.1.7 Software Deployment Evidence for Sprint Review.
Para el presente sprint, se ha desarrollado la landing page. Para el despliegue se emplearon las siguientes herramientas.

<ul>
 <li> Git: Sistema de control de versiones el cual empleamos para trabajar de manera colaborativa y monitorear las versiones de la landing page en un repositorio remoto.

 </li>

 <li> Gitflow: Flujo de trabajo colaborativo, esto nos permitió dividir el trabajo por ramas dentro de nuestro repositorio con la finalidad de facilitar la colaboración en el desarrollo. </li>

 <li>
    GitHub: Plataforma que nos brindo la herramienta de crear nuestro repositorio para almacenar las versiones de nuestro proyecto.
 </li>

 <li>
    Netlify: Plataforma que automatiza webs estáticas que nos permitió alojar y desplegar nuestra el landing page.
 </li>

</ul>

### 5.2.1.8 Team Collaboration Insights during Sprint.
