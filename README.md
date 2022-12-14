# Corecore-Practice-Challenges-week-3

## Ejercicio 1 - Calculadora
For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

Sum (+)

Subtract (-)

Multiplication (*)

Division (/)

The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). 

The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. 

If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. 

After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. 

``` python

  Algoritmo calculadora
	Imprimir "Bienvenido a la calculadora, por favor ingrese la operación deseada"
	Imprimir "1 para Suma (+)"
	Imprimir "2 para Resta (-)"
	Imprimir "3 para Multiplicación (*)"
	Imprimir "4 para División (/)"
	Leer operacion 
	imprimir "Ingrese los dos números a operar"
	leer x
	leer z
	si operacion == 4 y z == 0 entonces 
		Imprimir "❌ Operación no es valida"
	FinSi
	si operacion == 1  entonces
		r=x+z
		Imprimir "Procesando " x " + " z
		Imprimir "Resultado: " r
	FinSi
	si operacion == 2 entonces
		r=x-z
		Imprimir "Procesando " x " - " z
		Imprimir "Resultado: " r
	FinSi
	si operacion == 3 entonces
		r=x*z
		Imprimir "Procesando " x " * " z
		Imprimir "Resultado: " r
		fin si
	si operacion == 4 y z <> 0 entonces 
		r=x/z
		Imprimir "Procesando " x " / " z
		Imprimir "Resultado: " r
	Fin si
	
FinAlgoritmo
``` 

## Challenge 2 - Special number
You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number"

``` python

  Algoritmo specialNumber
	Leer n
	Si n == 100 Entonces
		Imprimir 'This is a special number'
	Sino
	Si n<1000 y (n%10=0) y n <> 100 Entonces
		Imprimir 'This number is almost special'
	SiNo
		Imprimir 'Just a regular number'
	FinSi
  FinSi

  FinAlgoritmo
  ``` 
  
  
 ## Challenge 3 - Calculadora Usando Segun 
 
 ``` python
 
 	Algoritmo CalculadoraUsandoSegun
	Imprimir "Bienvenido a la calculadora de JA"
	Imprimir "Por favor ingrese los números que desea operar"
	Leer x;
	Leer z;
	Imprimir "Por favor ingrese +, -, x, / según la operación que quiera realizar"
	Leer cal;
	Si cal == "+" o cal == "-" o cal == "x" o cal == "*" o cal == "/" Entonces
		Imprimir "Procesando " x cal z
		Segun cal hacer 
			"+":
				r=x+z
				Imprimir "El resultado es:" r
			"-":
				r=x-z
				Imprimir "El resultado es:" r
			"*" o "x":
				r=x*z
				Imprimir "El resultado es:" r
			"/":
				si z<>0 entonces r=x/z
					Imprimir "El resultado es:" r
				sino imprimir "Error, no puede dividir entre 0"
					fin si
			FinSegun
			sino imprimir "Operación no valida, por favor ingrese bien la operacion +, -, x, /"
		FinSi
	
	
	
	FinAlgoritmo
	
```

## Challenge 4 - Opción MultiPrograma

 ``` python

	Algoritmo MultiOptionProgram
	// Sum two numbers
	// Print the day of the week given the day number
	// Print the length of a given text
	Imprimir "Bienvenido al programa de multi opciones"
	Imprimir "Por favor seleccione una de las siguientes opciones para iniciar"
	Imprimir "1. Suma entre dos números"
	Imprimir "2. Imprime el día de la semana según el número ingresado"
	Imprimir "3. Imprime la longitud del texto de un texto dado"
	Leer operacion 
	Segun operacion
		"1":
			Imprimir "Ingrese los números que desea sumar"
			leer x
			Leer z
			r=x+z
			Imprimir "El resultado es " r
		"2":
			Imprimir "Ingrese el número para el día que desea ver"
			Leer n 
			Si n<1 o n>7 Entonces
				Repetir 
					Imprimir "ERROR INGRESE NUMERO ENTRE 1 y 7" 
					leer n
				Hasta Que n >= 1 y n<=7
			Fin si
			segun n
				1:
					Imprimir "Lunes"
				2:
					Imprimir "Martes"
				3:
					Imprimir "Miercoles"
				4:
					Imprimir "Jueves"
				5:
					Imprimir "Viernes"
				6:
					Imprimir "Sábado"
				7:
					Imprimir "Domingo"
			FinSegun
		"3":
			Imprimir "Ingrese el texto que desea leer"
			leer text
			Imprimir "El largo del texto es de " longitud(text) " caracteres"
	FinSegun
	
	FinAlgoritmo
 ```
