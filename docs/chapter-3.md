# Capítulo III: Requirements Specification

## 3.1. User Stories

<p>Para la especificación de requisitos de los usuarios, se desarrollaron las historias de usuario que describen cada requisito y funcionalidad que debe estar implementado en el desarrollo del producto final para satisfacer las necesidades del público objetivo. A continuación se presentan las historias de usuario relacionadas con la plataforma "CleanWave". Esta sección reúne historias de usuario centradas en la experiencia de los distintos roles: el Administrador y el usuario final. Aquí se definen las necesidades clave para cada uno, desde la navegación inicial y contacto.</p>

<table>
    <thead>
        <tr>
            <th>Story ID</th>
            <th>Título</th>
            <th>Descripción</th>
            <th>Criterios de Aceptación (Gherkin)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>EP01</td>
            <td>Landing Page Informativa</td>
            <td>Como visitante quiero explorar el sitio web para conocer el servicio y tomar decisiones informadas.</td>
            <td></td>
        </tr>
        <!-- US01 -->
        <tr>
            <td>US01</td>
            <td>Visualizar página principal</td>
            <td>Como visitante de la Landing Page, quiero acceder a la página principal para conocer el servicio.</td>
            <td>
                <strong>Escenario 1: Acceso correcto</strong><br>
                <strong>Dado que</strong> el visitante ingresa al sitio web<br>
                <strong>Cuando</strong> la página carga correctamente<br>
                <strong>Entonces</strong> el sistema muestra la información principal del servicio.<br><br>
                <strong>Escenario 2: Error de carga</strong><br>
                <strong>Dado que</strong> el visitante accede al sitio<br>
                <strong>Cuando</strong> ocurre un error de carga<br>
                <strong>Entonces</strong> el sistema muestra un mensaje informativo.
            </td>
        </tr>
        <!-- US02 -->
        <tr>
            <td>US02</td>
            <td>Ver propuesta de valor</td>
            <td>Como visitante quiero entender la propuesta de valor para evaluar el servicio.</td>
            <td>
                <strong>Escenario 1: Visualización correcta</strong><br>
                <strong>Dado que</strong> el visitante navega en la página<br>
                <strong>Cuando</strong> revisa la sección principal<br>
                <strong>Entonces</strong> el sistema presenta la propuesta de valor.<br><br>
                <strong>Escenario 2: Error de contenido</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección<br>
                <strong>Cuando</strong> el contenido no está disponible<br>
                <strong>Entonces</strong> el sistema muestra un mensaje.
            </td>
        </tr>
        <!-- US03 -->
        <tr>
            <td>US03</td>
            <td>Ver beneficios del servicio</td>
            <td>Como visitante quiero conocer los beneficios para decidir si usar el servicio.</td>
            <td>
                <strong>Escenario 1: Beneficios visibles</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección beneficios<br>
                <strong>Cuando</strong> revisa el contenido<br>
                <strong>Entonces</strong> el sistema muestra los beneficios.<br><br>
                <strong>Escenario 2: Beneficios no disponibles</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección<br>
                <strong>Cuando</strong> ocurre un error<br>
                <strong>Entonces</strong> el sistema muestra un mensaje informativo.
            </td>
        </tr>
        <!-- US04 -->
        <tr>
            <td>US04</td>
            <td>Ver cómo funciona el servicio</td>
            <td>Como visitante quiero entender el flujo del servicio para saber cómo utilizarlo.</td>
            <td>
                <strong>Escenario 1: Flujo visible</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección<br>
                <strong>Cuando</strong> revisa los pasos<br>
                <strong>Entonces</strong> el sistema muestra el proceso del servicio.<br><br>
                <strong>Escenario 2: Información no disponible</strong><br>
                <strong>Dado que</strong> el visitante accede<br>
                <strong>Cuando</strong> no hay contenido<br>
                <strong>Entonces</strong> el sistema informa al usuario.
            </td>
        </tr>
        <!-- US05 -->
        <tr>
            <td>US05</td>
            <td>Ver testimonios</td>
            <td>Como visitante quiero ver opiniones de otros usuarios para generar confianza.</td>
            <td>
                <strong>Escenario 1: Testimonios disponibles</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección testimonios<br>
                <strong>Cuando</strong> hay contenido<br>
                <strong>Entonces</strong> el sistema muestra opiniones.<br><br>
                <strong>Escenario 2: Sin testimonios</strong><br>
                <strong>Dado que</strong> el visitante accede<br>
                <strong>Cuando</strong> no hay testimonios<br>
                <strong>Entonces</strong> el sistema muestra un mensaje informativo.
            </td>
        </tr>
        <!-- US06 -->
        <tr>
            <td>US06</td>
            <td>Ver precios o planes</td>
            <td>Como visitante quiero conocer los precios para evaluar el costo del servicio.</td>
            <td>
                <strong>Escenario 1: Planes visibles</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección precios<br>
                <strong>Cuando</strong> hay información<br>
                <strong>Entonces</strong> el sistema muestra los planes.<br><br>
                <strong>Escenario 2: Planes no disponibles</strong><br>
                <strong>Dado que</strong> el visitante accede<br>
                <strong>Cuando</strong> ocurre un error<br>
                <strong>Entonces</strong> el sistema informa al usuario.
            </td>
        </tr>
        <!-- US07 -->
        <tr>
            <td>US07</td>
            <td>Contactar servicio</td>
            <td>Como visitante quiero enviar una consulta para obtener más información.</td>
            <td>
                <strong>Escenario 1: Envío exitoso</strong><br>
                <strong>Dado que</strong> el visitante completa el formulario<br>
                <strong>Cuando</strong> envía los datos<br>
                <strong>Entonces</strong> el sistema registra la solicitud.<br><br>
                <strong>Escenario 2: Datos incompletos</strong><br>
                <strong>Dado que</strong> el visitante llena el formulario<br>
                <strong>Cuando</strong> faltan datos<br>
                <strong>Entonces</strong> el sistema muestra validaciones.
            </td>
        </tr>
        <!-- US08 -->
        <tr>
            <td>US08</td>
            <td>Navegar entre secciones</td>
            <td>Como visitante quiero desplazarme por la página para explorar el contenido.</td>
            <td>
                <strong>Escenario 1: Navegación fluida</strong><br>
                <strong>Dado que</strong> el visitante interactúa con el sitio<br>
                <strong>Cuando</strong> navega entre secciones<br>
                <strong>Entonces</strong> el sistema muestra el contenido correctamente.<br><br>
                <strong>Escenario 2: Error de navegación</strong><br>
                <strong>Dado que</strong> el visitante navega<br>
                <strong>Cuando</strong> ocurre un error<br>
                <strong>Entonces</strong> el sistema muestra un mensaje.
            </td>
        </tr>
        <!-- US09 -->
        <tr>
            <td>US09</td>
            <td>Ver información de la empresa</td>
            <td>Como visitante quiero conocer la empresa para generar confianza.</td>
            <td>
                <strong>Escenario 1: Información visible</strong><br>
                <strong>Dado que</strong> el visitante accede a la sección “nosotros”<br>
                <strong>Cuando</strong> revisa la información<br>
                <strong>Entonces</strong> el sistema muestra datos de la empresa.<br><br>
                <strong>Escenario 2: Error</strong><br>
                <strong>Dado que</strong> el visitante accede<br>
                <strong>Cuando</strong> falla la carga<br>
                <strong>Entonces</strong> el sistema muestra mensaje.
            </td>
        </tr>
    </tbody>
</table>

## 3.2. Impact Mapping

## 3.3. Product Backlog
