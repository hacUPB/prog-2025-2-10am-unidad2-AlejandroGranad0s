# Actividad de repaso

1. Explica, en tus propias palabras, por que es necesario que las computadoras representen los datos en binario.

    Representar los datos con el sistema binario es mas eficiente para las computadoras, ademas este sistema permite representar los datos de una manera mas facil. lo que favorece a las computadoras al momento de procesar la informacion

2. Convierte el numero binario 10011011 a decimal y a hexadecimal.
a decimal - 155
a hexadecimal - 9B

4. Investiga y describe como se representa una imagen en formato PNG en el disco.

    Una imagen se representa en el disco como una secuencia de datos estructurados en bloques, donde cada bloque contiene informacion especifica sobre la imagen. Estos bloques incluyen metadatos, datos de imagen comprimidos, entre otros.

5. Analiza la siguiente situacion: Que sucede si intentas almacenar un numero mayor al que puede representar un byte (por ejemplo, 300)? Como lo maneja Python?

Un *byte* solo puede almacenar valores entre *0 y 255, ya que tiene **8 bits* (2⁸ = 256 posibles valores).

### En Python:

Los enteros (int) de Python *no tienen un límite fijo*, así que puedes trabajar con números grandes sin problema.

Sin embargo, si usas estructuras que simulan bytes, como bytes o bytearray, *sí hay restricciones*:

python
bytes([300])
# Resultado: ValueError: bytes must be in range(0, 256)

Para representar 300 correctamente en *más de un byte*, puedes usar el método to_bytes:

python
n = 300
b = n.to_bytes(2, byteorder='big')
print(b)  # Resultado: b'\x01,'


Aquí, 300 se guarda usando *2 bytes*, donde:
- \x01 representa 256
- \x2C representa 44
- En conjunto: (256×1) + 44 = *300*
