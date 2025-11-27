---
layout: default
title: "Cursos de Sistemes informàtics"
---

## Gestió de la Informació del Sistema i Administracions



SISTEMES DE FITXERS I PARTICIONS


·Mida del sector:

Un sector és l’unitat mínima fisica on es guarden les dades al disc(512 bytes per defecte i en principi no es pot modificar). 


·Mida del block:

Unitat mínima lògica de com es guarden les dades a nivell de sistema operatiu(4096 bytes per defecte de mida i esta si es pot modificar(quan formatem la partició))


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
una partició es un tros de disc q ocupa espai a nivell físic
el volum és una capa d’abstracció q es fica damunt les particions a nivell lògic, agrupació de particions o discos on a partir d’allí es poden fer més particions per treballar més còmodament.
- GPARTED
- Comandes


Un sector és l’unitat mínima fisica on es guarden les dades al disc (de 512 bytes per defecte i en principi no es pot modificar). 







