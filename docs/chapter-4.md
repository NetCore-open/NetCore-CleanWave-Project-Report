# Capítulo IV: Product Design

## 4.1. Style Guidelines

En esta sección, presentaremos nuestro plan para el diseño, estilo y apariencia de nuestra página web y las páginas de nuestra aplicación. Nuestro objetivo es garantizar que los usuarios disfruten de una interfaz intuitiva y amigable. Para lograrlo, hemos optado por utilizar elementos visuales que sean claros y estéticamente agradables, y hemos establecido restricciones para evitar la inclusión de gráficos poco atractivos o que sobrecarguen la experiencia del usuario.

### 4.1.1. General Style Guidelines

**Branding:** Para la creación del logo de nuestro producto CleanWave, se ha optado por un diseño moderno y minimalista que refleje limpieza, tecnología y eficiencia. El logotipo se compone de una tipografía sans-serif elegante, acompañada de un isotipo que simboliza la fluidez del agua y la conectividad digital (IA). Los colores utilizados son profesionales y equilibrados, reforzando la imagen de una plataforma SaaS robusta y confiable para la gestión de lavanderías.

<p align="center">
  <img src="../images/logo.png" alt="Logo de CleanWave" width="40%"/>
</p>

**Tono de Comunicación:**
- **Confiable y Profesional:** Para transmitir seguridad a los dueños de lavanderías sobre el manejo de su negocio.
- **Cercano y Empático:** Lenguaje directo que facilita la adopción tecnológica en negocios tradicionales.
- **Enfocado en la Eficiencia:** Resaltando beneficios como el ahorro de tiempo y la precisión en la logística.

**Tipografía:** La tipografía seleccionada es **Montserrat**, la cual será utilizada en todos los encabezados de la aplicación por su apariencia moderna y geométrica. Para los textos de cuerpo y párrafos operativos, se utilizará **Roboto**, ofreciendo una excelente legibilidad en dispositivos móviles y de escritorio. El tamaño y peso de la fuente variarán para establecer una jerarquía visual clara entre la gestión de inventarios y los reportes analíticos.

