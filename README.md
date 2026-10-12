# Proyecto-QA_Canva
Pruebas funcionales para la creación y edición de diseños en Canva
## 1. INFORMACION GENERAL
- Nombre del proyecto: pruebas funcionales para la creación y edición de diseños en Canva
- Especialidad: QA
- Fuente del proyecto: Canva- Aplicación Web

## 2. OBJETIVO
Flujo principal de Usuario: 

Crear un diseño → seleccionar una plantilla → editar elementos → agregar/eliminar páginas → guardar cambios→ descargar/compartir.

Validar que un usuario pueda crear y personalizar un diseño utilizando una plantilla, gestionar sus páginas, conservar correctamente los cambios y compartir o descargar el resultado sin errores que afecten su experiencia. 

¿Qué riesgo o bug se busca prevenir con el plan de pruebas?
El riesgo principal sería que un usuario pierda cambios, no pueda completar correctamente su diseño o que comparta o descargue un resultado diferente al esperado. 

## 3. PLAN DE TRABAJO 
El proyecto evaluará la calidad funcional del flujo de creación, edición, gestión, colaboración y exportación de diseños en Canva utilizando una cuenta gratuita. Las pruebas estarán enfocadas en plantillas gratuitas y en funcionalidades disponibles sin suscripción Pro. Se validará el comportamiento de los principales flujos de usuario, la conservación de cambios, los permisos de acceso mediante enlace y la integridad de los archivos descargados.

# 3.1. Exploración inicial
**Análisis de requisitos.**

**_A.	Creación de diseño_**

El Usuario debe poder iniciar un nuevo diseño desde Canva y acceder al editor correspondiente

**_B.	Selección de Plantilla_**

El Usuario debe poder buscar y seleccionar una Plantilla disponible y abrirla en el editor para personalizarla (Personalizar Plantilla)

**_C.	Edición de contenido_** 

El usuario debe poder modificar los elementos editables de la plantilla, incluyendo texto y otros elementos disponibles 

**_D.	Gestión de pagina_** 

El Usuario debe poder agregar, duplicar y eliminar páginas del diseño

**_E.	Conservación de cambios_**

Después de realizar las modificaciones, los cambios deben conservarse cuando el usuario vuelva a acceder al diseño

**_F.	Compartir diseño_**

El Usuario debe poder compartir su diseño y seleccionar diferentes niveles de acceso, como ver, comentar o editar, según las opciones disponibles para su cuenta.

**_G.	Descarga_**

El usuario debe poder descargar el diseño utilizando una opción de formato disponible para su diseño.

**_H.	Restricciones de permisos_** 

Cuando un diseño sea compartido con permisos limitados, el usuario receptor no debería poder realiza acciones que no correspondan al permiso otorgado (ver, comentar, editar)


# 3.2. Preparación
*Áreas principales del proyecto:*

**1.	Creación y edición** 

•	Crear diseño 

•	Seleccionar plantilla 

•	Editar textos 

•	Editar elementos 

•	Agregar páginas

•	Duplicar páginas 

•	Eliminar páginas 

**2.	Permanencia y colaboración**

•	Verificar que los cambios se guardan

•	Compartir

•	Generación de un enlace

•	Permisos de ver 

•	Permisos de comentar

•	Permisos de editar

**3.	Exportación**

•	Descargar

•	Seleccionar formato

•	Validar archivo descargado 

•	Validar contenido 

•	Validar textos

•	Validar elementos

•	Validar páginas

_Diseño de casos de prueba disponibles en Excel._

# 3.3. Construcción
_Ejecución de pruebas documentadas en Excel._

# 3.4. Evaluación

| Funcionalidad | Resultado Observado | 
| ------------ | ------------ | 
| Crear diseño| El diseño puede crearse correctamente| 
| Selección de plantilla| Se puede seleccionar una plantilla gratuita| 
| Abrir la plantilla en editor| La plantilla se abre correctamente| 
| Modificar textos| Los textos disponibles pueden modificarse| 
| Modificar elementos| Los elementos disponibles pueden modificarse| 
| Agregar páginas| Se pueden agregar páginas| 
| Duplicar páginas| Se pueden duplicar paginas| 
| Eliminar paginas| Se pueden eliminar páginas| 
| Conservar cambios | Los cambios permanecen después de salir y volver al diseño| 
| Compartir diseño| Se puede compartir mediante varias opciones| 
| Compartir mediante enlace| Se puede generar un enlace| 	
| Permisos de enlace| Se identificaron permisos para ver, comentar o editar| 
| Descargar diseño| Disponible para cuenta gratuita| 
| Descargar en diferentes formatos| Jpg, png, pdf, mp4, gif, y pptx disponibles según el diseño| 
| Integridad del archivo descargado| El contenido corresponde al diseño realizado | 
| Conservación de páginas en descarga| Las páginas se mantienen correctamente| 
 	
