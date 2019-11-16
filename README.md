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

 - R// Microsoft azure para cada maquina virtual crea 6 recursos en paralelo
 
 - Public IP address
 - Network Security Group
 - Network Interface
 - Disk
 - Virtual Network
 - Storage Account

2. ¿Brevemente describa para qué sirve cada recurso?

 - Public IP address: Este recurso es el encargado de tener la direccion IP publica para poder comunicarse con otras maquinas u otros recursos.
 - Network Security Group: Este recurso se encarga de dejar pasar algunas cosas y otras no para dirigir el trafico de datos hacia un grupo de red con una red virtual determinada.
 - Network Interface: Este recurso deja a las maquinas virtuales comunicarse con recursos locales y con internet.
 - Disk: Este recurso es el disco que se encarga de guardar todo lo de la maquina virtul.
 - Virtual Network: Este recurso es el que deja que diferentes recursos de Azure como las maquinas y otros puedan interactuar de una forma mas segura por medio de las redes y el internet.
 - Storage Account: Este recurso es el que guarda todos los datos como lo son archivos, tablas, discos entre otros.
 
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

   - Debido a que nuestra maquina virtual tiene unas especificaciones muy bajas consume mayor CPU que otras a diferencia que cuando le activamos el B1ms que lo hace mucho mas rapido y el porcentaje de consumo es menor.
 
6. Adjunte la imagen del resumen de la ejecución de Postman. Interprete:
    * Tiempos de ejecución de cada petición.
    * Si hubo fallos documentelos y explique.
B1ls:

Acontinuacion mostramos el resumen de las peticiones concurrentes que se le realizaron al servidor.

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/diezE.PNG)

Los resultados nos muestran que el tiempo que tardo en responder cada peticion es de 24.3s, con esta cantidad de datos aproximadamente recibidos de 1.99MB y sin ningun error. 

B2ms:

 el cosumo es el mismo:

 ![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/92.PNG)

7. ¿Cuál es la diferencia entre los tamaños `B2ms` y `B1ls` (no solo busque especificaciones de infraestructura)?

Primero el disco `B2ms` es mucho mas cara que el disco `B1ls`.

B2ms = memoria 8GB Storage 16GiB CPU performance 60% max. Performance 200% max.NICs 3

B1ls = memoria 0.5GB Storage 4GiB CPU performance 5% max. Performance 100% max.NICs 2

8. ¿Aumentar el tamaño de la VM es una buena solución en este escenario?, ¿Qué pasa con la FibonacciApp cuando cambiamos el tamaño de la VM?
 No, ya que el algoritmo no utiliza estos nuevos recursos y por eso el consumo antes y despues al igual que el tiempo de respuesta es el mismo asi que si se desea aumentar este tiempo de respuesta es necesario mejorar el algoritmo de Fibonacci.

La aplicacion deja de funcionar al momento de realizar el cambio y toca volver a activarla para que vuelba estar en ejecucion.

9. ¿Qué pasa con la infraestructura cuando cambia el tamaño de la VM? ¿Qué efectos negativos implica?

Como lo dije anteriormente al cambiar el tamaño de los recursos de la maquina virtual ella se reinicia y es necesario volver a correr la aplicacion ya que se detiene al momento de hacer este cambio. 

10. ¿Hubo mejora en el consumo de CPU o en los tiempos de respuesta? Si/No ¿Por qué?

Al ver la tablas publicadas anteriormente se puede ver que el consumo de CPU disminuye pero en los tiempos de respuesta son iguales ya que la aplicacion no hace uso de estos nuevos recursos y la mejora es por que esta maquina mejora la capacidad de procesamiento y no deja que se caiga el programa y realice mas operaciones.

11. Aumente la cantidad de ejecuciones paralelas del comando de postman a `4`. ¿El comportamiento del sistema es porcentualmente mejor?


# Parte 2 - Escalabilidad horizontal

## Crear el Balanceador de Carga


- Parte 2.1 - Escalabilidad horizontal

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.PNG)
![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.1.PNG)

 - Parte 2.2 - Escalabilidad horizontal 

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.2.PNG)

 - Parte 2.3 - Escalabilidad horizontal

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.3.PNG)

 - Parte 2.4 - Escalabilidad horizontal

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.4.PNG)

 - Parte 2.5 - Escalabilidad horizontal

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.5.PNG)

- Crear las maquinas virtuales (Nodos)

 - Parte 3.1 - Crear las maquinas virtuales
 
![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.6.PNG)

 - Parte 3.2 - Crear las maquinas virtuales

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.7.PNG)

 - Parte 3.3 - Crear las maquinas virtuales
 
![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.9.PNG)

 - Parte 3.4 - Crear las maquinas virtuales

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.10.PNG)

 - Parte 3.5 - Crear las maquinas virtuales

![Imagenes](https://github.com/checho1998/FibonacciApp/blob/master/Imagenes/PARTE2.11.PNG)


#### Preguntas

 - ¿Cuáles son los tipos de balanceadores de carga en Azure y en qué se diferencian?, ¿Qué es SKU, qué tipos hay y en qué se diferencian?, ¿Por qué el balanceador de carga necesita una IP pública?
 - ¿Cuál es el propósito del Backend Pool?

 R//: El proposito del backend pool es el que se encarga de recibir los datos de una manera similar a el de una aplicacion y dan respuesta, y definen como esos diferentes bakends se evaluan.
 
 - ¿Cuál es el propósito del Health Probe?
 
 El proposito de el Health Probe es determinar o evaluar la salud y el estado de los diferentes bakends para asi distribuir la carga en de las peticiones de los usuarios.
 
 - ¿Cuál es el propósito de la Load Balancing Rule? ¿Qué tipos de sesión persistente existen, por qué esto es importante y cómo puede afectar la escalabilidad del sistema?.

- ¿Qué es una Virtual Network? ¿Qué es una Subnet? ¿Para qué sirven los address space y address range?

Una Virtual Network es un tipo de red virtual propia en la nube para el uso del usuario en la nube de Azure. 

Una Subnet es un rango de direcciones IP para asignarlas a las diferentes maquinas y para eso es bueno implementar una division de una red grande en varias sub redes de esta misma.


 - ¿Qué son las Availability Zone y por qué seleccionamos 3 diferentes zonas?. ¿Qué significa que una IP sea zone-redundant?
 
 - ¿Cuál es el propósito del Network Security Group?
  
  Este recurso se encarga de dejar pasar algunas cosas y otras no para dirigir el trafico de datos hacia un grupo de red con una red virtual determinada.
  
 - Informe de newman 1 (Punto 2)
 
 - Presente el Diagrama de Despliegue de la solución.