**Colores de Marca:**
- **Azul Corporativo (#2157A4):** Color base para la identidad visual y navegación superior.
- **Azul Profundo (#0F3782):** Utilizado para menús laterales y elementos de alta jerarquía.
- **Verde Menta (#10B981):** Nuestro color de acento. Se aplica exclusivamente a botones de éxito, estados de "Pedido Listo" y elementos que refuercen la limpieza y frescura.
- **Azul Glacial (#4A5FAB):** Tono secundario para iconos y componentes visuales de apoyo.
- **Blanco Nieve (#FFFDFE):** Color de fondo para mantener una interfaz despejada y minimalista.

**Paleta de Colores:**

| Color | Código Hex | Uso Principal |
| :--- | :--- | :--- |
| Azul Principal | #2157A4 | Identidad de marca y navegación. |
| Azul Profundo | #0F3782 | Botones principales y jerarquía alta. |
| Verde Menta | #10B981 | Acento para éxito, frescura y acciones positivas. |
| Azul Detalle | #4A5FAB | Iconografía y componentes de apoyo. |
| Fondo | #FFFDFE | Fondo general de la aplicación y paneles de datos. |

<p align="center">
  <img src="../images/paleta-colores.png" alt="Paleta Colores" width="50%"/>
</p>

<p align="center">
  <img src="../images/paleta-colores-muestra.png" alt="Paleta Muestra" width="0%"/>
</p>

**Espaciado y Distribución:** El espaciado en CleanWave es fundamental para transmitir orden y pulcritud, reflejando la esencia de nuestro servicio de lavandería. Se ha diseñado una estructura con márgenes amplios entre cada elemento para que la gestión de pedidos y el seguimiento de prendas sean visualmente ligeros y fáciles de entender. Utilizaremos medidas proporcionales en toda la interfaz para asegurar que el diseño se vea organizado, equilibrado y profesional en cualquier pantalla.

### 4.1.2. Web Style Guidelines

Para CleanWave, desarrollaremos una plataforma digital que sea fácil de usar y accesible desde cualquier dispositivo con internet. Implementaremos un diseño adaptable para que los dueños de lavanderías y su personal puedan revisar toda la información de su negocio de manera fluida, ya sea desde una computadora en el local o desde un teléfono móvil durante las entregas. El objetivo principal es que la interfaz sea ligera, clara y que la información siempre esté disponible cuando se necesite.

Como equipo, hemos decidido que la estructura de la web sea muy organizada y sencilla de navegar. Queremos que el usuario encuentre lo que busca sin esfuerzo, por lo que colocaremos las funciones más importantes en lugares visibles y de fácil acceso. El diseño buscará eliminar cualquier distracción visual, permitiendo que el personal se enfoque únicamente en la gestión de las prendas y la atención a sus clientes.

**Diseño Adaptable:**
- **Versatilidad:** La página se ajustará automáticamente para verse bien tanto en pantallas grandes de escritorio como en pantallas pequeñas de celulares.
- **Facilidad de Lectura:** Los textos y cuadros de información tendrán el tamaño adecuado para que puedan leerse rápidamente sin importar el dispositivo.
- **Navegación Intuitiva:** Menús simples que permiten moverse entre las distintas secciones del sistema de forma rápida y sin complicaciones.

**Componentes Implementados:**

**Cabecera (Header):**
- Logo de CleanWave siempre visible para identificar la marca y regresar al inicio fácilmente.
- Un menú sencillo con las opciones básicas para el día a día del negocio.
- Botones de acceso al sistema claros y con los colores representativos de la marca.

**Sección Principal:**
- Mensajes directos que explican cómo CleanWave ayuda a mejorar el trabajo en la lavandería.
- Botones de acción llamativos para invitar a los nuevos usuarios a probar el sistema.
- Elementos visuales que muestran de manera simple el funcionamiento de la herramienta.

**Secciones de Trabajo:**

**Gestión de Pedidos e Inventario:** Un espacio ordenado donde se registra la ropa que ingresa y se puede ver en qué estado se encuentra cada pedido, evitando confusiones o pérdidas.

**Ayuda Logística:** Una sección diseñada para visualizar los recojos y entregas pendientes, ayudando a organizar el trabajo diario de manera más eficiente.

**Información de Planes:** Una comparación simple de las opciones disponibles para que cada dueño de lavandería elija la que mejor se adapte al tamaño de su negocio.

**Contacto y Ayuda:** Un área de soporte de fácil acceso para que los usuarios puedan comunicarse con nosotros ante cualquier duda o problema con el sistema.


## 4.2. Information Architecture

La arquitectura de la información de CleanWave establece la base organizativa de nuestras soluciones digitales. Dado que el proyecto abarca desde la captación comercial hasta la gestión operativa integral de las lavanderías, el propósito fundamental de esta arquitectura es simplificar la interacción. Se busca reducir la carga cognitiva para garantizar que los dueños de los negocios (administradores) y los usuarios finales accedan y naveguen por las distintas funcionalidades con el menor esfuerzo posible.

### 4.2.1. Organization Systems

Para garantizar una organización coherente e intuitiva en las interfaces de CleanWave, nos hemos basado exclusivamente en una única dimensión para organizar la plataforma: las **Estructuras de Organización (Organization Structures)**. Consideramos que la mejor forma de organizar nuestro sistema complejo (SaaS) es mediante un enfoque top-down que agrupe funcionalidades.

El proyecto adopta íntegramente una **Estructura Jerárquica (Tree Structure)**, a partir de la cual se derivan lógicamente todos los componentes del software, garantizando que el usuario navegue desde vistas generales hacia información detallada.

* **En la Web App Administrativa (SaaS):**
  La aplicación asienta su raíz en un **Dashboard (Panel de Control)** que sirve como nodo central, mostrando el estado actual y un resumen general de la lavandería. A partir de este nodo padre, la estructura de la aplicación web se ramifica en áreas operativas clave (nodos hijos):
  * **Módulo de Pedidos:** Que a su vez jerarquiza elementos como el Registro de Nuevos Pedidos, Histórico y Cambio de Estado de las prendas.
  * **Módulo de Logística:** Ramificado hacia la Visualización de Rutas, Entregas Pendientes y Mapas de Recolección.
  * **Módulo de Clientes:** Subdividido en Fichas de Cliente Individuales e Histórico de quejas.
  * **Módulo de Suscripción:** Desglosado en Información de Facturación y Actualización del Plan.

* **En el Tracking / Portal del Usuario Final:**
  La jerarquía es mucho más plana y asienta su raíz en el **Portal Principal de la Orden Activa**. A partir de ese nodo central, el usuario solo puede acceder a dos ramificaciones concretas (Detalles de la Orden Actual e Historial de Órdenes Previas), de manera que se limita el árbol de navegación para no saturar al usuario con opciones irrelevantes.

* **En la Landing Page Comercial:**
  La jerarquía está centrada en la "Home", donde la barra de menú inicial se desglosa hacia abajo en secciones ramificadas clave que el comprador del software necesita ver: Beneficios Centrales, Precios/Planes y Formulario de Contacto.


### 4.2.2. Labeling Systems

El sistema de etiquetado en CleanWave es consistente y fácil de entender, utilizando términos claros y descriptivos que ayudan a los usuarios a identificar rápidamente las secciones y su contenido. Ejemplos de etiquetado incluyen:

* **"Panel de Control":** La vista principal del sistema que resume el estado actual del negocio.
* **"Gestión de Pedidos":** Sección dedicada exclusivamente al registro y actualización del estado de las prendas.
* **"Rutas Logísticas":** Etiqueta clara para el módulo que optimiza los recojos y entregas a domicilio.
* **"Planes de Suscripción":** Descripción directa de las opciones de membresía disponibles para las lavanderías.
* **"Rastreo de Orden":** Sección específica para que el cliente final verifique en qué etapa de lavado está su ropa.

El etiquetado es conciso y ayuda a los usuarios a entender la estructura del contenido sin abrumarlos con información o términos técnicos de software.

### 4.2.3. SEO Tags and Meta Tags

Para optimizar la landing page de CleanWave y asegurar un buen posicionamiento en los motores de búsqueda (SEO), hemos definido las siguientes etiquetas clave:

* **Title:** CleanWave - Software Inteligente para Gestión de Lavanderías
* **Description:** Digitaliza y optimiza tu lavandería con CleanWave. Plataforma SaaS para el control de inventario de prendas, seguimiento de pedidos y optimización de rutas logísticas con IA.
* **Keywords:** software para lavanderías, gestión de lavanderías, app logística lavandería, control de inventario de ropa, rutas inteligentes IA, sistema SaaS lavanderías
* **Meta Tags:** - Viewport: width=device-width, initial-scale=1.0 - Charset: UTF-8 - Author: CleanWave Team - Robots: index, follow - Language: es-PE, en-US

### 4.2.4. Searching Systems

El sistema de búsqueda de CleanWave se adapta al entorno en el que se encuentra el usuario, priorizando la rapidez para encontrar información crítica.

* **En la Landing Page (Comercial):** Dado que es una página informativa enfocada en la conversión, no se incluye una barra de búsqueda compleja. La información está diseñada para ser altamente escaneable mediante títulos claros y navegación anclada, permitiendo al usuario encontrar planes y características con un simple *scroll*.
* **En la Plataforma SaaS (Operativa):** El motor de búsqueda interno es una herramienta fundamental para el trabajo diario de la lavandería. 
    * **Búsqueda directa:** Los empleados pueden buscar rápidamente un servicio ingresando el ID del pedido, el nombre del cliente o su número de teléfono.
    * **Filtros operativos:** Se proporcionan filtros avanzados para refinar la vista del inventario, permitiendo buscar prendas por "Estado" (Pendiente, En Lavado, Listo, Entregado) o por "Fecha de ingreso".
    * **Búsqueda logística:** En el módulo de rutas, el personal de reparto puede filtrar los recojos y entregas por zonas o distritos específicos.

### 4.2.5. Navigation Systems

El sistema de navegación es la estructura que permite a los dueños de lavanderías, empleados y clientes desplazarse de manera intuitiva y sin fricciones por toda la aplicación, sin importar el dispositivo que utilicen.

**Características principales de navegación:**

* **Barra de navegación principal (Sticky Header):** Una barra superior fija que acompaña al usuario al hacer *scroll*. En la landing page incluye enlaces directos a *Soluciones*, *Planes*, *Testimonios* y *Contacto*. En el SaaS, contiene los accesos rápidos a *Pedidos*, *Inventario* y *Rutas*.
* **Menú de hamburguesa (Diseño Responsive):** Para garantizar la operatividad en dispositivos móviles (especialmente útil para los repartidores en la calle), la navegación principal se colapsa en un menú de hamburguesa vertical, optimizando el espacio en pantallas pequeñas.
* **Call to Action Buttons (Botones CTA):** Ubicados estratégicamente para guiar los próximos pasos del usuario.
    * En la Landing: Botones como "Prueba Gratuita" (en color verde menta para destacar) y "Ver Planes" (en azul outline).
    * En el SaaS: Botones de acción rápida como "+ Nuevo Pedido" siempre visibles para agilizar la atención en mostrador.
* **Enlaces ancla (Anchor Links):** En la página comercial, los enlaces del menú dirigen suavemente a secciones específicas dentro de la misma página, permitiendo una navegación fluida sin necesidad de recargar el sitio.
* **Breadcrumbs (Migas de pan):** Utilizados dentro de la plataforma SaaS para que el usuario sepa exactamente en qué nivel del sistema se encuentra (ej. *Dashboard > Clientes > Perfil de Andrea > Pedido #1024*), facilitando el retorno a pantallas anteriores.
* **Footer Navigation:** Ubicado en la parte inferior de la página comercial, organiza enlaces secundarios por categorías: Información de la empresa, Soporte/Ayuda, Redes Sociales y Términos Legales.

## 4.3. Landing Page UI Design

En esta sección se detalla el diseño de la interfaz de usuario (UI) para la página comercial de CleanWave. El objetivo principal es traducir la Arquitectura de Información, previamente definida, en representaciones visuales claras y funcionales. El proceso abarca desde esquemas estructurales de baja fidelidad para validar la jerarquía de los datos, hasta el diseño final de alta fidelidad que experimentará el cliente.

### 4.3.1. Landing Page Wireframe

<p align="center">
  <img src="../images/LandingWireframe1.png" alt="Wireframe 1" width="85%"/>
</p>

<p align="center">
  <img src="../images/LandingWireframe2.png" alt="Wireframe 2" width="85%"/>
</p>

<p align="center">
  <img src="../images/LandingWireframe3.png" alt="Wireframe 3" width="85%"/>
</p>

Link: https://www.figma.com/design/z876Dy5cFZTavginMQPf2M/Sin-t%C3%ADtulo?node-id=0-1&t=vy9WcvpvE5uXP9R8-1


### 4.3.2. Landing Page Mock-up

<p align="center">
  <img src="../images/LandingMockup1.png" alt="Mock-up 1" width="85%"/>
</p>

<p align="center">
  <img src="../images/LandingMockup2.png" alt="Mock-up 2" width="85%"/>
</p>

<p align="center">
  <img src="../images/LandingMockup3.png" alt="Mock-up 3" width="85%"/>
</p>

<p align="center">
  <img src="../images/LandingMockup4.png" alt="Mock-up 4" width="85%"/>
</p>

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

<img alt="Design-Level Event Storming 1" src="../images/perfilCliente.JPG"/>
<img alt="Design-Level Event Storming 1" src="../images/perfilLavanderia.JPG"/>
<img alt="Design-Level Event Storming 1" src="../images/loginCleanwave.JPG"/>
<img alt="Design-Level Event Storming 1" src="../images/citaLavanderia.JPG"/>
<img alt="Design-Level Event Storming 1" src="../images/pagoServicioLavanderia.JPG"/>
<img alt="Design-Level Event Storming 1" src="../images/calificacionLavanderia.JPG"/>

### 4.4.2. Web Applications Wireflow Diagrams

### 4.4.2. Web Applications Mock-ups

### 4.4.3. Web Applications User Flow Diagrams

## 4.5. Web Applications Prototyping

## 4.6. Domain-Driven Software Architecture
En esta sección, el equipo profundiza en la arquitectura de software para la solución CleanWave, tomando como base los hitos alcanzados durante el Big Picture Event Storming. 
El objetivo es realizar una transición desde el entendimiento del negocio hacia un modelo técnico riguroso bajo la perspectiva de Domain-Driven Design (DDD).

Este enfoque permite delimitar los Bounded Contexts necesarios para separar responsabilidades críticas, como el seguimiento del estado de las prendas y el sistema de atención de quejas. 
A través de esta metodología, se han identificado los Aggregates, Events, Commands y Queries que garantizan la integridad de la lógica de negocio en cada etapa del proceso de lavandería.

Finalmente, se presenta y explica la representación visual de la arquitectura utilizando el C4 Model. 
Esta estructura jerárquica nos permite comunicar de manera efectiva la solución a través de tres niveles de detalle: el Software Architecture Context Level Diagram, los Software Architecture Container Level Diagrams y los Software Architecture Component Diagrams.
### 4.6.1. Design-Level Event Storming
La sesión se llevó a cabo de manera colaborativa utilizando la herramienta LucidChart y se estructuró en las siguientes actividades clave : 
1. Refinamiento de Eventos de Dominio
2. Identificación de Comandos y Actores
3. Definición de Agregados (Aggregates)
4. Delimitación de Bounded Contexts
5. Integración de Sistemas Externos y Queries

<img alt="Design-Level Event Storming 1" src="../images/Boundedc1.png"/>
<img alt="Design-Level Event Storming 2" src="../images/Boundedc2.png"/>
<img alt="Design-Level Event Storming 3" src="../images/Boundedc3.png"/>
<img alt="Design-Level Event Storming 4" src="../images/Boundedc4.png"/>
<img alt="Design-Level Event Storming 5" src="../images/Boundedc5.png"/>
<img alt="Design-Level Event Storming 5" src="../images/Boundedc6.png"/>

### 4.6.2. Software Architecture Context Diagram
<img alt="Context diagram" src="../images/contextdiagram2.png"/>

### 4.6.3. Software Architecture Container Diagrams

<img alt="containerdiagram" src="../images/containerdiagram1.png"/>


### 4.6.4. Software Architecture Components Diagrams

<img alt="componentdiagram" src="../images/componentdiagram1.png"/>

<img alt="componentdiagram" src="../images/componentfrontend.png"/>

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

<img alt="frontenddiagram" src="../images/frontendboundedobject.png"/>

<img alt="accessdiagram" src="../images/accessbounded.png"/>

<img alt="businessdiagram" src="../images/businessbounded.png"/>

<img alt="customerdiagram" src="../images/customerexpbounded.png"/>

<img alt="laundrydiagram" src="../images/laundryorderbounded.png"/>

<img alt="logisticsdiagram" src="../images/logisticsbounded.png"/>

<img alt="suscripciondiagram" src="../images/suscripcionbounded.png"/>

## 4.8. Database Design

### 4.8.1. Database Diagrams.

<img alt="logisticsdiagram" src="../images/dbdiagram1.png"/>

<img alt="logisticsdiagram" src="../images/dbdiagram2.png"/>

<img alt="logisticsdiagram" src="../images/dbdiagram3.png"/>

<img alt="logisticsdiagram" src="../images/dbdiagram4.png"/>

<img alt="logisticsdiagram" src="../images/dbdiagram5.png"/>

<img alt="logisticsdiagram" src="../images/dbdiagram6.png"/>