# Trabajo UD7

En este trabajo exploramos el manejo de discos en RAIDs y la disponibilidad de la información que contienen, ademas de la protección de la información mediante Politicas de backups.

## Creación de Backups y Política de Backups
Para poder realizar las copias y su restauración, primero creamos nuestra carpeta DatosBackup y añadimos los ficheros con los que trabajaremos. Las copias para la práctica las hemos guardado en el escritorio de la propia máquina, pero se deberían guardar en un medio externo para mayor seguridad. 

![Selección de Origen1](/img/1.jpg)
![Selección de Origen2](/img/2.jpg)
![Selección de Destino1](/img/3.jpg)

La política que decidimos aplicar será diaria y comenzaría a las 10 de la noche, de tipo incremental (del domingo hasta el viernes incluido, 6 copias incrementales en total durante la semana). El sábado se realizaría la copia completa a las 10 de la noche. Los nombres de las copias los pusimos de forma manual, ya que el programa no daba opción a hacerlo automáticamente.

![Selección de Frecuencia](/img/4.jpg)
![Selección de Tipo](/img/5.jpg)
![Selección de Contraseña](/img/6.jpg)




## Restauración de Backups
Simulamos los siguientes escenarios:

   - El lunes modificamos erróneamente el fichero1.txt y fichero2.txt y se creamos los ficheros fichero3.txt y fichero4.txt

   - El martes creamos el fichero5.txt

   - El miércoles borramos erróneamente fichero1.pdf y creamos los ficheros otroFichero3.jpeg y otroFichero4.jpeg

   - El jueves borramos erróneamente otroFichero1.jpg y creamos los ficheros ficheroLog3.txt y ficheroLog4.txt (directorio Logs)

Para restaurar una backup iremos a la pestaña de restore backup y seleccionaremos que tipo de restauración queremos hacer que en nuestro caso será de archivos en específico ya que sabemos que archivos se modificaron erróneamente.

![Selección de tipo Backup](/img/7.jpg)

Seleccionamos la carpeta del domingo para poder recuperar los archivos que se modificaron erróneamente el lunes.

![Selección de Backup1](/img/8.jpg)

Escribimos la contraseña ya que pusimos una opción que por temas de seguridad encripta las copias de seguridad.

![Contraseña](/img/9.jpg)

Seleccionamos los archivos que queremos recuperar ya que sabemos cuales fueron los que se modificaron erróneamente y cuando fue esa modificación.

![Selección de Archivos1](/img/10.jpg)

Seleccionaremos donde se restaurarán los archivos.

![Selección de destino](/img/11.jpg)

Debido a que los archivos que se modificaron no se eliminaron nos saldrá que eses archivos ya se encuentran en ese directorio por lo que tendremos que seleccionar la opción de apply for all para que se aplique la opción de replace a todos los archivos que queremos restaurar.

![Selección de Reemplazo](/img/12.jpg)

Seleccionamos la carpeta del martes para poder recuperar los archivos que se modificaron erróneamente el miércoles.

![Selección de Backup2](/img/13.jpg)

Escribimos la contraseña ya que pusimos una opción que por temas de seguridad encripta las copias de seguridad.

![Contraseña](/img/9.jpg)

Seleccionamos los archivos que queremos recuperar ya que sabemos cuales fueron los que se eliminaron erróneamente y cuando fue esa modificación.

![Selección de Archivos2](/img/14.jpg)

Seleccionaremos donde se restaurarán los archivos.

![Selección de destino](/img/11.jpg)

Seleccionamos la carpeta del martes para poder recuperar los archivos que se modificaron erróneamente el jueves.

![Selección de Backup3](/img/15.jpg)

Escribimos la contraseña ya que pusimos una opción que por temas de seguridad encripta las copias de seguridad.

![Contraseña](/img/9.jpg)

Seleccionamos los archivos que queremos recuperar ya que sabemos cuáles fueron los que se eliminaron erróneamente y cuando fue esa modificación.

![Selección de Archivos3](/img/16.jpg)

Y por último como se puede ver en la siguientes imágenes se recupero los archivos que se borraron y modificaron erróneamente.

![Resultado Final](/img/17.jpg)

![Resultado Final2](/img/18.jpg)

# RAID Windows

En este apartado crearemos RAIDs y comprobaremos que pasa si falla un disco que pertenece a un RAID en Windows.

## Volumen Simple

Para crear un Volumen Simple en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y seleccionaremos el tamaño del volumen.

![Tamaño Simple](/img/19.jpg)

A continuación seleccionaremos la letra que se asignará al Volumen.

![Letra Simple](/img/20.jpg)

Seleccionaremos qué formato en el que queremos formatear el volumen.

![Formateo Simple](/img/21.jpg)

Al final de la configuración pondrá un resumen de la configuración seleccionada.

![Final Simple](/img/22.jpg)

Y por último añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Volumen Distribuido

Para crear un volumen Distribuido en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y seleccionaremos los discos y los tamaños de cada disco que se le van a asignar al volumen.

![Tamaño Distribuido](/img/23.jpg)

A continuación seleccionaremos la letra que se asignará al Volumen.

![Letra Distribuido](/img/24.jpg)

Seleccionaremos qué formato en el que queremos formatear el volumen.

![Formateo Distribuido](/img/25.jpg)

Al final de la configuración pondrá un resumen de la configuración seleccionada.

![Final Distribuido](/img/26.jpg)

Y por último añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Volumen Seccionado

Para crear un Volumen Seccionado en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y seleccionaremos los discos y los tamaños de cada disco que se le van a asignar al volumen.

![Tamaño Seccionado](/img/27.jpg)

A continuación seleccionaremos la letra que se asignará al Volumen.

![Letra Seccionado](/img/28.jpg)

