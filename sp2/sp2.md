---
layout: default
title: "Cursos de Sistemes informàtics"
---

## Gestió de la Informació del Sistema i Administracions



SISTEMES DE FITXERS I PARTICIONS


·Mida del sector:

Un sector és l’unitat mínima fisica on es guarden les dades al disc(512 bytes per defecte i en principi no es pot modificar). 

<img width="660" height="455" alt="image" src="https://github.com/user-attachments/assets/f6f516b9-77b0-4aa1-9209-f092c8672d21" />


·Mida del block:

Unitat mínima lògica de com es guarden les dades a nivell de sistema operatiu(4096 bytes per defecte de mida i esta si es pot modificar(quan formatem la partició))

Mida block de la partició

<img width="588" height="98" alt="image" src="https://github.com/user-attachments/assets/071bb1bf-c825-45d9-b140-259fa2eeb719" />

du = mida fitxer en bytes
Amb la primera comanda ens diu el que ocupa:

<img width="572" height="242" alt="image" src="https://github.com/user-attachments/assets/c3df4ad0-6360-42d4-8319-bd05bd713d3c" />


Per saber si hem de desfragmentar:

<img width="659" height="377" alt="image" src="https://github.com/user-attachments/assets/0df4a249-e01c-44f1-bdfe-1d39fc6f13f8" />


Per desfragmentar:

<img width="659" height="377" alt="image" src="https://github.com/user-attachments/assets/2939ee62-87bd-4c89-9491-3941bc170435" />



·Fragmentació interna:

Espai de disc desaprofitat pq als blocks sobra molt espai per les coses que guardem ((per resoldre:)els podem fer més reduïts però tenen que tenir la mida de múltiples de 512 no tindrem fragmentació interna però el rendiment serà més lent)(ho fem quan formatem la partició)(trobar equilibri entre fragmentació i rendiment)


·Fragmentació externa:

