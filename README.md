# 1. Objetivos
El presente proyecto tiene por objeto enfrentar a los estudiantes del curso:
1. A la construcción de aplicativos webs para resolver problemas.
2. Al uso de los algoritmos vistos en clase.
3. Al diseño e implementación de soluciones correctas y eficientes a problemas computacionales,
usando los conceptos vistos en clase.
# 2. Definición de la Tarea

![image](https://github.com/ioaNN2394/ProyectoEDYA/assets/114038390/e2e80ac3-e5ad-472b-bc6a-be0837fe1632)
Figura 1

Tomando como referencia el ejercicio que hemos denominado Tablero de resultados (mostrado en
la Figura 1)1
, construir una solución al ejercicio en el cual se aplicarán las siguientes
modificaciones:
 Solo se procesará un único caso.
 La entrada del caso estará compuesta por m submissions. Su formato será el siguiente:
submission1; submission2; ….; submissionm
 Teniendo en cuenta que hay n contest (1≤n≤100), p problems (1≤p≤9), la entrada de cada
submission mantiene el formato:
contest problem time L
Donde constest es una cadena iniciada con Team y seguida del número correspondiente.

# Ejemplo:

si la entrada es:
'Team1 1 5 C;Team2 5 10 C;Team3 2 15 I;Team1 3 20 R;Team2 1 25 R;Team2 4 30
C;Team1 3 35 I;Team1 3 40 C;Team3 2 45 I;Team3 2 50 C'

 El scoreboard se calcula aplicando los siguientes criterios:
o Ordenamiento descendentemente por el número de problemas resueltos
(problemsSolved) - criterio1.
o Ordenamiento ascendentemente por el tiempo de penalización (penaltyTime) -
criterio2.
o Ordenamiento ascendentemente por el contest (criterio3).
Por lo cual cada línea del scoreboard debe mantener el siguiente formato:
contest problemsSolved penaltyTime


 La solución obligatoriamente debe tener una función en JavaScript denominada
calcularScoreBoard(caso) (escrita en el archivo util.js) que recibe el caso y produce una
sola cadena con el formato indicado para la salida.
Ejemplo: Si la variable caso se corresponde a la cadena del ejemplo anterior, la cadena
retornada por calcularScoreBoard(caso) será:
'Team2 2 40
Team1 2 65
Team3 1 90'

Observación: La nota obtenida depende de la correctitud de su algoritmo y eficiencia, con relación
a las soluciones de los demás grupos y una solución generada por el docente. 
