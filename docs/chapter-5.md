# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

En esta sección se describen las decisiones, convenciones y principios adoptados por el equipo para garantizar la coherencia, trazabilidad y control de versiones durante el ciclo de vida del desarrollo de la solución CleanWave. Se establecen los lineamientos para la configuración del entorno de desarrollo, gestión del código fuente, convenciones de estilo y configuración de despliegue.



### 5.1.1. Software Development Environment Configuration

### 5.1.2. Source Code Management

Para administrar el progreso del código, optamos por una estrategia más simple en lugar de implementar todo el flujo de Git Flow. En nuestro caso, trabajamos directamente con una sola rama principal (main), la cual contiene la versión estable y a la vez en desarrollo de nuestro proyecto. De esta manera, todas las nuevas funcionalidades y correcciones fueron integradas directamente en la rama main, sin necesidad de crear ramas adicionales para desarrollo o características específicas. Aunque este enfoque es menos modular que Git Flow, resultó práctico para el alcance actual del proyecto, ya que permitió un control más directo del avance y evitó la sobrecarga de gestionar múltiples ramas. Además, utilizamos GitHub como repositorio central, aprovechando su función GitHub Pages para la visualización de nuestro trabajo. Esto nos permitió desplegar los archivos .html y obtener un enlace web funcional de manera rápida y sencilla. En resumen, trabajar únicamente con la rama main nos permitió avanzar con agilidad en el desarrollo de la página de destino y mantener una versión estable y actualizada del proyecto sin complicaciones adicionales en la gestión de ramas.

Enlace de la Landing Page en GitHub Pages: 

<div align="center"> <img src="../images/Landing net.png" alt="Sprint 1 Board Screenshot" width="100%"> <p><em>Figura: Repositorio Landing Page</em>
</p> </div>

Repositorio Github de la Landing Page:

<div align="center"> <img src="../images/Landing page.png" alt="Sprint 1 Board Screenshot" width="100%"> <p><em>Figura: Repositorio Landing Page</em>
</p> </div>


### 5.1.3. Source Code Style Guide & Conventions

En esta sección se establecen las normas, buenas prácticas y convenciones que se utilizarán durante el desarrollo de la aplicación web orientada a la gestión digital de lavanderías. La aplicación busca optimizar procesos operativos como el registro de pedidos, seguimiento de prendas y coordinación logística.

La adopción de estas convenciones permitirá garantizar la calidad, coherencia y mantenibilidad del código, facilitando su evolución y escalabilidad conforme el sistema crezca.

Para el desarrollo del proyecto se emplearán tecnologías como HTML, CSS y JavaScript, mientras que para la definición de escenarios de prueba se utilizará el lenguaje Gherkin, alineado a prácticas de desarrollo ágil.

 **Uso de minúsculas y nomenclatura en inglés**

Se definirá el uso de nombres en idioma inglés para variables, funciones, clases y elementos del sistema, asegurando que estos reflejen claramente su funcionalidad dentro del dominio de la lavandería (por ejemplo: order-status, pickup-time, delivery-route). 

Ejemplo: 

```
.clr {
} /* Mala práctica: nombre ambiguo y poco descriptivo */

.order-status {
} /* Buena práctica: nombre claro y relacionado con el dominio */
```
**Sangría y identación**

La identación permite delimitar visualmente bloques y estructuras del código, facilitando la comprensión de su lógica interna. Una correcta sangría mejora la legibilidad, permite identificar dependencias entre elementos y reduce errores de interpretación.

Ejemplo:

**EN HTML**
```
<ul>
  <li>Pedido registrado</li>
  <li>Pedido en proceso</li>
  <li>Pedido entregado</li>
</ul>

```
**EN CSS**
```
body {
  background: #ffffff;
  color: #333333;
}
```
**EN JavaScript**
```
function calculateTotal(price, quantity) {
  return price * quantity;
}
```
A continuación, se detallan las reglas específicas aplicadas a cada lenguaje.

