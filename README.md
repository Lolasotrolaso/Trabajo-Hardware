# Política de backup Windows
1. Realiza los siguientes apartados relativos a Copia de Seguridad en Windows,
documentando los apartados d y f:

d. Diseña y configura en “Paragon Backup & Recovery Community Edition” una
política de backup que te permita mantener copia de seguridad diaria
de todo el contenido del directorio “DatosBackup”, teniendo en cuenta
las recomendaciones estudiadas en clase (optimizar el espacio dedicado
a copias y reducir el tiempo entre copias). Habrá que programar la
ejecución de diferentes tipos de copia de seguridad. Indica de forma 
esquemática o empleando una tabla la política de backup que has
diseñado. Justifica el por qué de cada copia y su frecuencia.

## Creacion de Backups y Política de Backups
Para poder realizar las copias y su restauración, primero creamos nuestra carpeta DatosBackup y añadimos los ficheros con los que trabajaremos. Las copias para la práctica las hemos guardado en el escritorio de la propia máquina, pero se deberían guardar en un medio externo para mayor seguridad. 

![Selección de Origen1](/img/1.jpg)
![Selección de Origen2](/img/2.jpg)
![Selección de Destino1](/img/3.jpg)

La política que decidimos aplicar será diaria y comenzaría a las 10 de la noche, de tipo incremental (del domingo hasta el viernes incluido, 6 copias incrementales en total durante la semana). El sábado se realizaría la copia completa a las 10 de la noche. Los nombres de las copias los pusimos de forma manual, ya que el programa no daba opción a hacerlo automáticamente.

![Selección de Frecuencia](/img/4.jpg)
![Selección de Tipo](/img/5.jpg)
![Selección de Contraseña](/img/6.jpg)


Simulamos los siguientes escenarios:

   - El lunes modificamos erróneamente el fichero1.txt y fichero2.txt y se crearon los ficheros fichero3.txt y fichero4.txt

   - El martes se creó el fichero5.txt

   - El miércoles se borro erróneamente fichero1.pdf y se crearon los ficheros otroFichero3.jpeg y otroFichero4.jpeg

   - El jueves se borró erróneamente otroFichero1.jpg y se crearon los ficheros ficheroLog3.txt y ficheroLog4.txt (directorio Logs)

## Restauración de Backups
Para restaurar una backup iremos a la pestaña de restore backup y selecionaremos que tipo de restauracion queremos hacer que en nuestro caso sera de archivos en especifico ya que sabemos que archivos se modificaron erroneamente.

![Selección de tipo Backup](/img/7.jpg)

Selecionamos la carpeta del domingo para poder recuperar los archivos que se modificaron erroneamente el lunes.

![Selección de Backup1](/img/8.jpg)

Escribimos la contraseña ya que pusimos una opcion que por temas de seguridad encripta las copias de seguridad.

![Contraseña](/img/9.jpg)

Selecionamos los archivos que queremos recuperar ya que sabemos cuales fueron los que se modificaron erroneamente y cuando fue esa modificación.

![Selección de Archivos1](/img/10.jpg)

Selecionaremos donde se restauraran los archivos.

![Selección de destino](/img/11.jpg)

Debido a que los archivos que se modificaron no se eliminaron nos saldra que eses archivos ya se encuentran en ese directorio por lo que tendremos que selecionar la opcion de aply for all para que se aplique la opcion de replace a todos los archivos que queremos restaurar.

![Selección de Rempazo](/img/12.jpg)

Selecionamos a carpeta del martes para poder recumerar los archivos que se modificaron erroneamente el miercoles.

![Selección de Backup2](/img/13.jpg)

Escribimos la contraseña ya que pusimos una opcion que por temas de seguridad encripta las copias de seguridad.

![Contraseña](/img/9.jpg)

Selecionamos los archivos que queremos recuperar ya que sabemos cuales fueron los que se eliminaron erroneamente y cuando fue esa modificación.

![Selección de Archivos2](/img/14.jpg)

Selecionaremos donde se restauraran los archivos.

![Selección de destino](/img/11.jpg)

