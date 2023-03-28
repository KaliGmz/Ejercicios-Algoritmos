# EJERCICIOS CON ALGORITMOS

## Resto de Ejercicios 

### Ejercicio 1
Calcular la letra de DNI Español
**Paso 1** : Definir el problema : a partir de un numero de DNI calcular la letra.  ¿Como se calcula la letra del DNI?

Numero DNI  dividirlo en 23 y el resto será el resultadoResto

El resultadoResto compararemos con la lista de códigos de la siguiente lista 



| resultadoRestado | Letra |
| ---------------- | ----- |
| 0                | T     |
| 1                | R     |
| 2                | W     |
| 3                | A     |
| 4                | G     |
| 5                | M     |
| 6                | Y     |
| 7                | F     |
| 8                | P     |
| 9                | D     |
| 10               | X     |
| 11               | B     |
| 12               | N     |
| 13               | J     |
| 14               | Z     |
| 15               | S     |
| 16               | Q     |
| 17               | V     |
| 18               | H     |
| 19               | L     |
| 20               | C     |
| 21               | K     |
| 22               | E     |



**Paso 2** : Poner la entrada, el proceso y la salida

Entrada:  DNI y tablaLetrasDNI

Proceso: 

- ​	Validar que el DNI tenga 8 dígitos y numéricos
  - Si es errónea asigne a la variable resultado "DNI Invalido"
- ​    Dividimos DNI en 23 y el resto asignar a resultadoResto
- ​	Comparar el resultadoResto con los valores de la tabla, asignar a          	letraDNI el valor equivalente en la tabla

Salida

- Escribir resultado 

**Paso 3** : Escribir el pseudocódigo

```
Algoritmo CalculoDNI
   # Entrada
   DNI<-leer()
   tablaLetrasDNI<-"TRWAGMYFPDXBNJZSQVHLCKE"
   resultado<-""
   # Proceso
   si DNI es valido Entonces
   		resultadoResto<-DNI mod 23 #mod es el resto de dividir
   		resultado<-recuperarLetra(resultadoResto,tablaLetrasDNI)
   sino 
   		resultado<-"DNI invalido"
   
   Fin si
   Escribir(resultado)
   # Salida
Fin Algoritmo
```



### Ejercicio 2

**Paso 1** : Definir el problema
Calcular el salario de un empleado
El salario en España se calcula a partir del salario bruto anual, que incluye todas las percepciones economicas que recibe un trabajador durante el año, inlcuyendo salario base, pagas extras, complementos y otros conceptos retributivos.

**Paso 2** : Poner la entrada, el proceso y la salida
Entrada: salario base, pagas extras, complementos, otrosConceptosRetributivos

IRPF, Seguridad Social

Proceso:

- ​		Sumar salarioBase, pagasExtras, complementos, otrosConceptosRetributivos y lo asigno a salarioBruto
- Sumar IRP, seguridad Social y lo asigno a deducciones
- salarioNeto asigna salarioBruto - deducciones

Salida:

Escribir(salarioBruto, SalarioNeto)

**Paso 3** : Escribir el pseudocofigo

```
Algoritmo Nomina
   # Entrada
   salarioBase<-Leer()
   pagasExtras<-Leer()
   complementos<-Leer()
   otrosConceptosRetributivos<-Leer()
   IRP<-Leer()
   Seguridad Social<-Leer()
   # Proceso
   salarioBruto<-salarioBase+pagasExtras+complementos+otrosConceptosRetributivos
   deducciones<-IRP+Seguridad Social
   salarioNeto<-SalarioBruto-deducciones
   # Salida
	Escribir(SalarioBruto,SalarioNeto)

Fin Algoritmo
```


### Ejercicio 3

**Paso 1** : Definir el problema

Determinar la ruta para llegar a una ciudad por avión

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: La ubicacion de partida y salida
Proceso: Introducir los datos y buscar si la ruta entre el pais indicado y tambien indicar el medio de transporte que seria avion y ver si esta disponible o no

