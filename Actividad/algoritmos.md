# Pseudocodigo

## Ejercicio 1

[Simbolos de diagrama de flujo](https://www.smartdraw.com/flowchart/simbolos-de-diagramas-de-flujo.htm)
![text](Captura%20de%20pantalla%202025-07-31%20104622.jpg)

## Ejercicio 2

Ingreso total semestral 

### Solucion 

```
Inicio
Leer ID, S1, S2, S3, S4, S5, S6
Total = S1 + S2 + S3 + S4 + S5 + S6
Promedio = Total/6
Escribir ID, Total, Promedio
FIn
 ``` 

![text](Diagrama%20flujo.drawio.png)

## Tarea

Curso se evalua con 7 notas, se conoce 6 notas y vale el 70% de la nota
Calcular cuanto debe sacar en la evaluacion final para aprobar con 3.0

```
Inicio
Leer N1, N2, N3, N4, N5, N6
Promedio = N1+N2+N3+N4+N5+N6 / 6
Total = ((Promedio * 0.7) - 3.0 )/ 0.3
Escribir Total
FIn
 ``` 
<img width="413" height="600" alt="image" src="https://github.com/user-attachments/assets/1d5892ec-1229-4f54-b72e-173cee262955" />


## Actividad

Realizar un algoritmo para determinar cuanto se debe pagar por equis cantidad de lapices considerando que si son 1000 o mas el costo es de $85 
cada uno. de lo contrario el precio es de $90. representar con el psudocodigo y el diagrama de flujo

|variables|tipo|comentario|
|---------|----|----------|
|lapices|Entrada|cantidad de lapices|
|precio | Salida|precio total de lapices|
|valor_unidad| Intermedia| Valor unitario de la caja|
|85, 90| Constantes| No cambian|

```
Inicio
Leer lapices
Si lapices >= 1000:
  valor_unidad = 85
Si no
  valor_unidad = 90
Fin si
Precio = lapices * valor_unidad 
Escribir "El valor total es: ", precio
Fin
 ``` 


### Parte 1: Identificar Algoritmos

Responde si los siguientes enunciados representan un algoritmo. Justifica la respuesta:

1. Una página web.
2. Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir.
3. "Piensa en un número y multiplícalo por otro".
4. Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro.
5. Una lista de compras organizada en orden alfabético

### Parte 2: Variables y Constantes

Indica si las siguientes afirmaciones describen una variable o una constante:

1. El valor de la gravedad en la Tierra, 9.8 m/s².
2. La edad de una persona calculada con base en el año actual y su año de nacimiento.
3. La cantidad de dinero en una cuenta bancaria.
4. La velocidad de la luz en el vacío, 299,792,458 m/s.
5. El radio de un círculo.

### Parte 3: Características de los Algoritmos

Responde si los siguientes enunciados cumplen con las características de un algoritmo. Justifica la respuesta:

1. Para elegir la ruta más corta entre varias ciudades, el algoritmo examina rutas candidatas, deteniéndose cuando los cambios en la distancia parecen lo suficientemente pequeños.
2. Suma los números ingresados y muestra el resultado.
3. Un conjunto de pasos para calcular el área de un rectángulo dado su base y altura.
4. El algoritmo cuenta el número de votos obtenidos por cada uno de los candidatos de una elección para presidente. Empieza solicitando el nombre del candidato y finaliza cuando se ingresa el valor -1.

### Parte 4: Comprensión de Herramientas

Indica si las siguientes afirmaciones son ciertas o falsas respecto al pseudocódigo y diagramas de flujo:

1. El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas.
2. Los diagramas de flujo son una representación gráfica de un algoritmo.
3. El pseudocódigo debe estar escrito en un lenguaje de programación específico.
4. Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos.

### Parte 5: Estructuras de Control

Describe para qué sirven las estructuras de control. Redacta dos ejemplos, uno de tu vida diaria, es decir cuando tienes que tomar decisiones en tus actividades diarias y oto ejemplo en el que se tengan que utilizar cálculos matemáticos para tomar una u otra decisión.
