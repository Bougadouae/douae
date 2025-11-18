<h1>Sistemas de fitxers  i patricions</h1>

<p>
  Definicions:
  - fragmentacio interna
fragmentacio interna : cuan los blocs son mas grans ...i se aprofita del disc

- .... externa
es cuan un archiu en blocs consecutius de la memoris i el seu accesos son mas lents i per tant baixa el rendiment</p>
------------------------------------------------------------------------------------------
<p>tipo de formateig
-baix nivell
si que borra fitxers , sistema de fitxers , i intenta arreglar sectors defectuosos pero necesitem programes especifics , no es podem feu con el sistema opertaiu 
-mig nivell
format lent , si troba sistema defectuosos intenta marcarlos pero no los repara
-alt nivel :format rapid , no as borrar el archou no mes es borra el sistema de fitxers , sectors defectusos los eleminan</p>
--------------------------------------------------------------------------------------------

gestio de particions
-gparted
-comandes
--gestio de procesos
--gestio d'usuaris i grups i permisos
--copies de seguretat i automatizació de tasques
--Quotes d'usuari

---------------------------------------------------------------------------------------------------
<h2>disco 10Gb :</h2>
<img width="826" height="530" alt="image" src="https://github.com/user-attachments/assets/b14c5e39-82f1-420a-b589-8c8774d43d80" />

<h2>mida de sector:</h2> 
<p>- mida sector: unitat minima fisica on se guarden los dades en un disco : por defecte : 512 bytes no la podem modificar</p>
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

__________________________________________________
<h1>Usuarios y permisos :</h1>


