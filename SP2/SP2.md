
<h1>Sistemas de fitxers  i patricions</h1>

<div>
  <i> <b>Definicions:</b> </i>
<ul><li><i>- Fragmentació interna:</i>
Es cuán los blocs son mas grans ...i se aprofita del disc</li> 

<li><i>-Fragmentació externa:</i>
Es cuán un archiu en blocs consecutius de la memoris i el seu accesos son mas lents i per tant baixa el rendiment</li></ul>
</div>

<div>
 <i> <b>Tipo de formateig </b> </i>
  <ul><li>-Baix nivell
Si que borra fitxers , sistema de fitxers , i intenta arreglar sectors defectuosos pero necesitem programes especifics , no es podem feu con el sistema opertaiu </li><li>-Mig nivell
format lent , si troba sistema defectuosos intenta marcarlos pero no los repara</li>
  <li>-Alt nivel :format rapid , no as borrar el archou no mes es borra el sistema de fitxers , sectors defectusos los eleminan</li></ul>
</div>


<h2>Gestió de particions</h2>
<ul>
  <li>Gparted</li>
    <li>Comandes</li>
    <li>Gestió de procesos</li>
  <li>Gestió d'usuaris i grups i permisos</li>
  <li>Copies de seguretat i automatizació de tasques</li>
<li>Quotes d'usuari</li>
</ul>

---------------------------------------------------------------------------------------------------
<h2>Disco 10Gb :</h2>
<img width="826" height="530" alt="image" src="https://github.com/user-attachments/assets/b14c5e39-82f1-420a-b589-8c8774d43d80" />

<h2>Mida de sector:</h2> 
<p>Definició: unitat minima fisica on se guarden los dades en un disco : por defecte : 512 bytes no la podem modificar.</p>
<img width="823" height="588" alt="image" src="https://github.com/user-attachments/assets/c02a27bb-0ee5-4b93-a92c-4baaaaf8dc44" />


<h2>block size : </h2> 
<p>- mida block
blocks para linux - cluster para windows : mitad minima logica on se guarden les dades a nivel de sistema operatiu : por defecte 4096 bytes (8 sectors) i esta mida sí que la podem cambiar cuan se formatem la partició i cada partició del disc pod detenir un medida de bloc i un sistema de fitxers diferent</p>
<img width="829" height="129" alt="image" src="https://github.com/user-attachments/assets/5f92a096-becd-4852-a901-513173321d48" />

<h2>particions : </h2> 
<img width="829" height="633" alt="image" src="https://github.com/user-attachments/assets/a8a14b13-29ee-4739-81db-f20883525458" />

<h2>sistema de fitxers:</h2> 
<p>sistemes de fitxers : 
Cada sistemes de fitxers te unes limitacions 
windows ntfs fat32
ubuntu ext4</p>
<img width="831" height="184" alt="image" src="https://github.com/user-attachments/assets/42fea851-a4c3-4fd8-9ec5-65299c11c2c5" />

<h2>fitxet hola.txt y cuanto ocupa realment en el OS:</h2> 
<img width="801" height="197" alt="image" src="https://github.com/user-attachments/assets/ae917ae5-109f-4f6c-8b60-333055805d18" />
---------------------------------------------------------------------------------------------------
<h2>gparted : </h2>
<img width="799" height="561" alt="image" src="https://github.com/user-attachments/assets/5a04bc1a-8158-49e9-8dbe-a360df1c1299" />
<p>Definicions:
- El g parted sive para asinar particions 
- Una partició es un tros físic del disc dur y amb el gparted podem gestionar particions pero no podeu modificar la mida del bloc 
- Volúm : es una capa de abstracció que esposa de amun de les particions io discos </p>


<h2> Comandes para particions ...: </h2>
<p>  el meu disc es :  /dev/sdb: 10Gib </p>
 <img width="821" height="169" alt="image" src="https://github.com/user-attachments/assets/bbb9b831-ff10-4322-99a7-5d99ac04d0c7" />