## Challenge 5 - TablasDeMultiplicar

 ``` python
 	Algoritmo TablasMultiplicar
	Imprimir "Tablas de multiplicar"
	Imprimir "Ingrese la tabla a calcular"
	Leer n
	z=1
	Imprimir "La tabla de " n " es"
	Mientras z <= 10 hacer 
		r=n*z
		Imprimir n "*" z "=" r
		z= z+1
	FinMientras
	Imprimir "Fin de la tabla"
	FinAlgoritmo
 ```
## Challenge 6 - Calculadora usando Do - While

``` python

	Algoritmo CalculadoraUsandoSegun
	Imprimir "Bienvenido a la calculadora de JA"
	Repetir
	Imprimir "Por favor ingrese los números que desea operar"
	Leer x;
	Leer z;
	Imprimir "Por favor ingrese +, -, x, / según la operación que quiera realizar"
	Leer cal;
	Si cal == "+" o cal == "-" o cal == "x" o cal == "*" o cal == "/" Entonces
		Imprimir "Procesando " x cal z
		Segun cal hacer 
			"+":
				r=x+z
				Imprimir "El resultado es:" r
			"-":
				r=x-z
				Imprimir "El resultado es:" r
			"*" o "x":
				r=x*z
				Imprimir "El resultado es:" r
			"/":
				si z<>0 entonces r=x/z
					Imprimir "El resultado es:" r
				sino imprimir "Error, no puede dividir entre 0"
					fin si
			FinSegun
			sino imprimir "Operación no valida, por favor ingrese bien la operacion +, -, x, /"
			FinSi
			Imprimir "Ingrese 1 para continuar con otra operación, e ingrese 2 para cerrar la calculadora"
			Leer n
	Hasta que n=2
	Imprimir "Calculadora Cerrada"
	
	FinAlgoritmo
```

## Challenge 7 - Tabla con For

``` python

	Algoritmo TablaConFor
	Imprimir "Tablas de multiplicar"
	Imprimir "Ingrese el número que desea operar"
	Leer n
	Imprimir "Tabla del " n
	Para z = 1 hasta 10 Hacer
		r=n*z
		Imprimir n "*" z "= " r
	FinPara
	
	FinAlgoritmo
```

## Challenge 8 - Orden Descendente / Ascendente

``` python

	Algoritmo OrdenNumeros
	// Usuario ingresa un numero y decide si presentarlo de forma ascendente o descendente desde 0
	Imprimir "Por favor ingrese el número que desea ejecutar";
	Leer n
	Imprimir "Ingrese 1 o 2 según la opción que desea ejecutar"
	Imprimir "1) Orden Ascendente (0 hasta el número ingresado)"
	Imprimir "2) Orden Descendente (Número ingresado a 0)"
	Leer z 
	Segun z Hacer 
		1: Para x<-0 Hasta n Con paso 1 Hacer 
				Imprimir x
			FinPara
		2: Para x<-n Hasta 0 Con paso -1 Hacer 
				Imprimir x
			FinPara
	FinSegun
	FinAlgoritmo
```

## Challenge 9 - Saludos 

``` python

	Algoritmo Saludos
	//Print Buenos dias! if the hour is from 0 to 12 - Buenas tardes! if the hour is from 13 to 18 - Buenas noches! if the hour is from 19 to 23
	// Ask the user if he wants to perform another greeting. If the answer is Si, the program must start again.
	// At the end of the program, print out the number of times the program has greeted.
	Para x<-0 Hasta x Con paso 1 Hacer 
	Repetir 
		Imprimir "Ingrese la hora del día"
		Leer h
		Si h==24 o h<=12 entonces
			Imprimir "Buenos días!"
		FinSi
		Si h>12 y h<=18 Entonces
			Imprimir "Buenas tardes!"
			Fin Si
		Si h<24 y h>=19 Entonces 
			Imprimir "Buenas noches!"
		FinSi
		Si h>24 o h<0 Entonces
			Imprimir "ERROR - Ingrese hora valida (0-24h)"
		FinSi
		Imprimir "¿Desea repetir el programa? (SI/NO)"
		Leer r
		x = x+1
	Hasta que Mayusculas(r) == "NO"
	Finpara 
	Imprimir "El programa se cargó " x " veces"
	FinAlgoritmo
```
