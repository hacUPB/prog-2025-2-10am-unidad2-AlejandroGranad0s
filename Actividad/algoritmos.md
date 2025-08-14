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
<img width="713" height="773" alt="Diagrama sin título drawio" src="https://github.com/user-attachments/assets/0b295b01-8c76-4731-b6e5-1107c52fc886" />

## Actividad

Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

|variables|tipo|comentario|
|---------|----|----------|
|total_compra|Entrada|valor de la compra|
|Descuento | Salida|descuento segun la compra|
|precio_final| Salida| Valor a pagar|
|15%, 8%, $250000| Constantes| Descuentos y valor limite|

```
Inicio
Leer total_compra
Si total_compra > 250000:
  descuento = total_compra * 0.15
Si no
  descuento = total_compra * 0.8
Fin si
Precio_final = total_compra - descuento
Escribir "El valor total es: ", precio_final
Fin
 ```

## Actividad

El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

|variables|tipo|comentario|
|---------|----|----------|
|alumnos|Entrada|valor de la compra|
|costo_alumnos | Salida|descuento segun la compra|
|costo_total| Salida| Valor a pagar|
|100,$65,50-99,$70,30-49,$95,1-30,$4000| Constantes| Datos|

```
Inicio
Leer alumnos
Si alumnos >= 100:
  costo_alumnos = $65
Si no
  Si alumnos >= 50
    costo_alumnos = $70
  Si no
     Si alumnos >= 30
       costo_alumnos = $95
     Si no
       costo_total = $4000
       costo_alumno = costo_total/alumnos
     Fin si
  Fin si
Fin si
Escribir "El valor total es: ", costo_alumnos
Fin
 ```
## Tarea
calcular la edad segun el año de nacimiento y el actual

|variables|tipo|comentario|
|---------|----|----------|
|dia|Entrada|nacimiento|
|mes|Entrada|nacimiento|
|año|Entrada|nacimiento|
|dia|Entrada|actual|
|mes|Entrada|actual|
|año|Entrada|actual|
|edad actual| Salida|edad actual|


```
Inicio
    // Solicitar datos de nacimiento
    Escribir "Ingrese su día de nacimiento (Diaa):"
    Leer Diaa
    Escribir "Ingrese su mes de nacimiento (Mesa):"
    Leer Mesa
    Escribir "Ingrese su año de nacimiento (Añoa):"
    Leer Añoa

    // Solicitar fecha actual
    Escribir "Ingrese el día actual (Diab):"
    Leer Diab
    Escribir "Ingrese el mes actual (Mesb):"
    Leer Mesb
    Escribir "Ingrese el año actual (Añob):"
    Leer Añob

    // Calcular edad básica
    Edad-actual = Añob - Añoa

    // Verificar si ya cumplió años este año
    Si Mesa > Mesb Entonces
        Edad-actual = Edad-actual - 1
    Sino
        Si Mesa == Mesb Entonces
            Si Diaa > Diab Entonces
                Edad-actual = Edad-actual - 1
            FinSi
        FinSi
    FinSi

    // Mostrar resultado
    Escribir "La edad actual es:", Edad-actual
Fin
```
<img width="586" height="852" alt="tarea edad drawio" src="https://github.com/user-attachments/assets/e9fd8839-2435-4fbb-a1ee-27757ebc730b" />


# Bucles
## ejercicio 1

Se requiere un algoritmo para determinar, de N cantidades, cuantas son cero, cuantas son menores a cero, y cuantas son mayores a cero.
REalice el diagrama de flujo y el pseudo codigo 
representarlo, utilizando el ciclo apropiado.

```
inicio
leer N
ceros = 0
mayores = 0
menores = 0
Mientras N > 0:
     Leer cant
     Si cant > 0:
         mayores = mayores + 1
     Si no
         Si cant = 0:
              ceros = ceros + 1
         Si no
              menores = menores + 1
         Fin si
     Fin si
     N = N - 1
Fin Mientras
Escribir ceros, mayores, menores
Fin
```

## ejercicio 2

hallar el factorial de un numero

```
inicio
Leer N
i = 1
mientras N > 0:
     si N = 0:
        i = i
     si no
         i = i*N
         N = N - 1
Fin mientras
Escribir "el factorial es:", i
Fin
```

## tarea 1

tarjeta de credito

|variables|tipo|comentario|
|---------|----|----------|
|valor_compra|Entrada|cantidad de lapices|
|numero_cuotas| Entrada|precio total de lapices|
|cuota|  Salida| Valor unitario de la caja|
|tasa_interes| Constantes| No cambian|

```
Inicio
    tasa_interes = 0.02 
    valor_compra = 0
    numero_cuotas = 0
    cuota = 0

    Leer valor_compra

    Leer numero_cuotas

    cuota = (valor_compra * (1 + tasa_interes)) / numero_cuotas

    Escribir "El valor de cada cuota es: ", cuota
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