<p> creí particion (mitad del tamaño del meu disc )</p>
 <img width="822" height="295" alt="image" src="https://github.com/user-attachments/assets/2cbb2ac3-4903-4237-af85-1060209bbd26" />
 <img width="828" height="494" alt="image" src="https://github.com/user-attachments/assets/ac40730b-10b3-4797-8637-e6bbb37fda80" />
-------------------------------------------------------------------------------------------------

 <img width="887" height="193" alt="image" src="https://github.com/user-attachments/assets/9e3706d2-3ee8-4210-b2e4-17b7970d291d" />
<img width="782" height="497" alt="image" src="https://github.com/user-attachments/assets/00da88aa-ee32-4230-bf15-60d2c1ef8d1e" />

<h2>creació carpetas, archivos dentro del disc y no se guarda en el mismo disco:</h2>
<img width="827" height="555" alt="image" src="https://github.com/user-attachments/assets/1bde6b61-e469-4b91-a106-f748c919da15" />

<img width="797" height="414" alt="image" src="https://github.com/user-attachments/assets/46dfafb1-5a5e-461d-a600-1f4a58962fc1" />
<img width="836" height="608" alt="image" src="https://github.com/user-attachments/assets/f1406ae9-9a7c-4e94-8b8e-6de47e81b077" />

<img width="642" height="253" alt="image" src="https://github.com/user-attachments/assets/9c46ea03-6454-4fbd-a81e-6856a512b0f1" />
<img width="835" height="686" alt="image" src="https://github.com/user-attachments/assets/19d904ca-3354-41bc-a720-e5447696ac32" />

<h1>Usuarios y permisos :</h1>

Cuando ejecutamos un programa en nuestro sistema operativo, este se convierte en un **proceso**. El sistema operativo es el encargado de administrar estos procesos, asignándoles recursos como tiempo de CPU y memoria RAM.

Cada proceso cuenta con características que lo identifican:

 <ul><li>PID (Process ID): Es un número único asignado a cada proceso dentro del sistema.</li><li> Usuario propietario: Es quien ha iniciado el proceso y define qué permisos tendrá ese programa. </li>
  <li>Estado: Un proceso puede estar activo (ejecutándose), en espera (durmiendo) o "zombie" (finalizado pero aún presente en la tabla de procesos)./li></ul>

Para administrar los procesos desde la terminal, disponemos de varios comandos:

<ul>
<li><"ps" / "top" : Visualizació ; Nos permiten visualizar los procesos activos y su consumo de recursos en tiempo real. /li>
<li>"kill" : Finalizació; Se utiliza para enviar señales a los procesos, generalmente para detenerlos o forzar su cierre (requiere el PID). </li>
<li>"nice" / "renice" : Modifican la prioridad de un proceso para que el sistema le dé más o menos preferencia de CPU. </li>
<li>"systemctl" : Es la herramienta principal para gestionar servicios (daemons) que corren en segundo plano (arrancar, parar, reiniciar). </li>
</ul>
<h1> Gestión de usuario, gruposy permisos :</h1>
En Linux, la administración de usuarios es crítica para la seguridad. Toda la información referente a usuarios y grupos se almacena en archivos de texto plano que podemos consultar.
  
<h2> Interfaz alternativa </h2>
  
Aunque la administración de servidores Linux se realiza principalmente mediante comandos, existen herramientas gráficas para facilitar esta tarea en entornos de escritorio. Una de las más clásicas es `gnome-system-tools`.

Como esta herramienta no siempre viene instalada por defecto en las versiones modernas de Ubuntu, primero debemos instalarla: `sudo apt install gnome-system-tools`
Una vez instalada, podemos ejecutarla para ver una interfaz amigable donde añadir o modificar usuarioscon el comando : 'users-admin'
<img width="729" height="543" alt="image" src="https://github.com/user-attachments/assets/eb8e0f34-0440-42fe-b319-936d9a273d8a" />

  
<h2>Archivos principales del sistema</h2>

El archivo **/etc/passwd** contiene el listado de todos los usuarios del sistema, indicando su UID, GID y su directorio personal (home).