Selecionamos a carpeta del martes para poder recumerar los archivos que se modificaron erroneamente el jueves.

![Selección de Backup3](/img/15.jpg)

Escribimos la contraseña ya que pusimos una opcion que por temas de seguridad encripta las copias de seguridad.

![Contraseña](/img/9.jpg)

Selecionamos los archivos que queremos recuperar ya que sabemos cuales fueron los que se eliminaron erroneamente y cuando fue esa modificación.

![Selección de Archivos3](/img/16.jpg)

Y por ultimo como se puede ver en la siguientes imagenes se recupero los archivos que se borraron y modificaron erroneamente.

![Resultado Final](/img/17.jpg)

![Resultado Final2](/img/18.jpg)

# RAID Windows

En este apartado crearemos RAIDs y comprobaremos que pasa si falla un disco que pertenece a un RAID en Windows.

## Volumen Simple

Para crear un Volumen Simple en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y selecionaremos el tamaño del volumen.

![Tamaño Simple](/img/19.jpg)

A continuación selecionaremos la letra que se asignara al Volumen.

![Letra Simple](/img/20.jpg)

Selecionaremos que formato en el que queremos formatear el volumen.

![Formateo Simple](/img/21.jpg)

Al final de la configuración pondra un resumen de la configuracion selecionada.

![Final Simple](/img/22.jpg)

Y por ultimo añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Volumen Distribuido

Para crear un Volumen Distribuido en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y selecionaremos los discos y los tamaños de cada disco que se le van a asignar al volumen.

![Tamaño Distribuido](/img/23.jpg)

A continuación selecionaremos la letra que se asignara al Volumen.

![Letra Distribuido](/img/24.jpg)

Selecionaremos que formato en el que queremos formatear el volumen.

![Formateo Distribuido](/img/25.jpg)

Al final de la configuración pondra un resumen de la configuracion selecionada.

![Final Distribuido](/img/26.jpg)

Y por ultimo añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Volumen Seccionado

Para crear un Volumen Seccionado en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y selecionaremos los discos y los tamaños de cada disco que se le van a asignar al volumen.

![Tamaño Seccionado](/img/27.jpg)

A continuación selecionaremos la letra que se asignara al Volumen.

![Letra Seccionado](/img/28.jpg)

Selecionaremos que formato en el que queremos formatear el volumen.

![Formateo Seccionado](/img/29.jpg)

Al final de la configuración pondra un resumen de la configuracion selecionada.

![Final Seccionado](/img/30.jpg)

Y por ultimo añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Volumen Reflejado

Para crear un Volumen Reflejado en el administrador de discos daremos click derecho al disco donde queramos crear el volumen y selecionaremos los discos y los tamaños de cada disco que se le van a asignar al volumen.

![Tamaño Reflejado](/img/31.jpg)

A continuación selecionaremos la letra que se asignara al Volumen.

![Letra Reflejado](/img/32.jpg)

Selecionaremos que formato en el que queremos formatear el volumen.

![Formateo Reflejado](/img/33.jpg)

Al final de la configuración pondra un resumen de la configuracion selecionada.

![Final Reflejado](/img/34.jpg)

Y por ultimo añadiremos Datos al Volumen.

![Añadir Datos](/img/35.jpg)

## Comportamiento de los RAIDs despues del fallo de un disco

Tras un fallo de en un disco el administrador de discos tendra un error en los volumenes a excepción del Volumen Simple y ya no aparecera ni el volumen Distribuido ni el Volumen Seccionado en el administrador de archivos como podemos ver en las imagenes y en la tabla a continuación.

![Discos Fallo1](/img/36.jpg)

![Discos Fallo2](/img/37.jpg)

|   | Simple   | Distribuido   | Seccionado   | Reflejado   |
| ------- | -------- | -------- | -------- | -------- |
| Disponibilidad de la informacion  |  Si    |    No   |    No   |     Si    |
|  Velocidad   | Normal |  Doble de rapido (aprox) |  Doble de rapido (aprox) | Normal |
| Comportamiento |  No es un RAID   |   RAID 0: porque divide la información entre los dos discos  |   RAID 0: porque divide la información entre los dos discos    |    RAID 1: realiza una copia exacta de la información en el segundo disco   | 


