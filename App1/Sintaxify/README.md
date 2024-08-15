# Sintaxify

## Resumen y Justificación

**Sintaxify** es una aplicación web diseñada para simplificar el análisis sintáctico de gramáticas formales, una tarea fundamental en el estudio de lenguajes formales y compiladores. La herramienta permite a los usuarios ingresar gramáticas, realizar la derivación más a la izquierda, calcular los conjuntos de primeros y siguientes, y construir la tabla M. Con esta información, Sintaxify facilita un análisis sintáctico descendente paso a paso para reconocer cadenas de entrada, proporcionando una plataforma interactiva y práctica para estudiantes y profesionales. Este proyecto es especialmente útil para egresados y estudiantes de ciencias de la computación, ya que les permite profundizar su comprensión y práctica en estos conceptos clave.
Actualmente Sintaxify solo realiza recursividad para las producciones de tipo E->E, por lo que se espera que se realice un seguimiento a futuro para que se apliquen todas las recursividades .

Justificaciones:
1.Facilitación del Aprendizaje:

Sintaxify proporciona una plataforma interactiva donde los estudiantes pueden practicar y visualizar el proceso de análisis sintáctico. Esto hace que conceptos abstractos y complejos sean más accesibles y comprensibles.

2.Herramienta de Referencia:

Para los profesionales, Sintaxify sirve como una herramienta de referencia rápida para la verificación de gramáticas y la construcción de tablas M, ahorrando tiempo y reduciendo errores en la fase de diseño de compiladores y parsers.

3.Refuerzo de Conocimientos:

La posibilidad de realizar análisis sintáctico paso a paso permite a los usuarios consolidar su comprensión de los algoritmos de parsing, cruciales en cursos de teoría de la computación y diseño de compiladores.

4.Preparación Profesional:

Sintaxify ayuda a preparar a los estudiantes para roles técnicos avanzados, ya que el análisis sintáctico es una habilidad fundamental en el desarrollo de lenguajes de programación y herramientas de software relacionadas.

5.Acceso Universal y Colaborativo:

Como una aplicación web, Sintaxify es accesible desde cualquier lugar, facilitando la colaboración entre estudiantes y profesionales. Su naturaleza abierta fomenta el aprendizaje compartido y el intercambio de conocimientos.
## Pasos para Ejecutarla

1. Clonar el Repositorio de GitHub:

* Abre tu terminal.
* Clona el repositorio usando el siguiente comando:
git clone https://github.com/proyectosingenieriauninorte/Sintaxify.git

* Navega al directorio del repositorio clonado:
cd Sintaxify

2. Abrir el Programa:

* Abre el archivo HTML principal en tu navegador, se encuentra en la carpeta principal 
* Por ejemplo:
open index.html
* Alternativas si estás en un entorno Linux:
xdg-open index.html

3. Ingresar el Contenido a Modificar:

* En la interfaz de la página web, localiza el campo de entrada para ingresar las producciones gramaticales.

* Ingresa las producciones en el formato adecuado, por ejemplo:
E -> E+T | T
T -> T*F | F
F -> (E) | id
Nota: Hay que tener en cuenta que la calculadora unicamnete realiza derivaciones cuando la recursividad es de tipo E->E
4. Ver el Resultado:

* Presiona el botón "Transformar Gramática" para procesar las producciones gramaticales.
* Observa el resultado mostrado en la página, que puede incluir las producciones transformadas, el cálculo de los conjuntos FIRST y FOLLOW, etc.

5. Ingresar el Contenido Modificado:

* Si el programa te proporciona contenido modificado o producciones transformadas, cópialo de la sección de resultados.

* Ingresa este contenido modificado en el campo de entrada nuevamente para realizar más transformaciones o cálculos adicionales

6. Ver los Resultados en Formato de Tabla:

* Presiona el botón correspondiente para visualizar los resultados en formato de tabla. Este botón puede llamarse "Ver en Tabla" o algo similar.

* Revisa los resultados mostrados en formato de tabla en la página.


Realizado por:
Nathalia de la Rans
Miguel Garcia
Juan Pineda
Esteban Ramírez