<h3>Visualización del contenido donde se definen los usuarios:</h3>
<img width="657" height="142" alt="image" src="https://github.com/user-attachments/assets/2eea0d0c-73f3-44f3-b473-fd2fc2243129" />
<img width="757" height="710" alt="image" src="https://github.com/user-attachments/assets/1d1157b5-a88e-4fd9-9d58-9ca241650872" /> 
<h3>Listado de los grupos configurados en el sistema : </h3>

<img width="623" height="781" alt="image" src="https://github.com/user-attachments/assets/b851acc6-bdf6-489d-8b40-72249f48c2d8" />
El archivo '/etc/group' define los grupos existentes en el sistema y qué usuarios pertenecen a cada uno.Por motivos de seguridad, las contraseñas no son visibles en el archivo general. Se almacenan cifradas en el archivo /etc/shadow, el cual solo puede ser leído por el usuario root. Aquí también se configuran las políticas de caducidad de las claves.

<h3>Contenido de las contraseñas encriptadas con privilegios root </h3>
<img width="621" height="339" alt="image" src="https://github.com/user-attachments/assets/8d464740-e89f-4004-97c9-ed2dd9809b28" />
<img width="859" height="192" alt="image" src="https://github.com/user-attachments/assets/1f366a33-78b3-485b-b9c9-b6b57ca6ea4c" />

<h2>Comandos para la Gestión de Usuarios</h2>
<h3>Creación de un usuario utilizando el asistente interactivo. </h3>

Existen dos herramientas principales para dar de alta usuarios:
1.  adduser: Es un asistente interactivo ;script de Perl; que solicita los datos paso a paso y crea automáticamente el directorio personal. Es más amigable.
2.  useradd: Es el comando nativo ;binario; más rápido y manual, ideal para scripts, pero no configura tantas opciones por defecto.

Ejemplo de creación con 'adduser':
<img width="794" height="592" alt="image" src="https://github.com/user-attachments/assets/f07fd4be-bbb7-4d9f-9e77-ee4e49fe369f" />
Una vez creado, podemos verificar que su directorio /home se ha generado correctamente.
<img width="599" height="80" alt="image" src="https://github.com/user-attachments/assets/d1a2af45-4ef8-4bf6-9cd3-885eb1fc91c3" />

<h3>Gestión del estado de la cuenta: bloqueo o eliminación: </h3>
También podemos bloquear temporalmente el acceso de un usuario (sin eliminarlo) usando `passwd -l`, o borrarlo definitivamente con `deluser`.
<img width="787" height="237" alt="image" src="https://github.com/user-attachments/assets/b96f3bfa-3ca9-49fb-9f54-06b6792fc77d" />

<h2>Preparación del Entorno :Usuarios y Directorios :</h2>

Para poner en práctica la teoría, vamos a simular un entorno de trabajo real. En este ejercicio crearemos un grupo de trabajo y varios usuarios, y gestionaremos el acceso a una carpeta compartida.

<h3>Creación de Usuarios y Grupos :</h3>
Primero, creamos el grupo `paloma` y los usuarios que utilizaremos para las pruebas (`nick`, `cire`, `ferran`, `deivy`).
<img width="759" height="463" alt="image" src="https://github.com/user-attachments/assets/7c057b68-76fc-4fa6-ac21-52054de92e91" />
<img width="822" height="733" alt="image" src="https://github.com/user-attachments/assets/4b0ddb75-907c-48d2-ae8c-65d52443f981" />
<img width="835" height="714" alt="image" src="https://github.com/user-attachments/assets/943fc03a-562a-4bd1-82d5-ba519984d9c2" />

<h3>Creación del Directorio de Trabajo : </h3> 

Creamos un directorio en `/var/` llamado `palomes` que servirá como carpeta compartida.
<img width="873" height="127" alt="image" src="https://github.com/user-attachments/assets/b4766fd3-fd1b-476e-9665-9341295188f3" />

<h3>Cambio de Propietarios :CHOWN:</h3> 

Por defecto, al crear la carpeta con `sudo`, el propietario es *root*. Vamos a cambiarlo para que el usuario `nick` sea el dueño y el grupo propietario sea `paloma` (o el grupo de nick, según decidamos).

El comando `chown` (Change Owner) nos permite cambiar usuario y grupo simultáneamente.
<img width="678" height="209" alt="image" src="https://github.com/user-attachments/assets/19a45e7c-d0d9-4874-a051-501abd1ccd6b" />