## 4. PREGUNTAS CLAVE
_**4.1. ¿Qué impacto tendría en el usuario la pérdida de los cambios realizados en un diseño de Canva?**_
Es importante poder validar que las modificaciones se conserven al salir del editor, volver a abrir el diseño o al experimentar interrupciones en la conexión.

_**4.2. ¿Qué riesgos de seguridad y privacidad podrían presentarse si los permisos de acceso no funcionan correctamente?**_ 
Un usuario con permisos de solo visualización no debería de poder realizar acciones reservadas para usuarios con permisos superiores. Una configuración incorrecta podría comprometer la integridad del diseño. 

_**4.3 ¿Qué consecuencias tendría que los archivos exportados no conservaran el contenido o la estructura del diseño original?**_
Una exportación incorrecta podría afectar la utilidad del archivo y generar inconvenientes para los usuarios que necesitan compartirlo o utilizarlo fuera de Canva.

## 5. QUÉ SE HIZO Y COMO
Se analizó el flujo de creación y gestión de diseños de Canva, identificando sus principales funcionalidades y definiendo el alcance de las pruebas desde una cuenta gratuita.
A partir de estos requisitos funcionales, se diseñaron 27 casos de prueba para validar la creación de diseños, edición de textos y elementos gráficos, gestión y conservación de páginas y cambios, permisos de acceso y exportación o descarga de los diseños.
Se ejecutaron pruebas positivas para comprobar el funcionamiento esperado y pruebas negativas para verificar las restricciones de acceso y el comportamiento ante distintas configuraciones o permisos. Los casos se documentaron con sus precondiciones, pasos a reproducir, resultados esperados y, seguidamente, se ejecutaron las pruebas para comparar el comportamiento observado con el esperado, documentándose así los resultados encontrados. 

_**Herramientas y técnicas:**_ Pruebas funcionales manuales, diseños de casos de prueba, validación de escenarios positivos y negativos, matriz de ejecución y documentación de evidencias.

## 6. RESULTADOS
Se diseñaron y ejecutaron 27 casos de prueba funcionales sobre Canva, enfocados en la creación y edición de diseños, gestión de páginas, conservación de cambios, permisos de acceso y exportación de archivos. 
La ejecución permitió evaluar el comportamiento de las funcionalidades incluidas en el alcance del proyecto y comparar los resultados obtenidos con los resultados esperados.
Los resultados se consolidaron en una matriz de pruebas para identificar los casos aprobados, los casos fallidos y las posibles incidencias que requirieran seguimiento

*Indicadores de ejecución.*

Casos de prueba diseñados: **_27_**

Casos de prueba ejecutados: **_27_**

Casos aprobados: **_27_**

Casos fallidos: **_0_**

Defectos identificados: **_0_**

## 7. CONCLUSIONES
Este proyecto permitió aplicar el proceso de pruebas de software a una aplicación web y digital utilizada para la creación y edición de diseños, desde la identificación de requisitos funcionales hasta el diseño, la ejecución y la documentación de casos de prueba. 
Durante el proceso, reforcé mis habilidades para analizar flujos de usuario, identificar escenarios positivos y negativos, definir resultados esperados y evaluar el comportamiento de una aplicación frente a diferentes condiciones de uso.
A su vez, también comprendí la importancia de validar no solo el desempeño de las funcionalidades principales, sino aspectos como la persistencia de la información, los permisos de acceso y la integridad de los archivos exportados. 
Como mejora futura, ampliaría las pruebas a otros navegadores, dispositivos y condiciones de conectividad, e incorporaría pruebas de accesibilidad y automatización para reducir el esfuerzo de regresión. 
En una entrevista, destacaría mi capacidad para transformar requisitos funcionales en casos de prueba estructurados, documentar resultados y evaluar la calidad de un producto desde la perspectiva del usuario.