Salida: La ruta del avion para llegar a una ciudad

**Paso 3** : Escribir el pseudocodigo

```
    Algoritmo ruta
  # ENTRADA:
	Inicio
	ubicacionPartidá ‹- leer()
	ubicacionDestino ‹- leer()
	Fin
	# PROCESO:
	Inicio
	GoogleMaps<-ingresar()
	comoLlegar ‹- seleccionar()
	campoDesde<-ingresar(ubicacionPartida)
	campoHacia ‹- ingresar (ubicacionDestino)
	mediosDeTransporte<-seleccionar("Avión")
	Si ruta ‹-"Error" Entonces
	mostrar mensaje <-"Error. La ruta no está disponible"
		Finalizar programa
	Si no
		Recopilar informaciónRuta(recorrido,escalas,duraclony
	Fin
	salida
	Escribir informacionRuta
	Fin Algoritmo
```


## Resto de ejercicios

### Ejercicio 4

**Paso 1** : Definir el problema
Calcula el área y perímetro de un círculo dado su radio.
Para calcular el área de un círculo, se puede utilizar la fórmula:
 Área = pi * radio^2 . 
Donde "pi" es una constante matemática aproximadamente igual a 3.1416 y "radio" es la distancia desde el centro del círculo hasta cualquier punto del borde.

Para calcular el perímetro de un círculo, se puede utilizar la fórmula:
Perímetro = 2 * pi * radio
Donde nuevamente "pi" es la constante matemática y "radio" es la distancia desde el centro del círculo hasta cualquier punto del borde.

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: Radio del circulo

Proceso: 

- Area= pi multiplicado por el radio dividido entre 2 

- Perimetro= multiplicar radio por pi y por 2

  Salida: 
  Escribir(Perimetro)
  Escribir(areacirculo)

**Paso 3** : Escribir el pseudocofigo

```
Algoritmo Circulo
   # Entrada
	radiocirculo<-leer()
	pi<-leer()
   # Proceso
	area <- pi * radiocirculo / 2
	perimetro <- 2 * pi * radiocirculo

   # Salida
	escribir("El área del círculo es ", area)
	escribir("El perímetro del círculo es ", perimetro)
Fin Algoritmo
```

### Ejercicio 5

**Paso 1** : Definir el problema
Dada una lista de números enteros, determina cuál es el mayor y cuál es el menor.

Al tener números enteros

- Si los dos números enteros son positivos, el mayor es el que tenga mayor valor absoluto.
- Si los dos números enteros son negativos, el mayor es el que tenga menor valor absoluto.
- Si uno de los números enteros es positivo y el otro es negativo, el mayor es el positivo.


**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: leer  lista de numeros enteros
Proceso:  

1. Inicialmente, se toma el primer número de la lista y se considera como el mayor y el menor número.
2. Luego, se recorre toda la lista de números y se compara cada número con el número mayor y menor actual.
3. Si el número actual es mayor que el número mayor actual, se actualiza el número mayor con el número actual.
4. Si el número actual es menor que el número menor actual, se actualiza el número menor con el número actual

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo NumerosEnteros
   # Entrada 
	numeros <- leer()
	# Proceso
	mayor = numeros[0]
	menor = numeros[0]
	para i desde 1 hasta longitud(numeros) - 1 hacer
	si numeros[i] > mayor entonces
		mayor = numeros[i]
	fin si
	si numeros[i] < menor entonces
		menor = numeros[i]
		fin si
	fin para
   # Salida
	escribir <-  "El número mayor es " + mayor
	escribir <- "El número menor es " + menor
	fin