<h3>Restricción de Permisos:CHMOD:</h3>

Vamos a configurar permisos más estrictos. Usaremos `chmod 750`:
  7 (Dueño - nick):Lectura, escritura y ejecución (rwx).
  5 (Grupo):Lectura y ejecución (r-x).
  0 (Otros): Ningún permiso.

Esto significa que los usuarios que no sean `nick` ni pertenezcan a su grupo, no podrán ni siquiera entrar.
<img width="609" height="162" alt="image" src="https://github.com/user-attachments/assets/e1383d8b-225b-44ea-b9a7-76169eed6ddb" />
Ahora, permitiremos que el grupo pueda escribir en la carpeta modificando los permisos con "g+w" (Group + Write).
<img width="706" height="223" alt="image" src="https://github.com/user-attachments/assets/6a6daf5a-a3c1-4ec6-a022-372c5e99aa2b" />

<h2>Permisos Especiales:</h2>
  <h3>Sticky Bit :</h3>
  
En directorios compartidos donde varios usuarios tienen permiso de escritura (como hemos hecho antes), existe un problema: un usuario podría borrar los archivos de otro compañero por accidente o malicia.
Para evitar esto, activamos el Sticky Bit.
<img width="574" height="113" alt="image" src="https://github.com/user-attachments/assets/da0b98e8-5e8d-4729-b33b-de270b24cbde" />
Con el Sticky Bit activo, aunque tengamos permisos totales sobre la carpeta, el sistema nos impedirá borrar un archivo que no sea nuestro.
<img width="882" height="374" alt="image" src="https://github.com/user-attachments/assets/52846f9a-4add-4554-8fed-edbdd97b3cff" />

<h3>SUID y SGID: </h3>
Además del Sticky Bit, existen otros dos permisos especiales que cambian el comportamiento de ejecución y propiedad: SUID y SGID.
SUID: El bit SUID (Set User ID) normalmente se usa en archivos ejecutables. Permite que, cuando un usuario ejecute un programa, este funcione con los permisos del propietario del archivo y no con los del usuario que lo lanza.
* Se activa sumando 4 en octal o usando `u+s`.
* En el listado se ve como una `s` en la parte del propietario.
<img width="586" height="104" alt="image" src="https://github.com/user-attachments/assets/38fd73aa-2b55-4158-a6b0-8cd644ce5749" />

SGID :El bit SGID (Set Group ID) es muy útil en carpetas compartidas. Si lo activamos en un directorio, cualquier archivo nuevo que se cree dentro heredará automáticamente el grupo de ese directorio, en lugar del grupo principal del usuario que lo crea. Esto facilita mucho el trabajo en equipo.
* Se activa sumando 2 en octal o usando `g+s`.
* En el listado se ve como una `s` en la parte del grupo.
<img width="613" height="109" alt="image" src="https://github.com/user-attachments/assets/20acc4dc-4f4e-4f95-bf4a-c70f1c2a8e23" />

<h2>Listas de Control de Acceso (ACLs) y Umask :</h2> 

Para finalizar la gestión de permisos, existen situaciones donde los permisos estándar (Dueño/Grupo/Otros) no son suficientes. Por ejemplo, si queremos dar permiso a un solo usuario específico sin añadirlo al grupo.

Las ACLs nos permiten asignar permisos granulares a usuarios o grupos concretos sobre un archivo o directorio.
<img width="902" height="435" alt="image" src="https://github.com/user-attachments/assets/b9016770-6bac-4a0c-bcbc-f0f94c5c1063" />

Finalmente, el **umask** es una variable de entorno que determina los permisos por defecto que tendrá cualquier archivo o carpeta nueva que creemos.

Funciona restando valor a los permisos totales (666 para archivos, 777 para directorios). Por ejemplo, un umask de `0022` hace que los archivos nazcan con `644` (se quita el permiso de escritura al grupo y a otros).
<img width="538" height="125" alt="image" src="https://github.com/user-attachments/assets/b96958eb-9f7a-4bbe-ba79-e9f2a5f2b6b4" />


