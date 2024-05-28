# Wiki de un tester

<p align="center">
  <img height="350" src="assets/portada.jpg">
</p>

René de Calle 13 decía "Atrevete", y así es como me animé a ordenar mis notas con la intención de compartirlas. A continuación van de una manera muy descontracturada todas las cosas que a medida que pasó el tiempo fuí anotando, guardando. Nada de lo que está acá es privado, todo es público y gratuito. Como hay mucho para leer, reduzco la intro y pasamos a la acción. 


Todo es mejor con música y por eso es que  te invito a escuchar lo que más te gusta en [Youtube ](https://www.youtube.com/) mientras lees.



<p align="center">
  <img width="150" src="assets/musica.jpg">  
</p>



Por ahora no existirá un orden lógico así que CTRL+F y buscar. Pero, lo primero es lo primero y **Under Test** es lo primero.


**_¿Qué es Under Test?_**   &nbsp; &nbsp; <img width="30" src="assets/under_test_logo-removebg-preview.png">

Es una Comunidad en español abocada al conocimiento de Testing de software y claramente es una columna importante en mi formación como Tester. Conocí a UT cuando apenas inicié este camino de Testing, y si bien no me acuerdo cómo es que llegué, sé que desde que formo parte aprendí muchisimo.

¿Querés saber más?  Unite a [nuestras redes](https://linktr.ee/under_test)!!



# **Índice**   <a name="id0"></a>

1. [Repos sobre testing (Roadmaps, Recursos)](#id1)
2. [Sitios que me fueron útiles en algún momento](#id2)
3. [Data Test (Archivos útiles)](#id3)
4. [Automation con Playwright (Guía personal)](#id4)
5. [Postman y APIs Testing](#id5)
6. [Canales QA en Telegram](#id6)
7. [Bitácora ISTQB](#id7)
8. [Canales de Telegram con cursos/cupones de Udemy](#id8)
9. [Tools](#id9)
10. [Plantillas](#id10)
11. [Artículos personales](#id11)
12. [Conferencias, charlas](#id12)
13. [Chats IA](#id13)
14. [Primeros Recursos](#id14)
15. [AICS - Asociación Internacional de Calidad de Software](#id15)
16. [Verbos y/o acciones útiles para redacción de casos de prueba](#id16)


# Repos sobre testing (Roadmaps, Recursos) <a name="id1"></a>

- [Recursos sobre Testing ](https://github.com/Nicolopez603/recursos-testing) de [Nico Lopez ](https://www.linkedin.com/in/nicolaslopezqa/) Un gran repo!

[Volver al índice](#id0)

# Sitios que me fueron útiles en algún momento <a name="id2"></a>

- [Repetidor de texto ](https://www.editpad.org/tool/es/repetidor-de-texto)

- [Generador de Lorem Ipsum ](https://www.lipsum.com/)

- [Convertidor en línea gratuito de Excel a JSON ](https://bfotool.com/es/excel-to-json)

- [Convertidor en línea gratuito de csv a JSON ](https://csvjson.com/csv2json)

[Volver al índice](#id0)

# Data Test (Archivos útiles) <a name="id3"></a>

- [Free Test Data Test ](https://freetestdata.com)

- [File Examples Data Test ](https://file-examples.com)

- [LukaszLapaj REPOSITORIO GitHub software-testing-resource-pack ](https://github.com/LukaszLapaj/software-testing-resource-pack)


## PDF

- [PDF-500 palabras - 1 pagina ](files/PDF-500palabras-1pagina.pdf)
- [PDF-4000 palabras - 10 paginas ](files/PDF-4000palabras-10paginas.pdf)
- [PDF-10000 palabras - 23 paginas ](files/PDF-10000palabras-23paginas.pdf)
- [PDF-20000 palabras - 46 paginas ](files/PDF-20000palabras-46paginas.pdf)


## JPG

- [Imagen 2.5MB ](files/Imagen2-5MB.jpg) 
- [Imagen 5MB ](files/Imagen5MB.jpg) 
- [Imagen 14MB ](files/Imagen14MB.png) 
- [Imagen 19MB ](files/Imagen19MB.png) 
- [Imagen 25MB ](files/Imagen25MB.png) 
- [Imagen 45MB ](files/Imagen45MB.png) 


[Volver al índice](#id0)

# Automation con Playwright (Guía personal) <a name="id4"></a>

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

- Playwright Tutorial Full Course 2024 | Playwright Testing Tutorial - Testers Talk https://www.youtube.com/watch?v=2poXBtifpzA&list=PLUeDIlio4THEgPRVJRqZRS8uw8hhVNQCM&index=2

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

### Input Files en Playwright: 

- Working with File Uploads in Playwright https://testerops.com/working-with-file-uploads-in-playwright/

- Playwright: Upload files from non-input element that cannot be used page.setInputFiles? https://stackoverflow.com/questions/66132097/playwright-upload-files-from-non-input-element-that-cannot-be-used-page-setinpu

- FILE UPLOAD IN PLAYWRIGHT https://testersdock.com/playwright-file-upload/


### Comandos útiles:

npx playwright codegen 

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




[Volver al índice](#id0)

# Postman y APIs Testing  <a name="id5"></a>

- [Academia Postman](https://academy.postman.com/)

- [Academia Postman -Catálogo de cursos-](https://academy.postman.com/page/course-catalog)

- [API Testing Using Postman: Mastering API Testing using POSTMAN - [Complete Course])](https://www.youtube.com/playlist?list=PL8VbCbavWfeEvyUo5qCEw96LNjPR5rR2k)

- [API Testing Full Course (SDET-QA)](https://www.youtube.com/playlist?list=PLUDwpEzHYYLuW9XEvFEJk2kqsk6HqscI4)

- [Postman Course | API Testing using Postman (JoanMedia)](https://www.youtube.com/playlist?list=PLYDwWPRvXB8-3QhgZvW1xOE-T-I2W7iDx)

- [Aprender a trabajar con APIs- Alberto Ramirez Caballero - PDF ](files/libros-articulos/Aprender_a_trabajar_con_APIs-Alberto_Ramirez_Caballero.pdf)

[Volver al índice](#id0)

# Canales QA en Telegram <a name="id6"></a>

- [Under Test](https://t.me/undertest_es)

- [QA Makers](https://t.me/qamakers)

[Volver al índice](#id0)

# Bitácora ISTQB <a name="id7"></a>

- [Advanced-Test-Automation-Engineer-Syllabus-GA-2016_ES ](ISTQB/Advanced-Test-Automation-Engineer-Syllabus-GA-2016_ES.pdf)

- [Automation_Ebook ](ISTQB/Automation_Ebook.pdf)

- [ES_LA-ISTQB_CTFL_Sample-ExamA-v1-0-Questions_v4-0 ](ISTQB/ES_LA-ISTQB_CTFL_Sample-ExamA-v1-0-Questions_v4-0.pdf)

- [Foundations_of_software_testing-ISTQB_Certification ](ISTQB/Foundations_of_software_testing-ISTQB_Certification.pdf)

- [ISTQB_CTFL_Syllabus-v4.0-ES ](ISTQB/ISTQB_CTFL_Syllabus-v4.0-ES.pdf)

- [ISTQB_Exam-Structures-and-Rules_v1_1 ](ISTQB/ISTQB_Exam-Structures-and-Rules_v1_1.pdf)

- [ISTQB_Exam-Structure-Tables_v1_6 ](ISTQB/ISTQB_Exam-Structure-Tables_v1_6.pdf)

- [Fragmentos de ISTQB_CTFL_Syllabus-v4.0-ES (Personal) ](ISTQB/Bitacora_personal_ISTQB.pdf)

- [Asociación Internacional de Calidad de Software ](https://aicsvirtual.org/examen-de-certificacion-astfc/)

- [SIMULADOR EXAMEN ISTQB V4.0 - qarmy ](https://qarmy.ar/simulador-istqb/)


## Playlists

- [ISTQB FOUNDATION LEVEL 4.0 (2024) de TM SQUARE](https://www.youtube.com/playlist?list=PLj5VKaW115t0LT-7DICjHkGuxdTEqFI91)

- [ISTQB. Foundation Level v.4.0 (2023) de ISTQB Questions]( https://www.youtube.com/playlist?list=PLIzM8WZiml6JTclsuZk3ixqftuizseX0a)

- [ISTQB CTFL v4.0 - Questions and Answers with Explanation de Grand Slam I.T. School](https://youtube.com/playlist?list=PLOu3KZLoa5b-gGoez9AO6MAw1r_iUGw8O&si=OthsvHvNMnpQXHjN)

[Volver al índice](#id0)


# Canales de Telegram con cursos/cupones de Udemy <a name="id8"></a>

A continuación van los links a varios canales (muchos de ellos mirror) sobre cupones o cursos de Udemy. La verdad es que no siempre aparecen relacionados a QA, pero es bueno tenerlos a mano.

- [Aprende Todo](https://t.me/leveryth)

- [Cupones y Cursos Gratis Udemy](https://t.me/UCupones)

- [Facialix](https://t.me/facialix)

- [Cursos Gratis (Facialix)](https://t.me/CursosFacialix)

- [Cursos gratis Udemy](https://t.me/UdemyGratisFree)

[Volver al índice](#id0)

# Tools <a name="id9"></a>

Captura de video

- [SCRE.IO - Extensión de Google Chrome - ](https://chromewebstore.google.com/detail/screen-recorder/hniebljpgcogalllopnjokppmgbhaden)


Crear instructivos paso a paso

- [SCRIBE, step by step - Extensión de Google Chrome -](https://chrome.google.com/webstore/detail/scribe-%E2%80%94-documentation-so/okfkdaglfjjjfefdcppliegebpoegaii)

[Volver al índice](#id0)

# Plantillas <a name="id10"></a>

<div class="tabs-container">
  <input type="radio" id="tab1" name="tab" checked>
  <label for="tab1">Casos de Prueba</label>
  <input type="radio" id="tab2" name="tab" >
  <label for="tab2">Bugs</label>


  <div class="tab-content">
    
<div id="content1">
      <p>
      
- **ID:** 

- **Descripción:** 

- **Datos de entrada:**
  - [ ] No Aplica
  - [ ] Aplica:

- **Precondiciones:**

- **Tipo de Caso:**    

  - [ ] Feliz/Positivo
  - [ ] Negativo
  - [ ] Confirmación de cambio en BD

- **Pasos a Ejecutar:**    

  1-

  2-

  3- 

- **Resultado Esperado:** 

- **Resultado Obtenido:**

- **Post-condiciones:**    

  - [ ] No Aplica
  - [ ] Aplica:

- **Ambiente QA:**</p>
    </div>
  

<div id="content2">
  <p>

- **ID:** 

- **Descripción:** 

- **Ambiente QA/Producción:**

- **Browser:** 

- **OS:** 

- **Versión:** 

- **Datos:**
  - [ ] No Aplica
  - [ ] Aplica:

- **Pasos para la reproducción:**    

  1-

  2-

  3- 

- **Resultado Esperado:** 

- **Resultado Actual:**

- **Evidencia:**</p>
  </div>
  </div>
</div>


[Volver al índice](#id0)


# Artículos Personales <a name="id11"></a>

- [Nuestros primeros pasos en automatización](https://www.linkedin.com/pulse/nuestros-primeros-pasos-en-automatizaci%25C3%25B3n-lucas-del-reguero-mart%25C3%25ADnez-nlgrf/?trackingId=pMG1t5Jq64992Vampyg0qw%3D%3D)

- [Creando nuestro primer proyecto de automatización de pruebas](https://www.linkedin.com/pulse/creando-nuestro-primer-proyecto-de-automatizaci%25C3%25B3n-lucas-bwflf/?trackingId=aa%2BRmmFHNNudvtBaCtlhFA%3D%3D)

- [Animándome a automatizar](https://www.linkedin.com/pulse/anim%25C3%25A1ndome-automatizar-lucas-del-reguero-mart%25C3%25ADnez-t6yhf/?trackingId=BiH5PVyf7o%2Fqvr8d1oE%2FZw%3D%3D)

- [Conociendo a Kiwi TCMS](https://www.linkedin.com/pulse/conociendo-kiwi-tcms-lucas-del-reguero-mart%25C3%25ADnez-uvuuf/?trackingId=HYR2CmTWbiDJQ75Ec%2FUz6A%3D%3DD)

- [Un tester conociendo IA](https://www.linkedin.com/pulse/un-tester-conociendo-ia-lucas-del-reguero-mart%2525C3%2525ADnez-e846f/?trackingId=5YV6f57sRuqkIkkYcKmVYA%3D%3D)

[Volver al índice](#id0)


# Conferencias, charlas <a name="id12"></a>

- [TestingUy - 10 Años a puro testing - BLOQUE MAÑANA](https://www.youtube.com/watch?v=Fab1hkvJIzA)

- [TestingUy - 10 Años a puro testing - BLOQUE TARDE](https://www.youtube.com/watch?v=jeFMjc4Kt7s)

- [KEYNOTE: Testing in the Era of AI - Dona Sarkar - TestingUy](https://www.youtube.com/watch?v=WAy_YKZioco)




[Volver al índice](#id0)



# Chats IA <a name="id13"></a>+

- [QAI -asistente QA de Wiki de un Tester ](https://hf.co/chat/assistant/6632ef3447051729e87d0403 )
- [Chat GPT - Open Ai](https://chat.openai.com/)
- [HuggingChat - Hugging Face](https://huggingface.co/chat/)
- [Gemini - Google](https://gemini.google.com/app)


[Volver al índice](#id0)


# Primeros Recursos  <a name="id14"></a>

- [Webinar Testing con rueditas- Leonardo Corrales](https://www.youtube.com/watch?v=GMmVoiR4erk)

- [Validación y verificación - Nadia Cavalleri](https://www.youtube.com/watch?v=X06h1MGfvTQ)

- [¿Qué son las pruebas funcionales y no funcionales? - Nadia Cavalleri](https://www.youtube.com/watch?v=ynVgWjGodFg)

- [Los 7 principios de las pruebas - Nadia Cavalleri](https://www.youtube.com/watch?v=XhRi29HF_3I)

- [Pruebas de caja blanca, caja negra y caja gris - Nadia Cavalleri](https://www.youtube.com/watch?v=N-a5DEa_f0U)

- [INTRODUCCIÓN A LAS PRUEBAS DE SISTEMAS DE INFORMACIÓN](https://drive.google.com/file/d/1qB6AM4x7F0wf2eZS_7_NN3yJMCKXY7UY/view?usp=drive_link)

## Apuntes UnderTest

- [ Primera Entrega]( https://www.linkedin.com/posts/under-test_apuntes-primera-entrega-activity-7105344825868087296-yW6P?utm_source=share&utm_medium=member_desktop)

- [ Segunda Entrega]( https://www.linkedin.com/posts/under-test_apuntes-segunda-entrega-activity-7108462555764785152-7gIn?utm_source=share&utm_medium=member_desktop)

- [ Tercera Entrega](https://www.linkedin.com/posts/under-test_apuntes-tercera-entrega-activity-7110971012694835200-1h4N?utm_source=share&utm_medium=member_desktop)

- [ Cuarta Entrega]( https://www.linkedin.com/posts/under-test_apuntes-cuarta-entrega-activity-7115318824735846400-8nM_?utm_source=share&utm_medium=member_desktop)


# AICS - Asociación Internacional de Calidad de Software  <a name="id15"></a>

- [Guía completa del Analista de Pruebas AICS ](AICS/Guia-completa-del-Analista-de-Pruebas.pdf)

[Volver al índice](#id0)


# Verbos y/o acciones útiles para redacción de casos de prueba  <a name="id16"></a>

<details>
  <summary>Interacción con la interfaz</summary>
  
- Hacer click
- Clickear
- Presionar
- Seleccionar
- Elegir
- Ingresar
- Introducir
- Escribir
- Digitar
- Pulsar
- Arrastrar
- Soltar
- Subir
- Descargar
- Abrir
- Cerrar
- Maximizar
- Minimizar
- Restaurar
- Redimensionar
- Acercar
- Alejar
- Rotar
- Girar
- Zoom in
- Zoom out
- Deslizar
- Desplazar
- Mover
- Posicionar
- Ubicar

</details>

<details>
  <summary>Navegación</summary>
  
- Ir a
- Acceder a
- Visitar
- Entrar en
- Salir de
- Regresar a
- Avanzar a
- Retroceder a
- Cambiar a
- Volver a
- Saltar a
- Ir atrás
- Ir adelante
- Subir nivel
- Bajar nivel
- Ir al inicio
- Ir al final
- Ir a la página anterior
- Ir a la página siguiente

</details>

<details>
  <summary>Ingreso de datos</summary>

- Ingresar texto
- Introducir número
- Seleccionar fecha
- Elegir opción
- Escribir comentario
- Adjuntar archivo
- Subir imagen
- Grabar audio
- Capturar video
- Ingresar código
- Generar clave
- Crear contraseña
- Restablecer contraseña
- Verificar captcha
- Ingresar PIN
- Ingresar código de seguridad

</details>


<details>
  <summary>Validación</summary>

- Verificar
- Comprobar
- Validar
- Confirmar
- Revisar
- Inspeccionar
- Evaluar
- Verificar existencia
- Comprobar formato
- Validar longitud
- Verificar patrón
- Comprobar sintaxis
- Validar estructura
- Verificar contenido
- Comprobar autenticidad
  
</details>


<details>
  <summary>Acciones</summary>
  
- Crear
- Editar
- Eliminar
- Actualizar
- Guardar
- Cancelar
- Restaurar
- Imprimir
- Exportar
- Importar
- Copiar
- Pegar
- Cortar
- Pegar especial
- Duplicar
- Mover a
- Copiar a
- Renombrar
- Reemplazar
- Borrar

</details>



<details>
  <summary>Autenticación</summary>
  
- Iniciar sesión
- Cerrar sesión
- Registrarse
- Recuperar contraseña
- Cambiar contraseña
- Olvidar contraseña
- Restablecer contraseña
- Verificar cuenta
- Activar cuenta
- Desactivar cuenta
- Bloquear cuenta
- Desbloquear cuenta
- Cambiar permisos
- Asignar roles

</details>



<details>
  <summary>Notificaciones</summary>
  
- Mostrar mensaje
- Ocultar mensaje
- Enviar notificación
- Recibir notificación
- Leer notificación
- Eliminar notificación
- Marcar como leída
- Marcar como no leída
- Silenciar notificaciones
- Activar notificaciones
- Personalizar notificaciones

</details>



<details>
  <summary>Flujo de trabajo</summary>

- Iniciar proceso
- Continuar proceso
- Detener proceso
- Reanudar proceso
- Finalizar proceso
- Aprobar proceso
- Rechazar proceso
- Pendiente proceso
- Archivar proceso
- Reabrir proceso
- Reasignar proceso
- Delegar tarea

</details>



<details>
  <summary>Búsqueda</summary>
  
- Buscar texto
- Filtrar resultados
- Ordenar lista
- Filtar por categoría
- Buscar por autor
- Buscar por fecha
- Buscar por título
- Buscar por descripción
- Refinar búsqueda
- Ampliar búsqueda

</details>


<details>

  <summary>Comunicación</summary>
  
- Enviar correo electrónico
- Recibir correo electrónico
- Leer correo electrónico
- Responder correo electrónico
- Reenviar correo electrónico
- Eliminar correo electrónico
- Marcar como spam
- Marcar como no spam
- Agregar contacto
- Eliminar contacto
- Bloquear remitente
- Desbloquear remitente


</details>

<details>

  <summary>Seguridad</summary>
  
- Autenticar usuario
- Autorizar acceso
- Denegar acceso
- Bloquear cuenta
- Desbloquear cuenta
- Cambiar permisos
- Asignar roles
- Revocar acceso
- Restringir acceso
- Habilitar two-factor
- Deshabilitar two-factor
- Generar token
- Verificar token


</details>

<details>

  <summary>Administración</summary>
  
- Crear usuario
- Editar usuario
- Eliminar usuario
- Asignar permisos
- Revocar permisos
- Crear grupo
- Editar grupo
- Eliminar grupo
- Asignar roles
- Revocar roles
- Crear perfil
- Editar perfil
- Eliminar perfil
- Asignar configuración
- Revocar configuración


</details>

<details>

  <summary>Reportes </summary>
  
- Generar informe
- Ver informe
- Imprimir informe
- Exportar informe
- Importar informe
- Filtrar informe
- Ordenar informe
- Agrupar informe
- Detallar informe
- Resumir informe


</details>

<details>

  <summary>Integración</summary>
  
- Conectar a API
- Desconectar de API
- Autenticar con OAuth
- Autorizar con OAuth
- Realizar solicitud HTTP
- Recibir respuesta HTTP
- Procesar respuesta HTTP
- Integrar con terceros
- Conectar a servicio web
- Desconectar de servicio web


</details>

[Volver al índice](#id0)

# Si te fue útil

- Comenta a otros sobre esta wiki.
- Comparte.
- Sumate a Under Test! 

## Contacto 

[**Lucas del Reguero Martinez**](https://www.linkedin.com/in/lucas-del-reguero-martinez/)











<style>
  .tabs-container {
    max-width: 600px;
    margin: auto;
    font-family: Arial, sans-serif;
    text-align: center; /* Centrar los elementos dentro del contenedor */
  }

  .tabs-labels {
    display: flex;
    justify-content: center; /* Centra las solapas horizontalmente */
    margin-bottom: -1px; /* Asegura que no haya espacio entre las solapas y el contenido */
  }

  /* Ocultar todas las secciones de contenido por defecto */
  #content1, #content2 {
    display: none;
  }

  /* Mostrar la sección de contenido correspondiente a la solapa seleccionada */
  #tab1:checked ~ .tab-content #content1,
  #tab2:checked ~ .tab-content #content2{
    display: block;
  }

  /* Estilo básico para las solapas */
  label {
    cursor: pointer;
    padding: 10px 20px;
    border-radius: 5px 5px 0 0;
    margin-right: 5px;
    display: inline-block;
  }

  label:last-of-type {
    margin-right: 0; /* Elimina el margen derecho del último label */
  }

  label:hover {
    background: #005fa3;
  }

  /* Estilo para la solapa activa */
  input[type="radio"]:checked + label {
    background: #005fa3;
  }

  /* Estilo para el contenido de las solapas */
  .tab-content {
    border: 1px solid #ddd;
    padding: 20px;
    border-radius: 0 5px 5px 5px;
    background: #f9f9f9;
    text-align: left; /* Alinear el contenido a la izquierda */
    color: black; /* Color de texto negro */
  }

  /* Estilo para solapa 1 (rojo) */
  #tab1:checked + label {
    background: #4caf50; /* Rojo */
    color: white; /* Texto blanco */
  }

  /* Estilo para solapa 2 (verde) */
  #tab2:checked + label {
    background: #ff4d4d; /* Verde */
    color: white; /* Texto blanco */
  }

  /* Ajustes adicionales para la estética */
  input[type="radio"] {
    display: none;
  }
</style>
