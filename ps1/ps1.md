---
layout: default
title: "Unidad 1. Fundamentos de la Inteligencia Artificial y el Aprendizaje Automático"
---

## Virtualització i instal·lació del SO Ubuntu



Requisits mínims:
<img width="901" height="555" alt="image" src="https://github.com/user-attachments/assets/e6baeb52-78b9-4355-b9fe-03decb93530c" />


Implementació dels requisits mínims:

<img width="722" height="738" alt="image" src="https://github.com/user-attachments/assets/32f24752-c24f-4911-a371-45c6a3030bff" />


## Procés d'instal·lació: 

<img width="725" height="485" alt="image" src="https://github.com/user-attachments/assets/d93a2475-3d94-4daa-a77c-04e85f5af109" />

<img width="860" height="625" alt="image" src="https://github.com/user-attachments/assets/64124d3a-74f4-48c9-b5b7-33b6b376be90" />

Sel·leccionem install Ubuntu.

<img width="863" height="700" alt="image" src="https://github.com/user-attachments/assets/850ca355-aeb7-424f-ba3d-776aca5bf3e4" />

<img width="863" height="700" alt="image" src="https://github.com/user-attachments/assets/e825fdbb-7bc6-4e8f-9664-217cb7ce38ac" />

<img width="863" height="700" alt="image" src="https://github.com/user-attachments/assets/21e7d611-4ab8-4bad-b075-ea598e97f168" />


A contiuació ens apareixera un lloc per registrar-nos, on haurem de ficar-nos un usuari i una contrasenya. Ho fem i polsem instal·lar.


Per poder fer les particions seleccionem free space i veurem que en s deixa polsar el signe +, ho fem i allí seleccionem el que natros necessitem.

Per exemple, jo he usat el Ext4journaling file system per a totes les particions. I, a partir d'allí he fet 3 particions: /(20GB: per tenir prou espai per al sistema i programes), home(16GB: perquè estaran totes les dades nostres), boot(4GB, conté el Kernel i el arrancada) i swap(2GB: per la memòria virtual)(Aquí no he usat el Ext4journaling file system ja que he usat el swap area per poder tenir-lo).

<img width="860" height="625" alt="image" src="https://github.com/user-attachments/assets/43957993-95d5-44ed-ae4c-4c986ac3fe72" />


I ja ho tenim instal·lat:







### Llicenciament

<img width="817" height="459" alt="image" src="https://github.com/user-attachments/assets/5fa5c9b1-1130-4e93-8837-62a1e112e7b1" />
A continuació explicaré el que hem pogut observar en la imatge anterior sobre les llicències típiques d'Ubuntu i quines són:
- GPL = és la més usada a Linux, ja que obliga a compartir el codi en cas de distribució.
- LGPL = és més flexible que l'anterior però més sensible per a les biblioteques.
- Apache, BSD, Artistic, MPL = són més permissives i deixen barrejar amb programari privatiu.
- GFDL = per la documentació
- CC0 = és domini públic (sense restriccions)

En resum, ninguna és la principal, no obstant la més usada de les ja mostrades seria la GPL.

## Instal·lacions duals i Gestors d'arrencada
## Particions i punts de restauració
## Cofiguració bàsica de la xarxa
## Comandes generals i instal·lació d'aplicacions