Fin Algoritmo
```

### Ejercicio 6

**Paso 1** : Definir el problema

Crea un algoritmo que convierta grados Celsius a Fahrenheit. ¿Como convertir grados celcius a Fahrenheit? Con operaciones matematicas

**Paso 2** : Poner la entrada, el proceso y la salida
Entrada: Grados celcius
Proceso: Transformar los grados celcius a fahrenheit
Salida: El resultado de convertir grados celcius a fahrenheit

**Paso 3** : Escribir el pseudocofigo

```
Algoritmo Fahrenheit
   # Entrada
	gradoscelcius<-leer()
   # Proceso
	gradosfahrenheit<- (gradoscelcius * 9/5) + 32
   # Salida
	Escribir<-(gradosfahrenheit)
Fin Algoritmo
```

### Ejercicio 7

**Paso 1** : Definir el problema
Dado un número entero, crea un algoritmo que determine si es par o impar. ¿Como saber si un numero es par o impar? Si se le divide para 2 y sale 0 es par sino impar

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: Numero entero

Proceso:

1. Leer el número entero 
2. Calcular el residuo de numero entero dividido entre 2 (residuo)
3. Si residuo es igual a cero, entonces numero entero es par; de lo contrario, numero entero es impar
4. Mostrar el resultado correspondiente (par o impar)

Salida:
Escribir: par o impar 

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo ParoImpar
   # Entrada
	numentero<-leer()
   # Proceso
	residuo<- numentero / 2
	 Si residuo == 0 entonces
        Escribir numentero, "es un número par"
    sino
        Escribir numentero, "es un número impar"
    FinSi
   # Salida
	 escribir<-(residuo)
Fin Algoritmo
```

### Ejercicio 8

**Paso 1** : Definir el problema

Crea un algoritmo que determine si un año es bisiesto o no
Definición estándar de años bisiestos, que son aquellos que son divisibles por 4, excepto los años que son divisibles por 100 pero no por 400.¿Como saber si un año es bisiesto o no? Con operaciones matematicas

**Paso 2** : Poner la entrada, el proceso y la salidaEntrada: Año

Proceso: 

1. Leer el año
2. Si el año es divisible entre 4, continuar con el paso 3, de lo contrario ir al paso 7
3. Si el año es divisible entre 100, continuar con el paso 4, de lo contrario ir al paso 5
4. Si el año es divisible entre 400, ir al paso 6, de lo contrario ir al paso 7
5. El año es bisiesto
6. El año es bisiesto
7. El año no es bisiesto

Salida: Año bisiesto o no



**Paso 3** : Escribir el pseudocofigo

```
Algoritmo AñoBisiesto
   # Entrada
	año<-leer()
   # Proceso
	 Si año % 4 = 0 entonces
    Si año % 100 = 0 entonces
      Si año % 400 = 0 entonces
        Escribir "El año es bisiesto"
      Sino
        Escribir "El año no es bisiesto"
      Fin Si
    Sino
      Escribir "El año es bisiesto"
    Fin Si
  Sino
    Escribir "El año no es bisiesto"
  Fin Si
   # Salida
Fin Algoritmo
```

### Ejercicio 9

**Paso 1** : Definir el problema

Crea un algoritmo que determine si una cadena de texto es un palíndromo o no.
Un palíndromo es una palabra, número o frase que se lee igual al derecho y al revés, es decir, que se puede leer de igual manera de izquierda a derecha que de derecha a izquierda. El algoritmo debe ser capaz de identificar si una cadena de texto dada cumple con esta condición, sin importar si la cadena contiene espacios, signos de puntuación, o si las letras están en mayúsculas o minúsculas.

**Paso 2** : Poner la entrada, el proceso y la salida
Entrada: cadena
Proceso:

1.  Eliminamos los espacios en blanco de la cadena de texto y convertimos todo a minúsculas para que la comparación sea insensible a mayúsculas y minúsculas.
2. Comparamos la cadena de texto original con su versión invertida .
3. Si la cadena original es igual a su versión invertida, entonces el resultado es "Si es palindrimo", indicando que la cadena de texto es un palíndromo.
4.  Caso contrario el resultado es "No es palindromo"