**HTML**
 
 Se utilizará HTML5 como estándar principal para el desarrollo de la estructura de la aplicación web, debido a que proporciona etiquetas semánticas, soporte multimedia y compatibilidad con navegadores modernos.

Document Type

El proyecto utilizará la declaración específica de HTML5, definida como <!DOCTYPE html>, permitiendo a los navegadores interpretar correctamente la estructura del documento. 

Ejemplo:

```
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Laundry Platform</title>
</head>
<body>
</body>
</html>
```
- **Blank Lines**

Se utilizarán líneas en blanco para separar grandes bloques de contenido HTML, con el objetivo de mejorar la legibilidad del documento y facilitar la identificación visual de secciones importantes de la interfaz.

Ejemplo
```
<body>
  <header>
    <h1>Laundry Service</h1>
  </header>

  <section>
    <h2>Cómo funciona</h2>
    <p>El cliente registra o solicita su servicio y puede hacer seguimiento del pedido.</p>
  </section>

  <section>
    <h2>Beneficios</h2>
    <p>Mayor transparencia, ahorro de tiempo y mejor control operativo.</p>
  </section>
</body>
```
- **HTML Quotation Marks**

Para los valores de atributos HTML se emplearán comillas dobles (""), manteniendo consistencia en todos los documentos del proyecto.

```
<img src="laundry-order.jpg" alt="Pedido de lavandería listo para entrega" />
```
- **Multimedia Fallback**

Se proporcionará contenido alternativo para elementos multimedia, especialmente imágenes, con el objetivo de mejorar la accesibilidad y permitir una adecuada interpretación del contenido.

Ejemplo:
```
<img
  src="delivery-route.jpg"
  alt="Ruta de entrega optimizada para pedidos de lavandería"
  width="600"
/>
```
**CSS**

Se utilizará CSS3 para el diseño visual y la presentación de la aplicación web. El objetivo es mantener una hoja de estilos clara, ordenada y fácil de mantener.

Property Name Stops

Se utilizará un espacio después de los dos puntos (:) que acompañan a cada propiedad CSS, así como un único espacio entre la propiedad y su valor.

Ejemplo:
```
.order-card {
  background: #ffffff;
  padding: 16px;
}
```
- **Declaration Stops**

Cada declaración de propiedad CSS finalizará con punto y coma (;) para mantener consistencia y evitar errores de interpretación.

Ejemplo:
```
.status-label {
  color: green;
  font-weight: bold;
}
```
- **CSS Quotation Marks**

Se utilizarán comillas de manera consistente solo cuando sean necesarias, evitando su uso innecesario en rutas o propiedades donde no aporten claridad. Asimismo, se mantendrá uniformidad en el estilo de redacción de selectores y valores.

Ejemplo:
```
.banner-title {
  font-family: 'Open Sans', Arial, sans-serif;
}
```
- **Declaration Block Separation**

Se mantendrá una separación clara entre selectores y bloques de declaraciones, evitando saltos de línea innecesarios y asegurando uniformidad visual en la hoja de estilos.

Ejemplo:
```
.delivery-info {
  margin-top: 1rem;
  color: #444444;
}
```
**JavaScript**
Se utilizará JavaScript como lenguaje principal para la lógica del sistema, permitiendo implementar funcionalidades como el registro de pedidos, consulta de estados, validaciones, manejo de eventos y comportamiento dinámico de la aplicación.
- **Spaces Around Operations**

Se colocarán espacios alrededor de operadores aritméticos, de comparación y asignación, así como después de las comas, para mejorar la legibilidad del código.

Ejemplo:
```
let totalPrice = unitPrice * quantity;
const districts = ['Miraflores', 'San Isidro', 'Barranco'];
```
- **End of Simple Declaration**
Toda declaración simple deberá finalizar con punto y coma (;), incluyendo variables, constantes y asignaciones.

Ejemplo:

