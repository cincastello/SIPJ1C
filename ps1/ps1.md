---
layout: default
title: "Unidad 1. Fundamentos de la Inteligencia Artificial y el Aprendizaje Automático"
---

## Virtualització i instal·lació del SO Ubuntu



Requisits mínims:
<img width="901" height="555" alt="image" src="https://github.com/user-attachments/assets/e6baeb52-78b9-4355-b9fe-03decb93530c" />


Implementació dels requisits mínims:

<img width="629" height="753" alt="image" src="https://github.com/user-attachments/assets/f05ebfbf-bc8d-4805-9523-cb9d30384967" />



## Procés d'instal·lació: 

<img width="717" height="466" alt="image" src="https://github.com/user-attachments/assets/a3c14ec7-7e5e-44b2-9c56-3b71bdf689b6" />

<img width="860" height="625" alt="image" src="https://github.com/user-attachments/assets/64124d3a-74f4-48c9-b5b7-33b6b376be90" />

Sel·leccionem install Ubuntu.

<img width="863" height="700" alt="image" src="https://github.com/user-attachments/assets/850ca355-aeb7-424f-ba3d-776aca5bf3e4" />

Aquí elegim minimal installation i download updates while installing Ubuntu.
<img width="863" height="700" alt="image" src="https://github.com/user-attachments/assets/e825fdbb-7bc6-4e8f-9664-217cb7ce38ac" />

Aquí sel·leccionem something else.
<img width="863" height="700" alt="image" src="https://github.com/user-attachments/assets/21e7d611-4ab8-4bad-b075-ea598e97f168" />

<img width="826" height="596" alt="image" src="https://github.com/user-attachments/assets/1a381b59-32ed-4e14-89a3-d48338824b82" />



A contiuació ens apareixera un lloc per registrar-nos, on haurem de ficar-nos un usuari i una contrasenya. Ho fem i polsem instal·lar. Veurem això a la nostra pantalla:
<img width="826" height="596" alt="image" src="https://github.com/user-attachments/assets/d169fa1e-3445-4855-989c-413d17b4059a" />
<img width="826" height="596" alt="image" src="https://github.com/user-attachments/assets/874ab4e6-7fc3-45fd-b693-750909979951" />

I finalment veurem això:
<img width="826" height="596" alt="image" src="https://github.com/user-attachments/assets/0bf63974-e737-4321-9827-9ee9a276de1a" />

Polsem el botó que posa restart i esperem a que ens digui que polsem enter i ho fem. D'aquí obrim la nostra sessió.
Seguidament seleccionem free space i veurem que en s deixa polsar el signe +, ho fem i allí seleccionem el que natros necessitem.

Per exemple, jo he usat el Ext4journaling file system per a totes les particions. I, a partir d'allí he fet 3 particions: /(20GB: per tenir prou espai per al sistema i programes), home(16GB: perquè estaran totes les dades nostres), boot(4GB, conté el Kernel i el arrancada) i swap(2GB: per la memòria virtual)(Aquí no he usat el Ext4journaling file system ja que he usat el swap area per poder tenir-lo).

<img width="860" height="625" alt="image" src="https://github.com/user-attachments/assets/43957993-95d5-44ed-ae4c-4c986ac3fe72" />


I ja tenim Ubuntu instal·lat.

<img width="1294" height="804" alt="image" src="https://github.com/user-attachments/assets/0080f39e-c1f1-4d26-a05b-3f6d6ebf2b2c" />




## Instal·lació Windows
Seleccionem la nostra maquina i anem a paràmetres --> emmagatzematge --> <img width="259" height="57" alt="image" src="https://github.com/user-attachments/assets/97540f08-2fbe-4a51-ac58-9a90879c227e" /> --> polsem el disquet blau i sel·leccionem el windows, es veurà així: <img width="259" height="57" alt="image" src="https://github.com/user-attachments/assets/ffc7c11d-c737-4f05-a826-f275572774e7" /> --> guardem els canvi i tornem a la nostra màquina i l'obrim.




## Instal·lació del grub
Entrem a la màquina al Ubuntu i obrim terminal i seguim aquestes instruccions:
<img width="879" height="804" alt="image" src="https://github.com/user-attachments/assets/3b0bd66e-b84a-4fd7-8a4e-053507fe1599" />


El pas a pas es veu així:
<img width="596" height="390" alt="image" src="https://github.com/user-attachments/assets/772ae890-be11-4d92-9869-d076363d4f1a" />
<img width="596" height="390" alt="image" src="https://github.com/user-attachments/assets/723e76be-d8db-4ace-b5cc-8e2fc220549d" />
<img width="603" height="372" alt="image" src="https://github.com/user-attachments/assets/24d786de-5595-4295-9673-4190ffc47e20" />
<img width="420" height="22" alt="image" src="https://github.com/user-attachments/assets/6dfd377f-4794-4df6-a64e-ba170e2991f3" />
<img width="534" height="155" alt="image" src="https://github.com/user-attachments/assets/d65ad63d-db4a-4513-acd0-10f83d5b056a" />

Recordem el número que ens surt al sda del EFI per poder usar-lo a la següent comanda.

<img width="604" height="16" alt="image" src="https://github.com/user-attachments/assets/80c15d18-b3c7-4180-ae3c-833bd0f7717f" />
<img width="589" height="105" alt="image" src="https://github.com/user-attachments/assets/d5bbd70d-2b40-4f9d-a4d0-38deea10ee71" />
<img width="437" height="17" alt="image" src="https://github.com/user-attachments/assets/ac746ab2-3a1f-4b37-87d3-59853744a7e2" />
<img width="469" height="95" alt="image" src="https://github.com/user-attachments/assets/9ad55cd8-bd68-4b62-a436-a264f06d7e31" />
<img width="568" height="301" alt="image" src="https://github.com/user-attachments/assets/bc2aa5de-0620-44d2-ac34-c14fe3847bed" />

Fem Ctrl X i intro per guardar i sortir.

<img width="561" height="157" alt="image" src="https://github.com/user-attachments/assets/07ce5e77-2cf1-4ef5-bf0f-92521fccfb71" />





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

