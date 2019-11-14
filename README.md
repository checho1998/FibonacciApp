# FibonacciApp

# Arquitecturas de Software - ARSW

# Escalamiento en Azure con Maquinas Virtuales, Sacale Sets y Service Plans

## Parte 0 - Entendiendo el escenario de calidad

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/primera.PNG)

## Parte 1.1 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/segunda.PNG)

## Parte 1.2 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/tercera.PNG)

## Parte 1.3 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/cuartaA.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/cuartaB.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/cuartaC.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/cuartaD.PNG)

## Parte 1.4 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/quinta.PNG)


## Parte 1.5 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/sextaA.PNG)


![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/sextaB.PNG)

## Parte 1.6 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/septima.PNG)

## Parte 1.7 - Escalabilidad vertical

- 1000000
![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/octavaA.PNG)

- 1090000
![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/octavaB.PNG)

## Parte 1.8 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/novena.PNG)

## Parte 1.9 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diez.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diezB.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diezC.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diezD.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diezF.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diezE.PNG)

## Parte 1.10 - Escalabilidad vertical

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/size.PNG)

## Parte 1.11 - Escalabilidad vertical

De nuevo parte 7:
 
![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/1010000Mejorado.PNG)


![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/1030000M.PNG)


![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/1050000M.PNG)


![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/1090000M.PNG)

De nuevo parte 8: 


![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/mejorado.PNG)

De nuevo parte 9: 

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/92.PNG)




**Preguntas**

1. ¿Cuántos y cuáles recursos crea Azure junto con la VM?

 - R// Microsoft azure para cada maquina virtual crea 3 recursos en paralelo
 
2. ¿Brevemente describa para qué sirve cada recurso?

 - postman96: Este recurso es el encargado de manejar las interfaces de red en la maquina virtual
 - postman-ip: Este recurso es el encargado de maneja la direccion IP publica de la maquina virtual 
 - postman-nsg: Este recurso es el encargado de manejar en la maquina virtual los grupos
 
 
3. ¿Al cerrar la conexión ssh con la VM, por qué se cae la aplicación que ejecutamos con el comando `npm FibonacciApp.js`? ¿Por qué debemos crear un *Inbound port rule* antes de acceder al servicio?
 
 R//:  Al cerrar la conexión ssh con la Maquina Virtual , el proceso en la aplicacion que se esta ejecutando se detiene ya que es              corrido desde la consola y al cerrarla se cae.
 
 Tenemos que crear un *Inbound port rule* para que otras personas puedan ingresar a nuestra aplicacion desde otro pc con internet.
 
4. Adjunte tabla de tiempos e interprete por qué la función tarda tando tiempo.

 R//:
   - 1000000 : 22.88s
   - 1010000 : 23.79s
   - 1020000 : 24.33s
   - 1030000 : 24.94s
   - 1040000 : 25.51s
   - 1050000 : 25.89s
   - 1060000 : 26.22s
   - 1070000 : 26.87s
   - 1080000 : 27.63s
   - 1090000 : 28.10s
   
5. Adjunte imágen del consumo de CPU de la VM e interprete por qué la función consume esa cantidad de CPU.
 
 R//:
 
   ![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/dese.PNG)

   - Debido a que nuestra maquina virtual tiene unas especificaciones muy bajas consume mayor CPU que otras.
 
6. Adjunte la imagen del resumen de la ejecución de Postman. Interprete:
    * Tiempos de ejecución de cada petición.
    * Si hubo fallos documentelos y explique.
7. ¿Cuál es la diferencia entre los tamaños `B2ms` y `B1ls` (no solo busque especificaciones de infraestructura)?
8. ¿Aumentar el tamaño de la VM es una buena solución en este escenario?, ¿Qué pasa con la FibonacciApp cuando cambiamos el tamaño de la VM?
9. ¿Qué pasa con la infraestructura cuando cambia el tamaño de la VM? ¿Qué efectos negativos implica?
10. ¿Hubo mejora en el consumo de CPU o en los tiempos de respuesta? Si/No ¿Por qué?
11. Aumente la cantidad de ejecuciones paralelas del comando de postman a `4`. ¿El comportamiento del sistema es porcentualmente mejor?


# Parte 2 - Escalabilidad horizontal

## Crear el Balanceador de Carga


- Crear el Balanceador de Carga

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.1.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.2.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.3.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.4.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.5.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.6.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.7.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.9.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.10.PNG)

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.11.PNG)