```
const orderStatus = 'ready';
let deliveryTime = 30;
```
- **General Rules for Complex Statements**
Las estructuras complejas, como condicionales, bucles y funciones, seguirán una sintaxis clara y consistente:

La llave de apertura irá al final de la línea.
Se dejará un espacio antes de la llave de apertura.
La llave de cierre irá en una nueva línea.
No se colocará punto y coma al final del bloque.

Ejemplo:
```
if (orderStatus === 'ready') {
  notifyCustomer();
}
```
- **Uso de nombres descriptivos**
Las funciones y variables deberán reflejar claramente su propósito dentro del dominio del negocio. En vez de utilizar nombres genéricos, se emplearán denominaciones relacionadas con el sistema de lavanderías. 

Ejemplo:
```
function updateOrderStatus(orderId, newStatus) {
  console.log(orderId, newStatus);
}
```
**Gherkin**

Gherkin será utilizado como lenguaje de especificación para describir escenarios de prueba y criterios de aceptación de las funcionalidades del sistema. Esto permitirá una comunicación más clara entre el equipo técnico y la perspectiva de negocio.
- **Discernible Given-When-Then Blocks**

Se empleará la estructura clásica de Gherkin basada en bloques Given – When – Then, utilizando And cuando sea necesario para añadir condiciones o resultados adicionales.

Ejemplo:
```
Scenario: Cliente consulta el estado de su pedido
Given que el cliente tiene un pedido registrado
And el pedido se encuentra en proceso
When consulta el estado del pedido
Then el sistema muestra el estado actual
And muestra el tiempo estimado de entrega
```
- **Steps with Tables**
Cuando un escenario requiera trabajar con múltiples registros o datos tabulares, se utilizarán tablas dentro de los pasos, facilitando la comprensión del contexto del escenario.
 
 Ejemplo:
```
Scenario: Visualizar pedidos registrados
Given que existen los siguientes pedidos:
| pedido   | estado      |
| ORD-001  | en proceso  |
| ORD-002  | listo       |
| ORD-003  | entregado   |
When el administrador consulta la lista de pedidos
Then el sistema muestra los pedidos registrados
```
- **Reducing Noise**
Se procurará eliminar información irrelevante de los escenarios, manteniendo únicamente los datos necesarios para comprender el comportamiento esperado del sistema. Esto permite que los criterios de aceptación sean más claros y fáciles de validar.

Ejemplo:
```
Scenario: Pedido listo para notificación
Given que el pedido está registrado
And el pedido cambia a estado listo
When el sistema procesa la actualización
Then el cliente recibe una notificación
```
- **Newlines between scenarios and separator comments**
Cuando se definan múltiples escenarios dentro de un mismo archivo, se dejarán líneas en blanco entre ellos y se podrán utilizar comentarios separadores para facilitar la lectura y navegación del documento.

Ejemplo:
```
#------- Escenario de consulta exitosa -------
Scenario: Cliente consulta pedido existente
Given que el cliente tiene un pedido registrado
When consulta el estado del pedido
Then el sistema muestra el estado correspondiente


#------- Escenario de pedido inexistente -------
Scenario: Cliente consulta pedido no registrado
Given que el cliente no tiene un pedido asociado
When consulta el estado del pedido
Then el sistema informa que no se encontró información
```
### 5.1.4. Software Deployment Configuration

Para desplegar nuestro landing page hemos optado por usar Github Pages el cual brinda la posibilidad de alojar sitios web estáticos sin costo alguno.

1. Ingresamos al repositorio de nuestra landing page

![Organización del repositorio](/images/Repositorio.png)

2. Ingresamos al repositorio de nuestra landing page

![Reposirotio Landing Page](/images/Landing%20page.png) 

3. Ingresamos a la sección de "Settings" del repositorio

![Settings del repositorio](/images/LandingSetting%20.png)

4. En la sección de "Pages", seleccionamos la rama "main" y la carpeta raíz (root) para desplegar nuestro sitio web.

![Configuración de Github Pages](/images/LandingSettingPage.png)

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