Salida: Escribir es palindromo o no palindromo (resultado)

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo Palindromo
   # Entrada
   cadena <- leer()
   #Proceso
   #cadena <- Convertir a minúsculas y eliminar espacios en blanco
   reversa <- depuracionCadena(cadena)
   Si cadena es igual a reversa entonces
     resultado <- "La cadena es un palíndromo"
   Sino
     resultado <- "La cadena no es un palíndromo"
   Fin Si
   # Salida
   escribir resultado
Fin Algoritmo

SubAlgoritmo depuracionCadena (cadena)
    #quita los espacios en blanco, otros caracteres y convierte todo a minusculas
    i<-0
    Mientras cadena[i] sea diferente de findecadena Haga
        caracter<-""
        Si  el ASCII de cadena[i]  mayor que 64 y ASCII de cadena[i] menor que 91 Entonces
            caracter<-cadena[i] en minusculas
        Fin Si
        Si  el ASCII de cadena[i]  mayor que 96 y ASCII de cadena[i] menor que 123 Entonces
            caracter<-cadena[i]
        End Si
        temporal <- temporal + caracter
        Si caracter es diferente "" Entonces
            i<-i+1
        Fin Si
    Fin Mientras
    L<-i
    reversa<-""
    Para N = 0 Hasta L-1 Con Paso 1 Haga
        reversa    <-reversa+ temporal[i-1]
        i<-i-1
    Fin Para
    devuelva reversa
Fin SubAlgoritmo

```



### Ejercicio 10

**Paso 1** : Definir el problema

Dada una lista de nombres, crea un algoritmo que ordene la lista alfabéticamente.
La lista puede contener cualquier cantidad de nombres y puede haber nombres repetidos. El objetivo del algoritmo es ordenar la lista en orden alfabético ascendente, es decir, que los nombres estén ordenados de la A a la Z.

**Paso 2** : Poner la entrada, el proceso y la salida
Entrada: Nombre
Proceso:

Definir la variable listanombres
Definir la longitud de la lista
Ordenar alfabeticamente

Salida: Nombres en orden alfabeto

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo NombresAlfabeto
   # Entrada
	nombres <- leer()
   # Proceso
	para i desde 0 hasta longitud(nombres)  hacer
		minimo <- i
			para j desde i + 1 hasta longitud(nombres) hacer
			si nombres[j] < nombres[minimo] entonces
			minimo = j
			fin si
	fin para
	intercambiar nombres[i] y nombres[minimo]
   # Salida
	mostrar "La lista ordenada alfabéticamente es: " + nombres
	Fin
Fin Algoritmo
```



### Ejercicio 11

**Paso 1** : Definir el problema

Crea un algoritmo que calcule el factorial de un número entero.¿Como se calcula? Multiplicando los numeros anteriores al numero dado

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: Leer el numero

Proceso: Factorial del numero dado
Salida: Escribir factorial

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo CalcularFctorial
   # Entrada
	numero<-leer()
   # Proceso
	factorial<- 1
	Para i <- 1 hasta numero Hacer
	   factorial  <- factorial * i
	Fin Para
   # Salida 
	Escribir factorial

Fin Algoritmo
```



### Ejercicio 12

**Paso 1** : Definir el problema

Dado un número entero, crea un algoritmo que determine si es primo o no¿Como saber si es primo o no? Si es divisible para uno y para si mismo

**Paso 2** : Poner la entrada, el proceso y la salida
Entrada: Numero entero
Proceso: Comprobar si es divisible para uno y para si mismo
Salida: Es primo o no

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo PrimoNOprimo
   # Entrada
	numero <- leer()
   # Proceso
	primo <- true
	para i desde 2 hasta numero - 1 hacer
		si numero % i == 0 entonces
		primo <- false
		break
		fin si
	fin para
	si primo entonces
   # Salida
		escribir <- "El número " + numero + " es primo"
		sino
		escribir <- "El número " + numero + " no es primo"
	fin si
Fin Algoritmo
```



