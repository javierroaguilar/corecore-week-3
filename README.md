# corecore-week-3

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
