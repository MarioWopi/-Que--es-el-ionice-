# ¿Qué es el ionice?

El **ionice** es un comando que nos permite controlar la prioridad de acceso de los recursos de **entrada y salida**, este programa permite usar 3 clases, que son las siguientes:

    - **El Idle**
    - **El Best effort**
    - **El Real time**
    
## El Idle

- El **Idle** lo que hace es, que el proceso solo podra acceder al disco cuando el resto de programas no lo hayan pedido , por lo tanto este programa esta restringido al usuario root.
    - Ejemplo: *ionice -c3 -p123*
    
    
## El Best effort

- El **Best efford** permite el uso de un parámetro como prioridad: La mayor prioridad es 0, y la prioridad más pequeña es el 7, contra más pequeño sea el número más prioridad tendrá. Y los programas que se ejecuten con la misma prioridad, accederán al disco mediante el algoritmo round-robin.
     - Ejemplo: ionice -c2 -n0 bash
     
## El RealTime 

**NO lo entiendo**



## Opciones para ejecutar el comando

En el comando ionic hay 3 opciones, que son las siguientes:
  
  - **El -c** (la clase): Tienen 4 clases, el 0 para ninguno, 1 para RealTime, 2 para Best effort y 3 para Idle.
  - **El -n** (classdata): Esto define los datos de la clase, para el RealTime y el Best effort del 0-7. 
  - **El -p** (pid): NO LO ENTIENDO
 

