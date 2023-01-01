# 01 - Introtrucción


## Introducción al curso

Bienvenidos al curso <nombre del curso>, este curso te va a servir para dominar la herramienta Terraform para Infraestructura
como Código, este curso es para cualquier persona que quiera añadir esta herramienta a sus conocimientos sobre la filosofia DevOps,
no se esperan conocimientos al respecto ya que se cubriran todos los aspectos de esta herramienta partiendo de 0.

Aunque progresemos desde lo más básico hasta conceptos avanzados, si que se requierien ciertas nociones sobre programación,
conocimientos basicos sobre Git en Github y alguna idea sobre los recursos disponibles en la Cloud de Google.

Si en algún momento teneis dudas, no dudeis en usar el sistema de comunicación de la plataforma o en mi correo personal.


## Recursos de aprendizaje: Repositorio/s, que contienen, cómo usarlos y cual es la Arquitectura de referencia

En la siguiente sección o más abajo podreis encontrar los enlaces a los distintos repositorios con los recursos para este curso.
El contenido de estos repositorios está estructuro por capitulos y sigue el mismo orden y agrupacón que el de este curso. Sentiros libres
de abrir sugerencias o de forkear el propio repositorio, Terraform y su ecosistema está en constante crecimiento, ahora que formais parte
de la comunidad vosotros también podeis hacer crecer el proyecto con vuestra perspectiva, así que mojaros.


## Contenido/Indice

A continuación voy a hacer un pequeño resumen sobre todos los modulos de este curso para dejar una idea clara de su estructura y
evolución de los contenidos.

Básicamente explicar que se empezará desde conceptos basicos y por lo tanto muy sencillos hasta conceptos más avanzados como pueden
ser la creación de providers/plugins propios con Golang.

Terraform es una herramienta de infraestructura como código (IAC) que permite a los usuarios definir y provisionar la infraestructura de TI de manera sencilla y reproducible. Con Terraform, puedes usar código para crear, cambiar y mejorar la infraestructura de forma segura y predecible. Terraform es compatible con una amplia gama de proveedores de infraestructura, incluyendo AWS, Azure, GCP y muchos más. Es muy útil para automatizar tareas de configuración y gestión de la infraestructura, lo que ahorra tiempo y reduce el riesgo de errores humanos.


## Explicación de Infraestructura como Código

Aqui hay que explicar la problematica y porque hemos llegado a este punto. Mantener un centro de datos nunca ha sido tarea facil, muy caro,
hace falta conocimiento muy especifico, no escala de forma natural, meta facturas (electricidad sobre todo debidas a la refrigeración).

Por lo que hace años que hemos dejado atras el hecho de tener a nuestro alcance el servidor que está manteniendo nuestras aplicaciones y servicios, ahora todo esta en la ya más que conocida Nube o Cloud.

Si dejas de necesitar un servidor puedes destruirlo con un solo click, si necesitas mucho más recursos en un pico de demanda puedes
escalar tu flota con ciertos grados de automatismo. Todo se puede proveer con el uso de una simple API y veremos como esto lo que está haciendo tERRAFORM basicamente, solo que lo hace de una forma excelente.

Aqui comentar quizas que es posible hacerlo desde una interfaz, pero es muy time consuming, también a traves de una /API/CLI.

Cuando quieres desplegar un proyecto en producción, lo razonable es que por debajo se esten gestionando distintos entornos de preproducción
o staging, confiar en opciones como las anteriores asume que no vas a cometer ningún fallo al replicarlo de forma manual, eso es un error,
somos humanos y equivocarnos es lo nuestro, aquí es donde juega un gran rol IaC y en este caso terraform, se puede definir todo con 
modulos de forma que desplegar recursos en distintos entornos sea una simple replica de la definición de un tipo de recurso o una
combinación de ellos.

Entonces, en resumen que es IaC?  TODO



## ¿Qué es Terraform?

Segun HashiCorp Terraform es una herramienta para construir, cambiar y versionar infraestructura de forma segura y eficiente.

Terraform es una herramienta que te permite crear infraestructura en la Cloud a partir de ficheros de configuración personalizados con el
lenguaje Terraform HCL, un lenguaje creado por HashiCorp y con backend basado en Golang que marca la diferencia con el resto de 
herramientas para IaC por su comprension y facilidad de lectura frente a los clasicos del campo como son YAML o JSON.

Mienta HCL se crean los distintos modulos que representan recursos en diferentes proveedores Cloud


Aqui sería el momento para exponer distintas alternativas a terraform que también pueden estar muy bien, diferenciar también cuales son
Cloud Specific (CF, GCP DM, Azure RM)y cuales son Cloud Agnostic.

Aqui estamos dando una herramienta que aprieta y afloja todo tipo de tornillos. Es bueno conocer una herramienta a la que no le importa
para que proveedor trabaja.
