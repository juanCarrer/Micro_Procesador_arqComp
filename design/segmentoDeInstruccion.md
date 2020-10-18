# Segmento de instrucción
###### La longitud de instrucción es de 16 bits

- # NOP
####  Operación burbuja
```
0000 0000 0000 0000
```

***

- # SUMA
####  Suma el contenido de dos direcciones 
```
 0001 - Resultado(dirección archivo registro) - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
0001 0000 0001 0111 
```

***

- # RESTA
####  Resta el contenido de dos direcciones
```
 0010 - Resultado(dirección archivo registro) - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
0010 0110 0101 1000 
```

***

- # LOAD
####  Carga el contenido de una dirección en memoria principal al archivo de registro
```
 0011 - dirección(archivo de registro) - dirección(memoria principal) - 0000
```
#####  Ejemplo
```
0011 0110 0101 0000
```

***

- # STORE
####  Guarda el contenido de una dirección del archivo de registro en memoria principal
```
 0100 - dirección(archivo de registro) - dirección(memoria principal) - 0000
```
#####  Ejemplo
```
0100 0010 1101 0000
```

***

- # AND
#### Realiza la operación AND 
```
 0101 -- Resultado(dirección archivo registro) - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
0101 1010 0000 0110
```

***

- # OR
#### Realiza la operación OR 
```
 0110 -- Resultado(dirección archivo registro) - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
0110 1000 1010 1110
```

***

- # NOT
#### Realiza la operación NOT 
```
 0111 -- Resultado(dirección archivo registro) - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
0111 1011 1110 1000
```

***

- # JZ
#### Realiza un salto en el PC si la suma de los operandos es 0
```
 1000 -- numero de saltos del PC - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
1000 0001 1110 1000
```

***

- # JN
#### Realiza un salto en el PC si la suma de los operandos es negativa
```
 1001 -- numero de saltos del PC - operando1(dirección archivo de registro) - operando2(dirección archivo de registro) 
```
#####  Ejemplo
```
1001 1001 1100 1010
```