### Ejercicio 13

**Paso 1** : Definir el problema

Crea un algoritmo que calcule el área y volumen de un cubo dado su lado¿Como se calcula?

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: lado del cubo
Proceso:
Cacular el area con operaciones matematicas
Calcular volumen que es igual a lado al cubo

Salida: El area y volumen

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo AreaCubi
   # Entrada
	lado <- leer()
   # Proceso
	area <- 6 * (lado * lado)
	volumen <- lado * lado * lado 
   # Salida
	escribir <- "El área del cubo es " + area + " unidades cuadradas"
	escribir <- "El volumen del cubo es " + volumen + " unidades cúbicas"
	fin
Fin Algoritmo
```

### Ejercicio 14

**Paso 1** : Definir el problema

Dada una lista de números enteros, crea un algoritmo que calcule la suma de todos los números
pares de la lista. ¿Como sumar solo los numeros pares? Quitando los duplicados y sumando los numeros unicos

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: lista
Proceso: Dividir cada numero entre 2 y si sale 0 es par y separarlo a parte y los que tengan resultado diferente son impares , una vez sacado los pares recorrer la lista de  pares y quitar los duplicados y despues sumar los unicos
Salida: Suma numeros unicos

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo SumaPares
   # Entrada
	lista <- leer()
	 # Proceso
	suma = 0
	para cada numero en lista hacer
		si numero dividido 2 = 0 entonces
		suma <- suma + numero
		fin si
	fin para
	Fin
 # Salida
	escribir <- "La suma de los números pares de la lista es " + suma
Fin Algoritmo
```

### Ejercicio 15

**Paso 1** : Definir el problema

Crea un algoritmo que determine si un número es positivo, negativo o cero.

**Paso 2** : Poner la entrada, el proceso y la salida
Entrada: numero
Proceso: Comprobar el numero con cero
Si es mayor es positivo
Si es menor es negativo
Y cero es cero
Salida: Dependiendo del numero seleccionado imprimir positivo, negativo o cero 

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo PosiNegativo
   # Entrada
	numero <- leer()
	# Proceso
	si numero > 0 entonces
	escribir <- "El número es positivo"
	sino si numero < 0 entonces
   # Salida
	escribir "El número es negativo"
	sino
	escribir "El número es cero"
	fin si

Fin Algoritmo
```

### Ejercicio 16

**Paso 1** : Definir el problema

Dada una lista de números enteros, crea un algoritmo que calcule la media de la lista. ¿Como se calcula? Sumando todos los numeros y dividiendo entre la longitud de la lista

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: lista

Proceso: 

- Pedir la lista
- Sumar los números de la lista
- Sacar la longitud de la lista
- Y dividir la suma de los números de la lista entre la longitud de la lista

Salida: Escribir "La media de la lista es "

**Paso 3** : Escribir el pseudocódigo

```
Algoritmo MediaLista
   # Entrada
	lista<- leer()
	# Proceso
	suma <- 0
	para cada numero en lista hacer
	suma <- suma + numero
	fin para
	media = suma / longitud(lista)
	escribir <- "La media de la lista es " + media
   # Salida
	Escribir<- "La media de la lista es " + media
Fin Algoritmo
```

### Ejercicio 17

**Paso 1** : Definir el problema

Crea un algoritmo que genere un número aleatorio entre 1 y 100, y le pida al usuario adivinarlo. El
algoritmo deberá indicar si el número introducido es mayor o menor que el número aleatorio, hasta
que el usuario adivine el número correcto.

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: num_aleatorio

Proceso: 
Pedir un numero de 1 a 100
Comprobar si es el numero, caso contrario poner si es mayor o menos que el numero aleatorio


Salida: numero

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo 
   # Entrada
   Inicio
	num_aleatorio<-leer()
	# Proceso
	adivinado = Falso
	mientras adivinado sea Falso
	entrada = leer_entrada_usuario()
	si entrada igual num_aleatorio entonces
	escribir<- "¡Adivinaste el número!"
	adivinado igual Verdadero
		sino si entrada mayor num_aleatorio entonces
		escribir<- "El número es mayor que " mas entrada
		sino
		escribir<- "El número es menor que " mas entrada
	fin si
	fin mientras
   # Salida
	Escrbir<-"¡Adivinaste el número!"
	fin
Fin Algoritmo
```

