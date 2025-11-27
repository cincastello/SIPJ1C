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


Fem: apt install gnome-system-tools, i aquí tenim el nostre usuari nom:contrasenya en un altre fitxer:id_usuari_id_grup_principal:

Fitxers implicats (3 passos, 1.passwd, 2.group, 3.shadow(4.gshadow))
Comandes bàsiques
Personalització de comandes


<img width="655" height="333" alt="image" src="https://github.com/user-attachments/assets/36d090db-9697-4c49-9199-54ce833915fe" />