En esta sección, documentaremos y explicaremos el progreso del Sprint 1 en términos de desarrollo del producto y colaboración del equipo. Abordaremos varios aspectos clave, incluyendo la planificación del sprint, el backlog del sprint, la evidencia de desarrollo para la Revisión del Sprint. Además, se destacarán los aspectos relacionados con la documentación de servicios, la evidencia de despliegue de software y las perspectivas de colaboración del equipo durante el sprint. Este análisis detallado nos permitirá evaluar el progreso del proyecto y realizar ajustes necesarios para futuros sprints.

#### 5.2.1.1. Sprint Planning 1.

En esta sección, nos sumergiremos en los detalles del Sprint Planning Meeting 1.

| **Sprint #** |                 **Sprint 1**              |
|--------------|-------------------------------------------|
|**Sprint Planning Background**                            |
| Date         | 06-04-2026                                |
| Time         | 2:00 PM                                   |
| Location     | Reunión virtual mediante meet             |
| Prepared By  | Jhoan Darner Janampa Gutierrez            |
| Attendees    |                  |
| Sprint n-1 Review Summary | No aplica                    |
| Sprint n-1 Retrospective Summary | No aplica             |
| **Sprint Goal & User Stories**                           |
|**Sprint 1**  | El sprint tiene como objetivo desarrollar y publicar la landing page inicial de la startup de lavanderías digitales, la cual permitirá presentar la propuesta de valor del servicio tanto a dueños de lavanderías como a clientes finales. Durante este sprint se implementarán las secciones principales: hero con llamada a la acción, problema y solución, sección “cómo funciona”, beneficios diferenciados para ambos segmentos, testimonios simulados, sección de planes, formulario de contacto y footer con información relevante. Asimismo, se asegurará un diseño moderno, responsive y adaptable a dispositivos móviles y escritorio. El criterio de aceptación es que todas las secciones carguen correctamente, los enlaces funcionen sin errores, el formulario valide datos correctamente y la navegación sea fluida. La landing deberá estar desplegada en un hosting accesible públicamente. Como métrica de éxito, se espera lograr al menos 15 visitas únicas y 30 interacciones en los botones principales durante el sprint.                   |
| Sprint 1 Velocity   | 20 Story Points                    |
| Sum of Story Points | 38 Story Points                    |

#### 5.2.1.2. Aspect Leaders and Collaborators

En esta sección se incluye la elaboración de el artefacto Leadership-andCollaboration Matrix (LACX), el cual elegirenos quién es el líder y quiénes son los
colaboradores para este Sprint 1 

|Team Members (Last Name, First Name)|     GitHub Username     |   Landing Page   |
|------------------------------------|-------------------------|------------------|
| Miguel Angel Jara Espinoza |    MiguelJara2        |        C         |
| Janampa Gutierrez Jhoan Darner        |      orraiAKBDFSK      |        L         |
| Gabriel Marcelo Mendoza Palacios        |        GabrielMendoza18        |        C         |
| Jorge Armando Laban Hijar |   jarlh19    |        C         |


#### 5.2.1.3. Sprint Backlog n.

El Sprint Backlog es el artefacto que recoge el conjunto de User Stories seleccionadas para el Sprint y las descompone en tareas o work-items concretos que el
equipo de desarrollo debe realizar. A diferencia del Product Backlog, que contiene todas las funcionalidades priorizadas del producto, el Sprint Backlog se centra
únicamente en los elementos comprometidos para un Sprint específico.

En este caso, el Sprint Backlog 1 está orientado al desarrollo de la Landing Page de la plataforma CleanWave, incluyendo la implementación del hero, secciones de
servicios, modales, páginas de rol, footer, asistente virtual y ajustes de responsividad.