### Ejercicio 18

**Paso 1** : Definir el problema
Crea un algoritmo que determine si una cadena de texto es un anagrama de otra cadena de texto.¿Que es un anagrama?
Procedimiento que consiste en crear una palabra a partir de la reordenación de las letras de otra palabra.

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: Cadena de texto
Proceso: Separar las letras de la cadena de texto, proceder a ver si con la ordenacion diferente sale otra nueva palabra
Salida: Escribir si es un anagrama o no

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo Anagrama
   Algoritmo Anagrama
# Entrada
cadenal <- Leer ()
cadena2 <- Leer() # Cambiar nombre a anagrama
# Proceso
n<-ContarElementosLista(cadenal)
m<-ContarElementosLista(cadenaz)
si n es igual a m
	i <- 0
	resultado < "es anagrama"
	Mientras i sea menor o igual que n-1
		noestaletra <- True
		Para j=i Hasta n-1 con paso 1 Hacer
			Si cadenal[i] es igual a cadena2(j] Entonces
				posicion <- j
				noEstaletra <- False
			Finsi
		FinPara
		Si noEstaLetra es igual a True Entonces
			resultado <- "no es anagrama
			i <- n
		Sino
			temporal <- cadena2[i]
			cadena2(i] <- cadenal[i]
			cadena2[posicion] <- temporal
			1 <- i+1
		Finsi
	FinMientras
Sino
#salida
resultado <- "no es anagrama"
Finsi

Fin Algoritmo
```

### Ejercicio 19

**Paso 1** : Definir el problema

Dada una lista de números enteros, crea un algoritmo que elimine los números duplicados de la
lista.¿Que es un numero duplicado? Un numero repetido o que se asemejan

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: numeros
Proceso: Crear variables vacias para añadir despues los numeros unicos. recorrer la lista e ir quitando los duplicados y una vez quitados sumamos los unicos
Salida: Escribir la suma de los numeros unicos

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo 
   # Entrada
	numeros <- leer()
   # Proceso
	unicos = ""
	vistos = ""
	para numero en numeros hacer
		si numero no está en vistos entonces
			agregar numero a unicos
			agregar numero a vistos
		fin si
	fin para
   # Salida
	escribir <- "Lista original: " + numeros
	escribir <- "Lista sin duplicados: " + unicos
	fim
Fin Algoritmo
```

### Ejercicio 20

**Paso 1** : Definir el problema

Crea un algoritmo que determine si un número es capicúa o no. ¿Como saber si un numero es capicua?Aquellos que se leen igual de izquierda a derecha y de derecha a izquierda. Pongamos un ejemplo. El 23.032 sería capicúa

**Paso 2** : Poner la entrada, el proceso y la salida

Entrada: numero
Proceso: invertir el numero y si coincide con el numero introducido
Salida: Escribir si es capicua o no

**Paso 3** : Escribir el pseudocodigo

```
Algoritmo NumCapicua
   # Entrada
	numero <- leer()
   # Proceso
	cadena <- convertir_a_cadena(numero)
	inversa <- ""
	para i desde longitud(cadena) - 1 hasta 0 hacer
		inversa <- inversa + cadena[i]
	fin para
	si cadena == inversa entonces
   # Salida
	escribir <- "El número " + numero + " es capicúa"
	sino
	escribir <- "El número " + numero + " no es capicúa"
	fin si
Fin Algoritmo
```

