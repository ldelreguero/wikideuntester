# wikideuntester

René de Calle 13 decía "Atrevete". Así es como me animé a ordenar mis notas, y porqué no compartirlas. A continuación van de una manera muy descontracturada todas las cosas que fui agregando como "favoritos" en el navegador y que a medida que pasó el tiemo fuí consultando. Nada de lo que está acá es privado, todo es público y gratuito. Como hay mucho para leer, reduzco la intro y pasamos a la acción. 


Todo es mejor con musica y por eso es que no viene nada mal algo de melodía

# ¿En qué momento estás leyendo esto que parece ser una Wiki?

### Lunes mientras buscas las ganas de trabajar
* [Todo el canal, porque las ganas se esconden bien escondidas](https://www.youtube.com/channel/UCNnQqoYFCqLID3GAMkGtS6A) 


### Sabado de madrugada
* [Blues Music Playlist](https://www.youtube.com/watch?v=FMSn7wVCwaw) 


Y si la idea es que todo sea descontracturado, no va a existir ni índice ni un orden lógico así que CTRL+F y buscar. Pero, lo primero es lo primero y **Under Test** es lo primero.

**_¿Qué es Under Test?_**

Es una Comunidad en español abocada al conocimiento de Testing de software y claramente es una columna importante en mi formación como Tester. Conocí a UT cuando apenas inicié este camino de Testing, y si bien no me acuerdo cómo es que llegué sé que desde que formo parte aprendí muchisimo.

¿Querés saber más?  Unite a [nuestras redes](https://linktr.ee/under_test) sin verguenza!!








# Repos sobre testing (Roadmaps, Recursos)

- [Recursos sobre Testing ](https://github.com/Nicolopez603/recursos-testing) de [Nico Lopez ](https://www.linkedin.com/in/nicolaslopezqa/) Un gran repo!




# Automation con Playwright (Guía personal)

### Pre-requisitos recomendados para iniciar un proyecto en Playwright

Requisitos necesarios para el correcto funcionamiento de un proyecto y cómo instalarlos.

* [Visual Studio Code](https://code.visualstudio.com/docs/?dv=win)
* [Nodejs](https://nodejs.org/en/download)
* Extensión 'Playwright Test for VSCode' en Visual Studio Code (Opcional)
* [Librería DotENV](https://github.com/motdotla/dotenv) 

## Empezando 

https://www.youtube.com/watch?v=WKQricsE2SI

Para crear un proyecto base es necesario:

1- Ejecutar npm init playwright@latest

A continuación sera necesario configurar el proyecto. 

Se deberá seleccionar:

- si se desea utilizar Js o Ts.
- Cómo se llamara la carpeta donde iran los tests.
- Si se desea utilizar Github Acccions 
- Si se desea instalar los Browsers de Playwright 

2- Instalar DotEnv 

npm install dotenv --save

https://www.npmjs.com/package/dotenv


## Estructura recomendada


README.md : El archivo README debe proporcionarnos toda la documentación del proyecto, instrucciones de instalación, requisitos previos y otra información relevante para QA's, Desarrolladores o cualquier persona interesada en desplegar el proyecto.

tests/ : En esta carpeta podremos agrupar conjuntos de pruebas relacionados en subcarpetas y casos de prueba individuales. Una buena organización de carpetas facilitará la ejecución de pruebas. Algunas personas también ubican el directorio de pages.
pages o POM/ : Aquí se encontrarán las clases de objetos de página que representan diferentes páginas o componentes de la aplicación web.

resources/ : Esta carpeta contiene todos los recursos adicionales requeridos por las pruebas, como imágenes, videos o archivos de audio. Existirán subcarpetas como por ejemplo videos, data, etc. 

resources/data/ : Aquí se encontrarán los diferentes archivos que poseen los datos requeridos para los diferentes tests. Pueden ser archivos JSON, XML o CSV.

reports/ : En esta carpeta se almacenarán los informes de prueba, capturas de pantalla, videos y otros elementos generados durante la ejecución de una prueba. Es recomendable guardar los archivos según el tipo de informe o recurso para mantener una estructura de informes limpia y organizada.

utils/ : Aquí se incluirán los módulos de utilidades que proporcionan funciones y recursos comunes para las pruebas.
env: El archivo .env deberá tener todas las definiciones de variables de entorno necesarias para la ejecución de nuestro proyecto.

config: Dependiendo del framework, existirá uno o varios archivos de configuración del proyecto. Es recomendable crear un directorio si la configuración del proyecto demanda más de un archivo de configuración.

## Links útiles

### Iniciando Playwright: 

- Sitio Oficial de Playwright : https://playwright.dev/

- Introducción a Playwright utilizando TypeScript - Carlos Gauto : https://www.youtube.com/watch?v=FOTEcR3ZJ4E

- Repositorio Introducción a Playwright utilizando TypeScript - Carlos Gauto: https://github.com/charlyautomatiza/starter-playwright

- Template de Proyecto de QAlified : https://github.com/QAlified/automation-framework-playwright

- Comandos de Playwright: https://ceroshjacob.medium.com/common-playwright-commands-f640e4e1b989

- Selección de Problemas y soluciones en Playwright: https://playwrightsolutions.com/

### Artículos sobre Page Object Model en Playwright: 

- Playwright Page Object Model: A Definitive Guide: https://www.lambdatest.com/learning-hub/playwright-page-object-model

- Building a Playwright JavaScript Framework with Page Object Model: https://www.linkedin.com/pulse/building-playwright-javascript-framework-page-object-model-appmetry/?trackingId=3l1HETMuR1iFiNBY%2B0h8Nw%3D%3D

- How to apply Playwright Fixtures with Page Object Model: https://medium.com/@tpshadinijk/how-to-apply-playwright-fixtures-with-page-object-model-658368968f21

- Mastering Playwright: Best Practices for Web Automation with the Page Object Model: https://medium.com/@lucgagan/mastering-playwright-best-practices-for-web-automation-with-the-page-object-model-3541412b03d1

- Page Object Model [Question] https://github.com/microsoft/playwright/issues/1604#issuecomment-1004711489
Assertions: 

- Playwright Assertions : Complete Guide With Examples: https://www.lambdatest.com/learning-hub/playwright-assertions

### Playlists/videos Youtube: 

- Curso Playwright en español - Julian Mesa https://www.youtube.com/playlist?list=PLeo6Q1inqlOdzwuW6ivlX_95682PfsGGG

- Curso de Playwright - Guillermo Marchebout �� https://www.youtube.com/playlist?list=PLPy7Tk66qAfVXqAs1Pk99kpXdGdbbk-Pm

- Playwright más fácil no podría ser - QA Minds Lab -https://www.youtube.com/watch?v=QCS_0oc3Wi0

- Automatización de pruebas con playwright https://www.youtube.com/watch?v=kiWiP5OMFcY

- Carlos Gauto, Charly Automatiza https://www.youtube.com/@CharlyAutomatiza

- Playwright Masterclass - Playwright Test https://www.youtube.com/watch?v=VKvZSpSWDZw

- What is Playwright? (� Playwright introduction tutorial, features & demo) https://www.youtube.com/watch?v=wGr5rz8WGCE

- Reuse Playwright Code across Files and Tests with Fixtures https://www.youtube.com/watch?v=2O7dyz6XO2s

- Playwright Beginner Tutorials https://www.youtube.com/playlist?list=PLhW3qG5bs-L9sJKoT1LC5grGT77sfW0Z8

- Faker.js Tutorial - Generate Random Name with Javascript https://www.youtube.com/watch?v=16p3LC1bFZc&t=3s

- PLAYWRIGHT: Fixtures + Page Object Model (EXPLICACIÓN DETALLADA) - JoanMedia 
https://www.youtube.com/watch?v=_vEnh_sx0oQ

- Playwright with Javascript | Page Object Model Pattern | POM | Part 34 - Pavan Kumar Bhimavarapu 
https://www.youtube.com/watch?v=IUjZQC2zGfg

- Playwright with Javascript | Locating Web Elements | Playwright built-in locator methods | Part 5 - Pavan Kumar Bhimavarapu 
https://www.youtube.com/watch?v=Yqyhkk5Tr3E&list=PLUDwpEzHYYLsw33jpra65LIvX1nKWpp7-&index=5

- Para definir el tamaño de pantalla correcto de acuerdo a cada monitor:
https://whatismyviewport.com/   y https://playwright.dev/docs/api/class-page#page-set-viewport-size


- Identar código en VSC:  https://www.youtube.com/watch?v=G6vi_jO95CE

- Comparar contenido PDF https://dev.to/ryanroselloog/verify-pdf-contents-using-playwright-and-pdf2json-1dob



### Comandos útiles:

npx playwright codegen https://demotest.siu.edu.ar/ 

npx playwright test --ui

npx playwright --help

npx playwright test --debug

npx playwright test 1Test.spec.js --repeat-each=3    (Se repite 3 veces los test)

## Actualización de Playwright

- Para ver en qué versión está actualmente

npx @playwright/test --version
o
npx playwright --version

- Para actualizar a la última versión estable

npm install @playwright/test@latest

- Para actualizar los browsers

npx playwright install



- https://www.youtube.com/watch?v=WHyQsX0w_5g&t=44s

- https://stackoverflow.com/questions/70262213/playwright-before-each-for-all-spec-files


https://stackoverflow.com/questions/66132097/playwright-upload-files-from-non-input-element-that-cannot-be-used-page-setinpu

https://testerops.com/working-with-file-uploads-in-playwright/ 


https://www.programsbuzz.com/course/playwright-tutorial


https://www.npmjs.com/package/playwright-utilities

https://testerops.com/working-with-file-uploads-in-playwright/

https://stackoverflow.com/questions/66132097/playwright-upload-files-from-non-input-element-that-cannot-be-used-page-setinpu

https://www.sdetcorner.com/2022/01/file-upload-playwright.html

https://testersdock.com/playwright-file-upload/

https://www.youtube.com/watch?v=HOzbXbA423w

https://www.youtube.com/watch?v=jWrBv-b58Yw

