Seleccionaremos qué formato en el que queremos formatear el volumen.

![Formateo Seccionado](/img/29.jpg)

Al final de la configuración pondrá un resumen de la configuración seleccionada.

![Final Seccionado](/img/30.jpg)

Y por último añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Volumen Reflejado

Para crear un Volumen Reflejado en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y seleccionaremos los discos y los tamaños de cada disco que se le van a asignar al volumen.

![Tamaño Reflejado](/img/31.jpg)

A continuación seleccionaremos la letra que se asignará al Volumen.

![Letra Reflejado](/img/32.jpg)

Seleccionaremos qué formato en el que queremos formatear el volumen.

![Formateo Reflejado](/img/33.jpg)

Al final de la configuración pondrá un resumen de la configuración seleccionada.

![Final Reflejado](/img/34.jpg)

Y por último añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Comportamiento de los RAIDs después del fallo de un disco

Tras un fallo de en un disco el administrador de discos tendrá un error en los volúmenes a excepción del Volumen Simple y ya no aparecerá ni el volumen Distribuido ni el Volumen Seccionado en el administrador de archivos como podemos ver en las imágenes y en la tabla a continuación.

![Discos Fallo1](/img/36.jpg)

![Discos Fallo2](/img/37.jpg)

|   | Simple   | Distribuido   | Seccionado   | Reflejado   |
| ------- | -------- | -------- | -------- | -------- |
| Disponibilidad de la información  |  Si    |    No   |    No   |     Si    |
|  Velocidad   | Normal |  Doble de rápido (aprox) |  Doble de rápido (aprox) | Normal |
| Comportamiento |  No es un RAID   |   RAID 0: porque divide la información entre los dos discos  |   RAID 0: porque divide la información entre los dos discos    |    RAID 1: realiza una copia exacta de la información en el segundo disco   | 


# RAID Linux

En este apartado crearemos RAIDs y comprobaremos que pasa si falla un disco que pertenece a un RAID en Linux.

## RAID 0

Lo primero que tendremos que hacer es con el comando lsblk para poder ver el nombre que el sistema asignó a los discos que como podemos ver en la imagen son sdb y sdc.

![Ver Discos](/img/38.jpg)

A continuación ya sabiendo el nombre de los discos ejecutaremos el comando mostrado a continuación donde después de --create /dev/ pondremos el nombre que queremos utilizar en el raid, después de --level= pondremos el nivel del raid que en este caso es 0 y por ultimo despues de --raid-devices= pondremos la cantidad de discos que queremos utilizar en el raid y sus ubicaciones en el sistema que las podemos encontrar en el paso anterior.

      mdadm --create /dev/md0 --level=0 --raid-devices=2 /dev/sdb /dev/sdc

![Crear RAID](/img/39.jpg)

Después Formateamos el disco en NTFS.

![Formateo Disco](/img/43.jpg)

Le añadimos la información que queramos guardar en el RAID.

![Añadir Datos](/img/40.jpg)

Y al fallar un disco al ser un RAID 0 habremos perdido la información almacenada en él.

![Fallo Disco](/img/41.jpg)

## RAID 1

Lo primero que tendremos que hacer es usar el comando lsblk para poder ver el nombre que el sistema asignó a los discos que como podemos ver en la imagen son sdb y sdc.

![Ver Discos](/img/38.jpg)

A continuación ya sabiendo el nombre de los discos ejecutaremos el comando mostrado a continuación donde después de --create /dev/ pondremos el nombre que queremos utilizar en el raid, después de --level= pondremos el nivel del raid que en este caso es 1 y por ultimo despues de --raid-devices= pondremos la cantidad de discos que queremos utilizar en el raid y sus ubicaciones en el sistema que las podemos encontrar en el paso anterior.

      mdadm --create /dev/md0 --level=1 --raid-devices=2 /dev/sdb /dev/sdc

![Crear RAID](/img/42.jpg)

Después Formateamos el disco en NTFS.

![Formateo Disco](/img/43.jpg)

Le añadimos la información que queramos guardar en el RAID.

![Añadir Datos](/img/44.jpg)

Y al fallar un disco al ser un RAID 1 podremos continuar accediendo a la información almacenada.

## RAID 5

Lo primero que tendremos que hacer es usar el comando lsblk para poder ver el nombre que el sistema asignó a los discos que como podemos ver en la imagen son sdb, sdc y sdd.

![Ver Discos](/img/38.jpg)

A continuación ya sabiendo el nombre de los discos ejecutaremos el comando mostrado a continuación donde después de --create /dev/ pondremos el nombre que queremos utilizar en el raid, después de --level= pondremos el nivel del raid que en este caso es 5 y por ultimo despues de --raid-devices= pondremos la cantidad de discos que queremos utilizar en el raid y sus ubicaciones en el sistema que las podemos encontar en el paso anterior.

      sudo mdadm -C /dev/md0 -l raid5 -n 3 /dev/sd[b-d]1

![Crear RAID](/img/46.jpg)

Después Formateamos el disco en NTFS.

![Formateo Disco](/img/45.jpg)

Le añadimos la información que queramos guardar en el RAID.

![Añadir Datos](/img/47.jpg)

Y al fallar un disco al ser un RAID 5 podremos continuar accediendo a la información almacenada.

## Comportamiento de los RAIDs después del fallo de un disco


|   | RAID 0  | RAID 1   | RAID 5  | 
| ------- | -------- | -------- | -------- |
| Disponibilidad de la información  | No  |   Si   |   Si  |
| Discos necesarios   | 2 discos mínimo |  2 discos mínimo (en pares) |  3 discos mínimo  | 
| Espacio disponible |  100%  | 50% | 66%  |
| Tolerancia de fallo |  No   |   Si, 1 disco  |  Si, 1 disco  |