# RAID Linux

En este apartado crearemos RAIDs y comprobaremos que pasa si falla un disco que pertenece a un RAID en Linux.

## RAID 0

Lo primero que tendremos que hacer es con el comando lsblk para poder ver el nombre que el sistema asigno a los discos que como podemos ver en la imagen son sdb y sdc.

![Ver Discos](/img/38.jpg)

A continuacion ya sabiendo el nombre de los discos ejecutaremos el comando mostrado acontinuación donde despues de --create /dev/ pondremos el nombre que queremos utilizar en el raid, despues de --level= pondremos el nivel del raid que en este caso es 0 y por ultimo despues de --raid-devices= pondremos la cantidad de discos que queremos utilizar en el raid y sus ubicaciones en el sistema que las podemos encontar en el paso anterior.

      mdadm --create /dev/md0 --level=0 --raid-devices=2 /dev/sdb /dev/sdc

![Crear RAID](/img/39.jpg)

Despues Formatearemos el disco en NTFS.

![Formateo Disco](/img/43.jpg)

Le añadimos la informacion que queramos guardar en el RAID.

![Añadir Datos](/img/40.jpg)

Y al fallar un disco al ser un RAID 0 habremos perdido la información almacenada en el.

![Fallo Disco](/img/41.jpg)

## RAID 1

Lo primero que tendremos que hacer es con el comando lsblk para poder ver el nombre que el sistema asigno a los discos que como podemos ver en la imagen son sdb y sdc.

![Ver Discos](/img/38.jpg)

A continuacion ya sabiendo el nombre de los discos ejecutaremos el comando mostrado acontinuación donde despues de --create /dev/ pondremos el nombre que queremos utilizar en el raid, despues de --level= pondremos el nivel del raid que en este caso es 1 y por ultimo despues de --raid-devices= pondremos la cantidad de discos que queremos utilizar en el raid y sus ubicaciones en el sistema que las podemos encontar en el paso anterior.

      mdadm --create /dev/md0 --level=1 --raid-devices=2 /dev/sdb /dev/sdc

![Crear RAID](/img/42.jpg)

Despues Formatearemos el disco en NTFS.

![Formateo Disco](/img/43.jpg)

Le añadimos la informacion que queramos guardar en el RAID.

![Añadir Datos](/img/44.jpg)

Y al fallar un disco al ser un RAID 1 podremos continuar accediendo a la información almacenada.

## RAID 5

Lo primero que tendremos que hacer es con el comando lsblk para poder ver el nombre que el sistema asigno a los discos que como podemos ver en la imagen son sdb, sdc y sdd.

![Ver Discos](/img/38.jpg)

A continuacion ya sabiendo el nombre de los discos ejecutaremos el comando mostrado acontinuación donde despues de --create /dev/ pondremos el nombre que queremos utilizar en el raid, despues de --level= pondremos el nivel del raid que en este caso es 5 y por ultimo despues de --raid-devices= pondremos la cantidad de discos que queremos utilizar en el raid y sus ubicaciones en el sistema que las podemos encontar en el paso anterior.

      sudo mdadm -C /dev/md0 -l raid5 -n 3 /dev/sd[b-d]1

![Añadir Datos](/img/45.jpg)

Despues Formatearemos el disco en NTFS.

![Añadir Datos](/img/46.jpg)

Le añadimos la informacion que queramos guardar en el RAID.

![Añadir Datos](/img/47.jpg)

Y al fallar un disco al ser un RAID 5 podremos continuar accediendo a la información almacenada.

## Comportamiento de los RAIDs despues del fallo de un disco


|   | RAID 0  | RAID 1   | RAID 5  | 
| ------- | -------- | -------- | -------- |
| Disponibilidad de la informacion  | No  |   Si   |   Si  |
| Discos necesarios   | 2 discos mínimo |  2 discos mínimo (en pares) |  3 discos mínimo  | 
| Espacio disponible |  100%  | 50% | 66%  |
| Tolerancia de fallo |  No   |   Si, 1 disco  |  Si, 1 disco  |
