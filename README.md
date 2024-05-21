# Política de backup y sistemas RAID.
1. Realiza los siguientes apartados relativos a Copia de Seguridad en Windows,
documentando los apartados d y f:

a. En un Windows 11 Pro instala el software “Paragon Backup & Recovery
Community Edition”.

b. Dedica unos minutos a familiarizarte con su interfaz e identifica cómo
puedes: crear diferentes tipos de copias de seguridad (completa,
incremental y diferencial), cómo programar la ejecución de las copias,
cómo establecer copia de seguridad para todo el sistema, cómo
establecer copia de seguridad para un conjunto de ficheros y directorios
concreto, cómo puedes restaurar los datos que contiene una copia de
seguridad, etc.

c. Crea la siguiente estructura de ficheros y directorios en
C:\Users\tuUsuario\Documents\:
- [d] DatosBackup
    - [d] Logs
        - [f] ficheroLog1.txt
        - [f] ficheroLog2.txt
    - [f] fichero1.txt
    - [f] fichero2.txt
    - [f] fichero1.pdf
    - [f] otroFichero1.jpeg
    - [f] otroFichero2.jpeg

d. Diseña y configura en “Paragon Backup & Recovery Community Edition” una
política de backup que te permita mantener copia de seguridad diaria
de todo el contenido del directorio “DatosBackup”, teniendo en cuenta
las recomendaciones estudiadas en clase (optimizar el espacio dedicado
a copias y reducir el tiempo entre copias). Habrá que programar la
ejecución de diferentes tipos de copia de seguridad. Indica de forma
esquemática o empleando una tabla la política de backup que has
diseñado. Justifica el por qué de cada copia y su frecuencia.

e. Simula los siguientes escenarios:

   - El lunes se modificaron erróneamente fichero1.txt y fichero2.txt y se crearon los ficheros fichero3.txt y fichero4.txt

   - El martes se creó el fichero5.txt

   - El miércoles se borro erróneamente fichero1.pdf y se crearon los ficheros otroFichero3.jpeg y otroFichero4.jpeg

   - El jueves se borró erróneamente otroFichero1.jpg y se crearon los ficheros ficheroLog3.txt y ficheroLog4.txt (directorio Logs)

f. Realiza y documenta el proceso de restauración que llevarías a cabo el
viernes tras caer en la cuenta de los errores generados durante la
semana, simulados anteriormente. El proceso debe permitir recuperar
con éxito todos los ficheros modificados/borrados erróneamente.
(NOTA: En lugar de utilizar días de la semana reales, realiza las modificaciones
necesarias para cumplir cada escenario y lanza manualmente la copia de
seguridad que proceda en cada caso).

2. Realiza los siguientes apartados relativos a Sistemas RAID en Windows,
documentando los apartados b, c, d, e y f:

a. En una máquina virtual que tenga instalado Windows 11 Education Pro,
crea dos nuevos discos virtuales de 10 GB cada uno. Una vez arrancado
Windows, utilizando la herramienta “Administración de discos”, inicializa
cada uno de los dos discos como “Disco Dinámico” y realiza lo siguiente:

b. Crea un volumen simple de 1 GB.

c. Crea un volumen distribuido en dos discos (1 GB y 2 GB,
respectivamente).

d. Crea un volumen seccionado formado por dos discos de 4 GB cada uno.

e. Crea un volumen reflejado de 4 GB.

f. Copia algunos ficheros dentro de cada uno de los diferentes volúmenes
creados, desconecta el segundo disco virtual e indica qué ha pasado con
esos datos (si están disponibles o no) en cada uno de los volúmenes. Crea
un esquema o tabla que describa el comportamiento que ha tenido cada
uno de los volúmenes tras la desconexión del segundo disco virtual.¿Cuál
se ha comportado como un RAID0 y cuál como un RAID1?. Justifica tus
respuestas.

3. Realiza los siguientes apartados relativos a Sistemas RAID en Ubuntu Linux,
documentando los apartados b, c, d y f:
a. En una máquina virtual que tenga instalado Ubuntu Linux, crea tres
nuevos discos virtuales de 10 GB cada uno. Investiga sobre el uso de la
herramienta MDADM y configura lo siguiente:

b. Un RAID 0 que utilice dos discos virtuales de 10 GB cada uno.

c. Un RAID 1 que utilice dos discos virtuales de 10 GB cada uno.

d. Un RAID 5 que utilice tres discos virtuales de 10 GB cada uno.

e. Una vez creada cada unidad RAID, copia algunos ficheros dentro de ella,
desconecta uno de los discos virtuales que la forman y comprueba qué ha
pasado con esos datos.

f. Crea un esquema o tabla que describa el comportamiento que ha tenido
cada una de las unidades RAID creadas: discos necesarios, espacio
disponible, tolerancia al fallo de un disco, etc.