És quan a mesura q treballa amb el sistem aoperatiu els arxius no queden guardats en blocks continus de memòria i llavors el rendiment baixa, entre altres. (per resoldre:)(en windows tenim el desfragmentador per reduir la fragmentació externa i en linux es diu q el seu sistema de fitxers és tan bo q no cal passar cap fragmentador


·Tipus de sistemes de fitxers:

Hi han molts, per a windows(+ coneguts=fat32, ntfs) i linux(+ coneguts = ext4)
- Depenent de quin usem hi podrà accedir un cert sistema operatiu o sistemes
- La mida dels blocs
- La mida dels arxius
- Noms dels arxius
- Rendiment
etc


·En que influeix usar un o un altre?

· Tipus de formateig:

Tenim 3 tipus (alt nivell(característiques:(és el ràpid) quan formatem a traves del so no es borren els arxiu q hi havien sino el sistema de fitxers)(el recuva recupera els arxius), baix nivell(característiques:es borra TOT, intenta reparar un sector defectuós) i mig nivell(característiques el mateix q el ràpid i mira si hi ha algun sector defectuós però sol ho diu i no fa res))

- Particions/volums

Una partició es un tros de disc q ocupa espai a nivell físic.

El volum és una capa d’abstracció q es fica damunt les particions a nivell lògic, agrupació de particions o discos on a partir d’allí es poden fer més particions per treballar més còmodament.

Part pràctica:

<img width="659" height="377" alt="image" src="https://github.com/user-attachments/assets/9a2623c0-c8d0-4654-819f-de22d6eeba60" />


Apartat de comandes:

<img width="585" height="104" alt="image" src="https://github.com/user-attachments/assets/9b441407-7a25-49cd-bef4-5617a5d482b6" />

<img width="597" height="350" alt="image" src="https://github.com/user-attachments/assets/18c419fd-6fae-4a81-8d7d-15f0c1c665fd" />

<img width="591" height="347" alt="image" src="https://github.com/user-attachments/assets/fc0adc31-e481-40ff-b5a0-2b7f75304e5b" />

<img width="476" height="159" alt="image" src="https://github.com/user-attachments/assets/ca69ba2e-c7ff-4662-876b-4dd5ff221460" />


Amb el gparted no es pot canviar la mida de bloc sol amb comandes


<img width="591" height="250" alt="image" src="https://github.com/user-attachments/assets/257d9a74-7d22-4982-bc33-c9c08ba21756" />


Per reduir


<img width="588" height="342" alt="image" src="https://github.com/user-attachments/assets/5d9dd93c-cdea-4b7d-8fbe-9bf0ca755a15" />


- GPARTED


<img width="605" height="72" alt="image" src="https://github.com/user-attachments/assets/8cdbb770-a416-4fcc-9179-4774a26ea095" />


- Comandes

<img width="637" height="289" alt="image" src="https://github.com/user-attachments/assets/c6291420-57a9-40e5-88e8-2b2eecc64685" />

<img width="650" height="292" alt="image" src="https://github.com/user-attachments/assets/7a8a75be-8731-454e-8e35-e9e2059c7fc4" />

<img width="650" height="292" alt="image" src="https://github.com/user-attachments/assets/6f8966be-77ad-4297-9cbb-d6acef419684" />

<img width="484" height="132" alt="image" src="https://github.com/user-attachments/assets/9593b9b8-5cd6-49b2-acaf-9ce26f08a1ae" />

<img width="656" height="262" alt="image" src="https://github.com/user-attachments/assets/3582f247-2024-45d9-80d3-86d1dc745c9a" />

<img width="550" height="201" alt="image" src="https://github.com/user-attachments/assets/114c00ac-46a9-4d9e-88cf-67950509d01f" />



Un sector és l’unitat mínima fisica on es guarden les dades al disc (de 512 bytes per defecte i en principi no es pot modificar). 


Fitxers implicats (3 passos, 1.passwd, 2.group, 3.shadow(4.gshadow))

nano gro
nano group
nano shadow: tot el q fa referent a les contres, dates de caducitat, etc
nano gshadow

Comandes bàsiques

Personalització de comandes

Fem: apt install gnome-system-tools, i aquí tenim el nostre usuari nom:contrasenya en un altre fitxer:id_usuari_id_grup_principal:

És el fitxer central que conté la informació de tots els usuaris en sistemes Linux.


<img width="655" height="333" alt="image" src="https://github.com/user-attachments/assets/36d090db-9697-4c49-9199-54ce833915fe" />

Nom ususari. git number(grup principal q te assignat l’usuari).


Password en un altre fitxer:

<img width="655" height="333" alt="image" src="https://github.com/user-attachments/assets/0377ac7c-f85f-4708-ab79-ebdc90eb9ca1" />

Caducitats i tot el que hem fet respecte a les contres, tots usuaris que formen part del grup

id del usuari

aquí es veu el de dalt i qui es el usuari admin d’aquell grup

<img width="652" height="350" alt="image" src="https://github.com/user-attachments/assets/c0f17d39-98e4-427f-a53e-28c95ddf7c2f" />

id grup prinicpal del usuari

<img width="652" height="387" alt="image" src="https://github.com/user-attachments/assets/d993cf99-efb3-4544-8172-1742bbc30119" />

<img width="323" height="72" alt="image" src="https://github.com/user-attachments/assets/6ab40d42-aec5-47cf-8834-730daf4cce43" />

<img width="526" height="82" alt="image" src="https://github.com/user-attachments/assets/6effe737-d240-4645-9af5-2262fde1b23d" />


Fins q no iniciem sessió al nou usuari no podem fer canvis des de el principal

Chown per canviar usuari propietari del grup


Anem a crear un usuari nou anomenat "vesper". Primer li assignem una contrasenya, però el sistema ens avisa que és massa curta, de manera que n'hem d'escollir una de més llarga.

A continuació, comprovem que l'usuari tingui la shell bash configurada, i mitjançant una ordre li assignem aquesta shell perquè pugui utilitzar-la.

També hem de crear manualment la carpeta personal a /home/vesper i assignar-ne la propietat a l'usuari, ja que a vegades aquesta carpeta no es crea automàticament.

Finalment, ja tenim l'usuari "vesper" configurat i preparat per a ser utilitzat, amb la seva carpeta personal i la shell bash correctament assignades.


<img width="628" height="468" alt="image" src="https://github.com/user-attachments/assets/3333433f-f423-4c1e-bb6d-c467d6edd7a9" />

<img width="267" height="47" alt="image" src="https://github.com/user-attachments/assets/823e6649-1b19-46ed-9d58-26a1cafe590b" />

Usem usermod per modificar usuaris existents
Després d’entrar gràficament a l’altre usuari es creen les carpetes

Per eliminar usuari:
- deluser
- userdel


<img width="477" height="343" alt="image" src="https://github.com/user-attachments/assets/8ff24e78-72ba-42a0-b354-db8c6ffd33bb" />

<img width="623" height="349" alt="image" src="https://github.com/user-attachments/assets/c4d1582c-4e2a-4d27-844e-adb5b1b3d632" />


Per bloquejar-lo:


<img width="654" height="125" alt="image" src="https://github.com/user-attachments/assets/711c9bd4-4295-4472-b9f2-276cfe93fd1d" />


Per desbloquejar-lo fiquem una U:


<img width="668" height="78" alt="image" src="https://github.com/user-attachments/assets/0c772a95-56c4-48a9-a775-4d4c0598c2c0" />


Així fem un grup:


<img width="502" height="66" alt="image" src="https://github.com/user-attachments/assets/4558e115-fbd1-468f-b3e6-72c291460e73" />

<img width="593" height="27" alt="image" src="https://github.com/user-attachments/assets/6d3e7ba8-7767-4182-9765-cc5d11690ea3" />

<img width="618" height="41" alt="image" src="https://github.com/user-attachments/assets/6896f035-6af7-4295-bab1-cd237049d615" />


Així s’afegeix un usuari de 3 formes diferents:

<img width="570" height="239" alt="image" src="https://github.com/user-attachments/assets/b38ec3fb-c26d-41c2-addc-f326bf258a9f" />

<img width="584" height="49" alt="image" src="https://github.com/user-attachments/assets/e0b652a1-9edd-4fc0-9363-dc37cd502f2b" />

<img width="608" height="47" alt="image" src="https://github.com/user-attachments/assets/c936918f-3f45-459b-95e2-8f2b769b8472" />

<img width="646" height="371" alt="image" src="https://github.com/user-attachments/assets/efda9a93-20f4-49dc-94cc-a033e7b180cf" />


Per treure un usuari d’un grup:


<img width="551" height="72" alt="image" src="https://github.com/user-attachments/assets/f944525d-7787-494d-aa5e-d182371d0832" />


Segona manera:


<img width="577" height="71" alt="image" src="https://github.com/user-attachments/assets/5f140341-4ad2-494d-9de0-2f1c27e882db" />


Modifica el grup principal de l’usuari:


<img width="607" height="74" alt="image" src="https://github.com/user-attachments/assets/1691bb8a-87f7-40b9-ba7a-50d3065e17d4" />

<img width="450" height="22" alt="image" src="https://github.com/user-attachments/assets/f01b91ee-184d-43f2-aef6-567287a1d009" />


Per comprovar:


<img width="625" height="66" alt="image" src="https://github.com/user-attachments/assets/051063ec-a855-4cf2-94fc-9e6f2d147513" />

<img width="642" height="156" alt="image" src="https://github.com/user-attachments/assets/616bab86-e37a-4c4c-ac7d-20914e5bcd38" />

<img width="482" height="25" alt="image" src="https://github.com/user-attachments/assets/ee486c9c-ffcb-429a-b92b-d31449d81bd4" />

Et diu els grups dels q forma part l’usuari:

<img width="482" height="21" alt="image" src="https://github.com/user-attachments/assets/2b0ba6f5-8dea-49e9-b9ec-fbf3d89e0174" />


Per esborrar un grup:

<img width="635" height="198" alt="image" src="https://github.com/user-attachments/assets/d3c5884c-d8df-43cb-8359-ce94338f51f4" />

<img width="376" height="25" alt="image" src="https://github.com/user-attachments/assets/fb4f9046-8c6e-401e-927b-a0db069b2c87" />


Si està assignat com a principal d’un usuari no ens el deixarà borrar així que haurem de reasignar el grup principal al usuari amb usermod -g prova4 prova4 i després ho comprovem amb groupdel proves per veure si ens el deixa provar.


<img width="442" height="23" alt="image" src="https://github.com/user-attachments/assets/f4eb4aa3-d71d-4533-a1fd-32c0d47cf887" />

<img width="442" height="23" alt="image" src="https://github.com/user-attachments/assets/9221361d-be75-4288-863e-e6236799adb3" />


Arxius ocults perquè tenen punt:

<img width="587" height="171" alt="image" src="https://github.com/user-attachments/assets/33a41888-e753-474b-b005-4c33d77d331f" />


Es copien a tots els usuaris, si el modifico tb passarà als altres usuaris, llavors pa editar algo de un ho farem a la home i no al skel. Així:


<img width="587" height="171" alt="image" src="https://github.com/user-attachments/assets/86bda4d9-b95b-4145-ae5b-055eb470f6ea" />


Canviem l’inici dels UID i el GID per a que comencin al número 2000

<img width="636" height="344" alt="image" src="https://github.com/user-attachments/assets/e7870ac0-ee50-4768-a0e0-56cf89b2d1a3" />

<img width="550" height="295" alt="image" src="https://github.com/user-attachments/assets/86a70d21-1833-4187-8715-7e47e8ee38ea" />


Per canviar la configuració dels usuaris nous:


<img width="550" height="295" alt="image" src="https://github.com/user-attachments/assets/c89f2ce1-b7b8-4c79-9ed6-4513b6e441a1" />

<img width="550" height="311" alt="image" src="https://github.com/user-attachments/assets/1f4ac38f-5801-4c9a-aa66-6d30c293e430" />

(per canviar la forma d’accedir al home)


Les comandes usades:


<img width="585" height="78" alt="image" src="https://github.com/user-attachments/assets/8362bdc6-a9a3-4570-85c2-3df3bbe0a2c5" />


Ha funcionat:


<img width="644" height="261" alt="image" src="https://github.com/user-attachments/assets/f46fa3f4-b8a8-456d-87bf-8d1af189442b" />



En useradd no se li crea una home automàticament


<img width="521" height="98" alt="image" src="https://github.com/user-attachments/assets/94ccd17c-fda3-42aa-b65f-43a56096a100" />


CONFIGURACIÓ PER A ADDUSER I USERADD:


<img width="629" height="134" alt="image" src="https://github.com/user-attachments/assets/0c68a209-f8e0-4e75-a1ef-8709d8941bad" />


Canviem el tipus de shell de bin bash a bin fish i el nom per accedir al home.

<img width="592" height="39" alt="image" src="https://github.com/user-attachments/assets/fcdb69d3-3c50-45a1-bc5e-41cd6fce2a9c" />

<img width="592" height="43" alt="image" src="https://github.com/user-attachments/assets/3e4e7a8c-6507-4c95-9418-be93476aa47e" />

<img width="642" height="243" alt="image" src="https://github.com/user-attachments/assets/ef0082bb-e17d-42d4-af39-a785945d1a72" />




## Permisos
Part 1:

Part 2:
CÒPIES DE SEGURETAT I AUTOMATITZACIÓ DE TASQUES
1. Teoria Còpies de Seguretat
Explicació en taula:

<img width="620" height="598" alt="image" src="https://github.com/user-attachments/assets/2454ada9-4801-4c8f-baf5-5b4a8d6ffdee" />




Tipus:

<img width="619" height="579" alt="image" src="https://github.com/user-attachments/assets/53589252-55cc-4c23-be53-d79242d36aa7" />





2. Teoria comandes Backups:

<img width="628" height="290" alt="image" src="https://github.com/user-attachments/assets/38c9f716-3e23-460d-93c0-c70cbcd5f744" />




3. Pràctica comandes Backups:
   1. cp

      
      <img width="652" height="422" alt="image" src="https://github.com/user-attachments/assets/2a0cf541-88a1-42b7-b388-004b47efd377" />


   2. rsync


      <img width="652" height="422" alt="image" src="https://github.com/user-attachments/assets/84421864-da80-464c-b570-e5705d6de34b" />


   3. dd
  

      <img width="661" height="434" alt="image" src="https://github.com/user-attachments/assets/0af5829f-76e2-4dcf-b5fb-f580bbe3d80c" />



4. Pràctica programes backups
  1. Deja-Dup
  2. Duplicity




      

      