Enlace: [Enlace Sprint 1](https://upc-team-k20qr1ry.atlassian.net/jira/software/projects/CLEAN/boards/68/backlog?epics=visible&selectedIssue=CLEAN-16) 


<div align="center"> <img src="../images/Sprint1.png" alt="Sprint 1 Board Screenshot" width="100%"> <p><em>Figura: Sprint 1</em>
</p> </div>



## Sprint Backlog – Sprint 1

| ID US | Título User Story | ID WI | Título Work-Item | Descripción | Est. (Hrs) | Asignado a | Estado |
| :--- | :--- | :--- | :--- | :--- | :---: | :--- | :--- |
| **US01** | Menú de navegación | WI-01 | Implementar navbar | Crear barra de navegación con enlaces a Inicio, Beneficios, Planes y Contacto | 3 | Jhoan Janampa Gutierrez | Done |
| **US02** | Visualización de planes | WI-02 | Implementar sección de planes | Mostrar planes con precio, características y botón de acción | 4 | Jhoan Janampa Gutierrez | Done |
| **US03** | Selección de plan | WI-03 | Implementar selección de plan | Permitir seleccionar un plan y redirigir al registro | 3 | Jhoan Janampa Gutierrez | Done |
| **US04** | Propuesta de valor | WI-04 | Implementar sección hero | Crear sección principal con título, descripción y botones CTA | 4 | Jhoan Janampa Gutierrez | Done |
| **US05** | Cómo funciona | WI-05 | Implementar sección “Cómo funciona” | Mostrar flujo del servicio en pasos (registro, proceso, entrega) | 4 | Jhoan Janampa Gutierrez | Done |
| **US06** | Beneficios | WI-06 | Implementar sección beneficios | Mostrar beneficios para lavanderías y clientes | 3 | Jhoan Janampa Gutierrez | Done |
| **US07** | Testimonios | WI-07 | Implementar testimonios | Crear sección con opiniones simuladas de usuarios | 3 | Jhoan Janampa Gutierrez | Done |
| **US08** | Formulario de contacto | WI-08 | Implementar formulario | Crear formulario con validación y confirmación | 5 | Jhoan Janampa Gutierrez | Done |
| **US09** | Información de contacto | WI-09 | Implementar sección contacto | Mostrar correo, teléfono y ubicación | 2 | Jhoan Janampa Gutierrez | Done |
| **US10** | Sección “Nosotros” | WI-10 | Implementar sección empresa | Mostrar información de la startup | 3 | Jhoan Janampa Gutierrez | Done |
| **US11** | Preguntas frecuentes | WI-11 | Implementar FAQ | Crear lista de preguntas y respuestas | 3 | Jhoan Janampa Gutierrez | Done |
| **US12** | Redes sociales | WI-12 | Implementar redes sociales | Agregar enlaces a redes sociales | 2 | Jhoan Janampa Gutierrez | Done |
| **US13** | Footer | WI-13 | Implementar footer | Agregar enlaces legales y contacto | 3 | Jhoan Janampa Gutierrez | Done |
| **US14** | Responsividad | WI-14 | Adaptar diseño responsive | Ajustar diseño a móvil, tablet y desktop | 6 | Jhoan Janampa Gutierrez | Done |
| **US15** | CTA principal | WI-15 | Implementar botones CTA | Crear botones de acción para registro y contacto | 2 | Jhoan Janampa Gutierrez | Done |
| **US16** | Sección cobertura | WI-16 | Implementar cobertura | Mostrar zonas donde opera el servicio | 3 | Jhoan Janampa Gutierrez | Done |
| **US17** | Beneficios lavandería | WI-17 | Implementar beneficios B2B | Mostrar beneficios para negocios | 3 | Jhoan Janampa Gutierrez | Done |
| **US18** | Beneficios usuario | WI-18 | Implementar beneficios cliente | Mostrar beneficios para usuarios finales | 3 | Jhoan Janampa Gutierrez | Done |
| **US19** | Demo del servicio | WI-19 | Implementar demo visual | Simular flujo del pedido (registro → proceso → entrega) | 5 | Jhoan Janampa Gutierrez | Done |
| **US20** | Política de privacidad | WI-20 | Implementar sección legal | Agregar políticas y términos de uso | 2 | Jhoan Janampa Gutierrez | Done |

#### 5.2.1.4. Development Evidence for Sprint Review

A continuación presentaremos los commits realizados en el repositorio de nuestra Landing Page, todos estos commits se han hecho en la rama “main” durante el desarrollo de nuestro Sprint 1.

## Git Commit History – NetCore-LandingPage

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Committed On (Date) |
|:-----------|:-------|:----------|:---------------|:--------------------|:--------------------|
| NetCore-LandingPage | main | e9c7a8c7d61c7e733a584432af5a25fdd02f775d | feat: implement smooth scroll and DOM interactions | Added smooth scrolling behavior and JavaScript DOM event handling | Apr 21, 2026 |
| NetCore-LandingPage | main | 97d53eee124543db7fcbf953abe234b08e120407 | feat: adjust image and text grid for about section | Refined layout grid for the 'About Us' section images and text | Apr 21, 2026 |
| NetCore-LandingPage | main | bcd0f18d9fb7b45ac2972d61bc322a1af95e34f9 | feat: add team information block | Created a new block to display team member details | Apr 21, 2026 |
| NetCore-LandingPage | main | 2263d347d00df669fcb26aa4474ea9d0f12889fc | feat | General feature implementation and updates | Apr 21, 2026 |
| NetCore-LandingPage | main | 976825500023eb767bb97a999fd45524324b78c3 | feat: create mock layout for live logistics dashboard | Initial design for the logistics tracking dashboard interface | Apr 21, 2026 |
| NetCore-LandingPage | main | a5c1006695119b650e76030cb649ad83f3900789 | feat: design large buttons for role selection | Implemented high-visibility buttons for user role selection | Apr 21, 2026 |
| NetCore-LandingPage | main | 9db716e5e0fb26ef44e603dfbda9613d0b837d00 | feat: add B2B and B2C roles division | Separated logic and views for B2B and B2C segments | Apr 21, 2026 |
| NetCore-LandingPage | main | 9cba14f6b7ad666d3f79cef8967d52b6957e2244 | feat: design floating cards for services | Added CSS for floating card effects in the services section | Apr 21, 2026 |
| NetCore-LandingPage | main | ce161bbface1d4799a6c8bee2707b95ccf2a92b5 | feat: mockup core services grid | Developed the main grid layout for primary service offerings | Apr 21, 2026 |
| NetCore-LandingPage | main | 496946242a7a251264d4e85d2f815e2864a18260 | feat: design hero section typography and stats grid | Styled the hero typography and added the statistics grid | Apr 21, 2026 |
| NetCore-LandingPage | main | 3b4d7de4469ec4ca64ebd76278dbda8bd9d4bd4a | feat: build main hero section with metrics | Integrated real-time or static metrics into the hero area | Apr 21, 2026 |
| NetCore-LandingPage | main | ab88999e81b12c296315bda67b5ad9d7ea1fc81f | feat: apply fixed design and blur to navbar | Added sticky positioning and backdrop-blur filter to the navbar | Apr 21, 2026 |
| NetCore-LandingPage | main | ab88999e81b12c296315bda67b5ad9d7ea1fc81f | feat: mockup top navigation bar | Initial mockup of the fixed top navigation menu | Apr 21, 2026 |
| NetCore-LandingPage | main | af5020f9e58e846b5d7356bcf337c16d1525f1cc | feat: create reusable components (buttons and badges) | Built reusable button and badge components for the UI | Apr 21, 2026 |
| NetCore-LandingPage | main | d59656cb7b76735c3397ec0a463e415bd234b92f | feat: add color palette, typography, and CSS reset | Defined global styles, variables, and typography rules | Apr 21, 2026 |
| NetCore-LandingPage | main | 414901b4c9710534e0991b99edc18ca1171f2f9f | feat: create base HTML structure and link static files | Initialized index.html and linked CSS/JS assets | Apr 21, 2026 |
| NetCore-LandingPage | main | 35bd7458f3ae0f246c79e418748a40ae2bb2bc9d | Resolve merge conflicts | Fixed synchronization issues during branch merging | Apr 21, 2026 |
| NetCore-LandingPage | main | 35bd7458f3ae0f246c79e418748a40ae2bb2bc9d | feat: add color palette, typography, and CSS reset | Re-applied global style settings and design tokens | Apr 21, 2026 |
| NetCore-LandingPage | main | 5480b53b30733e6beef387a4beae0f9e65fe395c | feat: create base HTML structure and link static file | Refined base structure and static linking | Apr 21, 2026 |
| NetCore-LandingPage | main | 9db716e5e0fb26ef44e603dfbda9613d0b837d00 | Fix header formatting in README.md | Corrected Markdown syntax errors in the documentation | Apr 20, 2026 |
| NetCore-LandingPage | main | 11f3c1c8a8651140f46fdc4207907ccf2bf2ca0d | Landing page | General updates and content polish for the main landing | Apr 20, 2026 |
| NetCore-LandingPage | main | 34c4ee17f2eef2fd76ba92af5802ce91d5504658 | Initial commit | Project initialization and repository setup | Apr 17, 2026 |


#### 5.2.X.5. Execution Evidence for Sprint Review

Lo que se logró en el Sprint 1 es desplegar una primera versión de la landing page. En esta logramos desarrollar la barra navegadora, las secciones establecidas
de la Landing Page y el formulario de contacto. También se adoptó exitosamente la metodología GitFlow, trabajando en la branch principal “main”.

![Inicio](../images/landing.1.png)
![Que Ofrecemos](../images/landing.2.png)
![Somos Cloud](../images/landing.3.png)
![iot](../images/landing.4.png)
![Labs](../images/landing.5.png)
![Planes](../images/landing.6.png)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Durante el desarrollo del Sprint 1, logramos avances significativos en la creación y configuración del repositorio del proyecto destinado a la Landing Page. Contar con esta base desde el inicio facilitó la organización del trabajo y la estructuración de las ideas del equipo.

En la siguiente etapa, optamos por aprovechar las herramientas colaborativas de GitHub, lo que permitió mejorar la coordinación entre los integrantes. Gracias a esto, se consiguió una implementación fluida y ordenada. Asimismo, al brindar acceso al repositorio a todo el equipo y centralizar el trabajo en la rama principal, los commits se realizaron de manera rápida y sin inconvenientes, permitiendo que cada miembro pudiera visualizar los cambios y el progreso de forma constante.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

A continuación, detallaremos los procesos realizados a lo largo del Sprint 1: Lo primero que realizamos fue crear dos repositorios en GitHub, uno para nuestro
Landing Page.
![Repositorio Landing Page](../images/Landing%20page.png)

Finalmente configuramos GitHub Pages para obtener un enlace directo a la Landing Page, facilitando la revisión continua de los cambios realizados.
Link: https://netcore-open.github.io/NetCore-LandingPage/ 
![GitHub Pages](../images/gitpages.png)

#### 5.2.1.8. Team Collaboration Insights during Sprint

Mediante la sección de Insights de GitHub, se presenta a continuación la evidencia de colaboración del repositorio del Landing Page, mostrando la contribución de cada miembro del equipo durante el desarrollo del Sprint 1.

---

#### Analíticos de GitHub — Report

![Gráfica de contribuciones — Landing Page](../images/commit.png)

 #### Analíticos de GitHub — Landing Page
 
![Gráfica de contribuciones — Landing Page](../images/topcommit.png)


Las imágenes evidencian la participación de los 4 integrantes del equipo en el desarrollo y despliegue del Landing Page durante el Sprint 1. La distribución de commits refleja una colaboración activa y equitativa entre todos los miembros:

| Integrante | Usuario GitHub | Commits |
|---|---|---|
| Jhoan Darner Janampa Gutierrez | `orraiAKBDFSK` | 21 |
| Miguel Angel Jara Espinoza | `MiguelJara2` | 2 |
| Gabriel Marcelo Mendoza Palacios | `GabrielMendoza18` | 5 |
| Jorge Armando Laban Hijar | `jarlh19` | 0 |

La distribución de commits confirma que todos los integrantes tuvieron participación en el Sprint 1, con una diferencia máxima de 16 commits entre el miembro más activo y el menos activo, lo que evidencia un trabajo colaborativo a lo largo del sprint.

#### 5.2.2. Sprint 2

En esta sección, nos sumergiremos en los detalles del Sprint Planning Meeting 2.

#### 5.2.2.1.Sprint Planning 2.

| **Sprint #** |                 **Sprint 1**              |
|--------------|-------------------------------------------|
|**Sprint Planning Background**                            |
| Date         | 20-04-2026                                |
| Time         | 2:00 PM                                   |
| Location     | Reunión virtual mediante meet             |
| Prepared By  | Jhoan Darner Janampa Gutierrez            |
| Attendees    |                  |
| Sprint n-1 Review Summary | Durante el Sprint 1 se desarrolló y publicó la Landing Page inicial del proyecto, incluyendo las secciones principales, navegación responsive y formularios de contacto. Se validó correctamente la propuesta visual y la experiencia de navegación.                  |
| Sprint n-1 Retrospective Summary |El equipo identificó una buena distribución de tareas frontend; sin embargo, se detectó la necesidad de mejorar la integración entre componentes y optimizar tiempos de validación antes del despliegue.duplicaciones.             |
| **Sprint Goal & User Stories**                           |
|**Sprint 2**  | El sprint tiene como objetivo desarrollar el frontend funcional de la plataforma de gestión de lavanderías, utilizando una Fake API para simular la interacción con datos del sistema. Durante este sprint se implementarán las vistas principales relacionadas con pedidos, prendas, estados del servicio, consulta de pedidos y navegación interna del sistema. Asimismo, se utilizarán datos simulados para validar el flujo de interacción entre administrador y cliente sin depender todavía del backend real. El criterio de aceptación es que las vistas del sistema funcionen correctamente, que la Fake API permita listar, registrar, actualizar y consultar pedidos simulados, y que la navegación entre secciones sea fluida y responsive. La métrica de éxito será completar los principales flujos frontend sin errores críticos y validar al menos 5 pedidos simulados durante las pruebas internas. sprint.                   |
| Sprint 1 Velocity   | 28 Story Points                    |
| Sum of Story Points | 54 Story Points                    |

#### 5.2.2.2. Aspect Leaders and Collaborators.

En esta sección se incluye la elaboración de el artefacto Leadership-andCollaboration Matrix (LACX), el cual elegirenos quién es el líder y quiénes son los
colaboradores para este Sprint 1 

|Team Members (Last Name, First Name)|     GitHub Username     |   Landing Page   |
|------------------------------------|-------------------------|------------------|
| Miguel Angel Jara Espinoza |    MiguelJara2        |        C         |
| Janampa Gutierrez Jhoan Darner        |      orraiAKBDFSK      |        L         |
| Gabriel Marcelo Mendoza Palacios        |        GabrielMendoza18        |        C         |
| Jorge Armando Laban Hijar |   jarlh19    |        C         |
| Nestor Marcial Molina Umeres |   nestoroUpc   |        C         |
#### 5.2.2.3.Sprint Backlog 2.

El siguiente Sprint Backlog presenta las historias de usuario y tareas planificadas para el Sprint 2, orientado a la implementación del frontend en Angular y Angular Material.

Todas las tareas son monitoreadas y actualizadas mediante Jira Software.

#### 5.2.2.4.Development Evidence for Sprint Review.
#### 5.2.2.5.Execution Evidence for Sprint Review.
#### 5.2.2.6.Services Documentation Evidence for Sprint Review.
#### 5.2.2.7.Software Deployment Evidence for Sprint Review.
#### 5.2.2.8.Team Collaboration Insights during Sprint.