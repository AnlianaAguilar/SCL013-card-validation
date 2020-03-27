# Tarjeta de crédito válida

## Índice

* [1. Preámbulo](#1-preámbulo)
* [2. Resumen del proyecto](#2-resumen-del-proyecto)
* [3. Objetivos de aprendizaje](#3-objetivos-de-aprendizaje)
* [4. Consideraciones generales](#4-consideraciones-generales)
* [5. Criterios de aceptación mínimos del proyecto](#5-criterios-de-aceptación-mínimos-del-proyecto)
* [6. Pistas, tips y lecturas complementarias](#6-pistas-tips-y-lecturas-complementarias)
* [7. Checklist](#8-checklist)

***

## 1. Preámbulo

El [algoritmo de Luhn](https://es.wikipedia.org/wiki/Algoritmo_de_Luhn),
también llamado algoritmo de módulo 10, es un método de suma de verificación,
se utiliza para validar números de identificación; tales como el IMEI de los
celulares, tarjetas de crédito, etc.

Este algoritmo es simple. Obtenemos la reversa del número a verificar (que
solamente contiene dígitos [0-9]); a todos los números que ocupan una posición
par se les debe multiplicar por dos, si este número es mayor o igual a 10,
debemos sumar los dígitos del resultado; el número a verificar será válido si
la suma de sus dígitos finales es un múltiplo de 10.

![gráfica de algoritmo de Luhn](https://www.101computing.net/wp/wp-content/uploads/Luhn-Algorithm.png)

## 2. Resumen del proyecto

En este proyecto tendrás que construir una aplicación web que le permita a un
usuario validar el número de una tarjeta de crédito. Además, tendrás que
implementar funcionalidad para ocultar todos los dígitos de una tarjeta menos
los últimos cuatro.

La temática es libre. Tú debes pensar en qué situaciones de la vida real se
necesitaría validar una tarjeta de crédito y pensar en cómo debe ser esa
experiencia de uso (qué pantallas, explicaciones, mensajes, colores, ¿marca?)
etc.

## 3. Objetivos de aprendizaje

Trabajando en parejas aprenderán a construir una aplicación web que interactuará
con lx usuarix final a través del navegador, utilizando HTML, CSS y JavaScript
como tecnologías.

Dicho en palabras sencillas, aprenderás a:

* Organizar tu tiempo y priorizar tareas en un entorno de
  **alta incertidumbre**.
* Entender las **necesidades del usuario** y cómo proponer una solución.
* Entender la importancia del proceso de prototipado durante la creación de un
  producto digital.
* Utilizar etiquetas semánticas de HTML y elementos de formulario.
* Mostrar elementos de formulario en la pantalla usando **HTML** y **CSS**.
* Utilizar diversos tipos de selectores en CSS: de elemento, de clase, de id.
* Utilizar el modelo de cajas de CSS (border, margin, padding).
* Definir reglas de estilo en CSS.
* Permitir al usuario interactuar con elementos del DOM y hacer que la
  aplicación responda cuando ocurran esos **eventos del DOM**.
* Manipular _**strings**_ (cadenas de texto).
* Usar **control de flujo** (bucles, condicionales, ...).
* Actualizar la pantalla con los resultados (**manipular el DOM**) a través de
  **innerHTML** o **textContent**.
* **Implementar funciones** dada una descripción de su comportamiento.
* Verificar que tus funciones hagan las cosas para las que fueron creadas
  (**pruebas unitarias (_unit tests_) con [Jest](https://jestjs.io/es-ES/)**).
* Configurar tu cuenta de git.
* Hacer _fork_ y _clonar_ el repositorio del proyecto.
* Mantener actualizado los cambios en tu repositorio remoto
  (commit, pull, push).
* Desplegar tu proyecto en [GitHub Pages](https://pages.github.com).

## Sotf Skills o Habilidades Blandas

* **Planificación, organización y manejo del tiempo** : Organizarse de manera general, haciendo una estimación aproximada de los tiempos que se necesitarán para la realización del proyecto. Conocer las ceremonias y artefactos ágiles (sprint planning, dailys, retrospectiva, revisión de tablero en trello al menos, etc) a pesar de que no se utilicen con regularidad.
* **Autoaprendizaje** : Demostrar interés y adquirir nuevos conocimientos autónomamente, estudiando de manera independiente, lo que se traduce, en que cuando es necesario, la estudiante buscará aclarar conceptos y resolver dudas sobre la materia.
* **Presentaciones** : Utilizar ciertas estrategias para hablar en público (tono y ritmo de voz adecuado, contacto visual con el público, interacción con medios de presentación), que permitan asegurar un mediano entendimiento de la audiencia.
* **Adaptabilidad** : Afrontar los cambios inesperados o nuevos desafíos con una actitud positiva, aunque no necesariamente se logre accionar o adaptarse de la mejor manera a los diferentes contextos.
* **Solución de problemas** : Trabajar en la búsqueda y en la elaboración de soluciones alternativas a problemas de mediana complejidad.
* **Responsabilidad** : Demostrar actitud de compromiso, reflejandolo en la entrega de trabajo a tiempo, conectándose a la hora acordada y/o avisando cuando no se pueda asistir.
* **Dar y recibir feedback** : Escuchar los comentarios y críticas de los demás de manera respetuosa, y/o comunicar a los demás las opiniones de forma constructiva.
* **Comunicación eficaz** : Comunicar ideas a los demás cuando es necesario, aunque no siempre se fomenten de manera proactiva estas instancias de comunicación.
* **Trabajo en equipo** : Trabajar con otros de forma colaborativa y en base a un objetivo común, entregando ideas para la construcción del proyecto.

## 4. Consideraciones generales

* Este proyecto se debe resolver de manera grupal. Recuerda que cada una aprende a diferente ritmo.
* El proyecto será entregado subiendo tu código a GitHub (commit/push) y la
  interfaz será desplegada usando GitHub pages. Si no sabes lo que es GitHub, no
  te preocupes, lo aprenderás durante este proyecto.

## 5. Criterios de aceptación mínimos del proyecto

Usa solo caracteres numéricos (dígitos) en la tarjeta a validar [0-9].

### Definición del producto

En el `README.md`, cuéntanos cómo pensaste en los usuarios y cuál fue tu proceso
para definir el producto final a nivel de experiencia y de interfaz.

* Quiénes son los principales usuarios de producto.
* Cuáles son los objetivos de estos usuarios en relación con tu producto.
* Cómo crees que el producto que estás creando está resolviendo sus problemas.

### Interfaz de usuario (UI)

La interfaz debe permitir al usuario:

* Insertar el número que queremos validar.
* Ver el resultado si es válido o no.
* Ocultar todos los dígitos de su número de tarjeta menos los últimos
4 caracteres.
* No debe poder ingresar un campo vacío.

### UX (Diseño de experiencia de usuario)

Antes de iniciar a codear, debes entender el problema que quieres solucionar y
cómo tu aplicación lo soluciona.

* Trabaja tu primer prototipo con papel y lápiz (blanco y negro).
* Luego valida esta solución con una compañera (pedir feedback).
* Toma lo aprendido al momento de validar tu primer prototipo y desarrolla un
  nuevo prototipo usando alguna herramienta para diseño de prototipos
  ([Balsamiq](https://balsamiq.com/), [Figma](https://www.figma.com/),
  [Google Slides](https://www.google.com/intl/es/slides/about/), etc.)
Estos puntos los presentarás en el `README.md`.

### Scripts / Archivos

#### General

##### `README.md`

Debe contener lo siguiente:

* Un título con el nombre de tu proyecto.
* Un resumen de 1 o 2 líneas de qué se trata tu proyecto.
* La imagen final de tu proyecto.
* Investigación UX:
  1. Explicar quiénes son los usuarios y los objetivos en relación con el
    producto.
  2. Explicar cómo el producto soluciona los problemas/necesidades de dichos
    usuarios.
  3. Luego colocarás la foto de tu primer prototipo en papel.
  4. Agregar un resumen del feedback recibido indicando las mejoras a realizar.
  5. Imagen del prototipo final.

#### Visualmente (HTML y CSS)

Deberás maquetar de forma exacta el prototipo final que hiciste en la herramienta
de diseño de prototipos que escogiste utilizando HTML y CSS. En este momento elegirás
los colores, tipo de fuente, etc a usar.

A continuación describimos los archivos que utilizarás:

##### `src/index.html`

En este archivo va el contenido que se mostrará al usuario (esqueleto HTML).
Encontrarás 3 etiquetas iniciales, las cuales si deseas puedes borrar y empezar
de cero:

* `<header>`: encabezado de tu proyecto.
* `<main>`: contenido principal de tu proyecto.
* `<footer>`: pie de página de tu proyecto.

##### `src/style.css`

Este archivo debe contener las reglas de estilo. Queremos que escribas tus
propias reglas, por eso NO está permitido el uso de frameworks de CSS
(Bootstrap, materialize, etc).

#### Funcionalmente (JavaScript - pruebas unitarias)

* La lógica del proyecto debe estar implementada completamente en JavaScript.
* En este proyecto NO está permitido usar librerías o frameworks, sólo JavaScript
puro también conocido como Vanilla JavaScript.
* No se debe utilizar la _pseudo-variable_ `this`.

Vas a tener 2 archivos JavaScript separando responsabilidades, a continuación
indicamos qué harás en cada archivo:

##### `src/validator.js`

Acá escribirás las funciones necesarias para que el usuario pueda verificar la
tarjeta de crédito y ocultar los dígitos de su número de tarjeta.
Esta función debe ser pura e independiente del DOM.

Para esto debes implementar el **objeto `validator`**, el cual ya se encuentra
_exportado_ en el _boilerplate_. Este objeto (`validator`) contiene
dos métodos (`isValid` y `maskify`):

* **`validator.isValid(creditCardNumber)`**: `creditCardNumber` es un `string`
con el número de tarjeta que se va a verificar. Esta función debe retornar un
`boolean` dependiendo si es válida de acuerdo al [algoritmo de Luhn](https://es.wikipedia.org/wiki/Algoritmo_de_Luhn).

* **`validator.maskify(creditCardNumber)`**: `creditCardNumber` es un `string` con
el número de tarjeta y esta función debe retornar un `string` donde todos menos
los últimos cuatro caracteres sean reemplazados por un numeral (`#`) o 🐱.
Esta función deberá siempre mantener los últimos cuatro caracteres intactos, aún
cuando el `string` sea de menor longitud.

    Ejemplo de uso

    ```js
    maskify('4556364607935616') === '############5616'
    maskify(     '64607935616') ===      '#######5616'
    maskify(               '1') ===                '1'
    maskify(               '')  ===                ''
    ```

##### `src/index.js`

Acá escribirás todo el código que tenga que ver con la interacción del DOM
(seleccionar, actualizar y manipular elementos del DOM y eventos).
Es decir, en este archivo deberás invocar las funciones `isValid` y `maskify`
según sea necesario para actualizar el resultado en la pantalla (UI).

##### `test/validator.spec.js`

En este archivo tendrás que completar las pruebas unitarias de las funciones
`validator.isValid(creditCardNumber)` y `validator.maskify(creditCardNumber)`
implementadas en `validator.js` utilizando [Jest](https://jestjs.io/es-ES/).
Tus pruebas unitarias deben dar un 70% en _coverage_ (cobertura),
_statements_ (sentencias), _functions_ (funciones) y _lines_ (líneas); y un
mínimo del 50% de _branches_ (ramas).

***

## 6. Pistas, tips y lecturas complementarias

### Primeros pasos

1. Antes que nada, asegúrate de tener un :pencil: editor de texto en
  condiciones, algo como [Atom](https://atom.io/) o
  [Code](https://code.visualstudio.com/).
2. Para ejecutar los comandos a continuación necesitarás una :shell:
  [UNIX Shell](https://github.com/Laboratoria/bootcamp/tree/master/topics/shell),
  que es un programita que interpreta líneas de comando (command-line
  interpreter) así como tener [git](https://github.com/Laboratoria/bootcamp/tree/master/topics/scm/01-git)
  instalado. Si usas un sistema operativo "UNIX-like", como GNU/Linux o MacOS,
  ya tienes una _shell_ (terminal) instalada por defecto (y probablemente `git`
  también). Si usas Windows puedes usar la versión completa de [Cmder](https://cmder.net/)
  que incluye [Git bash](https://git-scm.com/download/win) y si tienes Windows 10
  o superior puedes usar [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
3. Una de las integrantes del equipo debe realizar un :fork_and_knife:
  [fork](https://help.github.com/articles/fork-a-repo/) del repo de tu cohort,
  tus _coaches_ te compartirán un _link_ a un repo y te darán acceso de lectura
  en ese repo. La otra integrante del equipo deber hacer un fork **del
  repositorio de su compañera** y
  [configurar](https://gist.github.com/BCasal/026e4c7f5c71418485c1) un `remote`
  hacia el mismo.
4. :arrow_down: [Clona](https://help.github.com/articles/cloning-a-repository/)
  tu _fork_ a tu computadora (copia local).
5. 📦 Instala las dependencias del proyecto con el comando `npm install`. Esto
  asume que has instalado [Node.js](https://nodejs.org/) (que incluye [npm](https://docs.npmjs.com/)).
6. Si todo ha ido bien, deberías poder ejecutar las :traffic_light:
  pruebas unitarias (unit tests) con el comando `npm test`.
7. Para ver la interfaz de tu programa en el navegador, usa el comando
  `npm start` para arrancar el servidor web y dirígete a
  `http://localhost:5000` en tu navegador.
8. A codear se ha dicho! :rocket:

### Recursos y temas relacionados

A continuación un video de Michelle que te lleva a través del algoritmo de Luhn
y un par de cosas más que debes saber para resolver este proyecto. ¡Escúchala
con detenimiento y sigue sus consejos! :)

[![tips credit card](https://img.youtube.com/vi/f0zL6Ot9y_w/0.jpg)](https://www.youtube.com/watch?v=f0zL6Ot9y_w)

[Link](https://www.youtube.com/watch?v=f0zL6Ot9y_w)

Terminal y shell de UNIX:

[![Playlist de Terminal y shell de UNIX](https://img.youtube.com/vi/GB35Eyb-J4c/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

Control de versiones y trabajo colaborativo con Git y GitHub:

[![Playlist de control de versiones y trabajo colaborativo](https://img.youtube.com/vi/F1EoBbvhaqU/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

Diseño de experiencia de usuario (User Experience Design):

* [Ideación](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/intro-ux/01-el-proceso-de-diseno/00-el-proceso-de-diseno)
* [Prototipado (sketching)](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/intro-ux/01-el-proceso-de-diseno/00-el-proceso-de-diseno)
* [Testeo e Iteración](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/intro-ux/01-el-proceso-de-diseno/00-el-proceso-de-diseno)

Desarrollo Front-end:

* [Valores](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/javascript/01-basics/01-values-variables-and-types)
* [Tipos](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/javascript/01-basics/01-values-variables-and-types)
* [Variables](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/javascript/01-basics/02-variables)
* [Control de flujo](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/javascript/02-flow-control/00-opening)
* [Tests unitarios](https://lms.laboratoria.la/cohorts/scl-2020-03-bc-core-scl013/courses/javascript/11-testing/00-opening)
* [Documentación de NPM](https://docs.npmjs.com/)

Organización del Trabajo:

* [Metodologías Ágiles](https://www.youtube.com/watch?v=v3fLx7VHxGM)
* [Scrum en menos de 2 minutos](https://www.youtube.com/watch?v=TRcReyRYIMg)
* [Scrum en Detalle](https://www.youtube.com/watch?v=nOlwF3HRrAY&t=297s). No
  esperamos que hagas todo eso desde este proyecto. Iremos profundizando poco a
  poco a lo largo del -_bootcamp_.
* [Blog: cómo funciona el algoritmo de Luhn](http://www.quobit.mx/asi-funciona-el-algoritmo-de-luhn-para-generar-numeros-de-tarjetas-de-credito.html).

## 7. Checklist

Esta sección está para ayudarte a llevar un control de lo que vas completando.

### Parte Obligatoria

* [ ] `README.md` incluye info sobre proceso y decisiones de diseño.
* [ ] `README.md` explica claramente quiénes son los usuarios y su relación con
  el producto.
* [ ] `README.md` explica claramente cómo el producto soluciona los
  problemas/necesidades de los usuarios.
* [ ] Usa VanillaJS.
* [ ] No utiliza `this`.
* [ ] Implementa `validator.isValid`.
* [ ] Implementa `validator.maskify`.
* [ ] Pasa linter con configuración provista.
* [ ] Pasa pruebas unitarias.
* [ ] Pruebas unitarias cubren 70% de _statements_, _functions_ y _lines_, y un
  mínimo del 50% de _branches_.
* [ ] Interfaz permite ingresar un número para ser validado.
* [ ] Interfaz muestra el resultado de la validación correctamente.
* [ ] Interfaz debe ocultar con (`#`) todos los dígitos con excepción de los últimos cuatro.