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

Aquí elegim minimal installation i download updates mentre instal·lem Ubuntu.
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


## Llicenciament

<img width="817" height="459" alt="image" src="https://github.com/user-attachments/assets/5fa5c9b1-1130-4e93-8837-62a1e112e7b1" />

A continuació explicaré el que hem pogut observar en la imatge anterior sobre les llicències típiques d'Ubuntu i quines són:
- GPL = és la més usada a Linux, ja que obliga a compartir el codi en cas de distribució.
- LGPL = és més flexible que l'anterior però més sensible per a les biblioteques.
- Apache, BSD, Artistic, MPL = són més permissives i deixen barrejar amb programari privatiu.
- GFDL = per la documentació
- CC0 = és domini públic (sense restriccions)

En resum, ninguna és la principal, no obstant la més usada de les ja mostrades seria la GPL.


## Instal·lacions duals i Gestors d'arrencada

· Instal·lació Windows



Seleccionem la nostra maquina i anem a paràmetres --> emmagatzematge --> <img width="259" height="57" alt="image" src="https://github.com/user-attachments/assets/97540f08-2fbe-4a51-ac58-9a90879c227e" /> --> polsem el disquet blau i sel·leccionem el windows, es veurà així: <img width="259" height="57" alt="image" src="https://github.com/user-attachments/assets/ffc7c11d-c737-4f05-a826-f275572774e7" /> 

Obrim la màquina, entrem al windows i fem el següent:

<img width="535" height="395" alt="image" src="https://github.com/user-attachments/assets/2022ae3e-0ec2-4565-a3a2-cf5906b43f07" />
<img width="512" height="384" alt="image" src="https://github.com/user-attachments/assets/2b25f25a-eb33-47bc-ae52-405c9855ec4f" />
<img width="503" height="378" alt="image" src="https://github.com/user-attachments/assets/b14d6951-1323-42f1-a4dc-82dde1c7e63c" />

Personalitzem.

<img width="503" height="378" alt="image" src="https://github.com/user-attachments/assets/e40da65a-f297-4508-864b-2d479eec8af0" />
<img width="551" height="447" alt="image" src="https://github.com/user-attachments/assets/03f43327-52a8-4876-904f-e51189d636ff" />

Continuem, seleccionem l’idioma i teclat espanyol, omitim afegir algun teclat extra i en ves de començar amb una conta de windows polsem entrar en un domini.

<img width="473" height="349" alt="image" src="https://github.com/user-attachments/assets/7505ef1d-3879-4b80-bb2c-217e6123382c" />
<img width="655" height="549" alt="image" src="https://github.com/user-attachments/assets/6c26c064-bd04-4681-82c1-18c73cdebb8e" />

Apaguem.






· El grub

Entrem a la màquina al Ubuntu i obrim terminal i fem el següent:

Primer que res fem sudo su i després nano /etc/default/grub

<img width="597" height="382" alt="image" src="https://github.com/user-attachments/assets/c1f1ead8-f565-4c20-9c3a-cc5a6f7185ac" />

Fem Ctrl x i intro per guardar i sortir.

<img width="582" height="165" alt="image" src="https://github.com/user-attachments/assets/f3873c22-6b3b-4362-b192-130ed9ea990b" />
<img width="598" height="386" alt="image" src="https://github.com/user-attachments/assets/d4e10e2d-7659-4515-bc17-c2cf66eaac6b" />
<img width="594" height="361" alt="image" src="https://github.com/user-attachments/assets/064e37c0-fba0-461f-9a4d-559f8e48d35b" />

Recordem el número que ens surt al sda del EFI per poder usar-lo a la següent comanda.

<img width="594" height="361" alt="image" src="https://github.com/user-attachments/assets/1c26ad00-ac6f-469a-b1f2-c956696398cf" />
<img width="594" height="361" alt="image" src="https://github.com/user-attachments/assets/40394b15-d4ec-4d6d-8f78-aca7a7c7c3e6" />
<img width="594" height="361" alt="image" src="https://github.com/user-attachments/assets/97278e37-65ab-425a-810a-23e33fbda887" />
<img width="594" height="361" alt="image" src="https://github.com/user-attachments/assets/dd628150-76c5-4978-9c94-f4e1f55deeff" />
<img width="598" height="386" alt="image" src="https://github.com/user-attachments/assets/9b2711d6-e99a-4ce4-920a-355c14f15739" />
<img width="598" height="386" alt="image" src="https://github.com/user-attachments/assets/c47fd467-1682-4559-bb88-964a4cb6610c" />
<img width="598" height="386" alt="image" src="https://github.com/user-attachments/assets/887724ef-62aa-4d68-ba10-ef74b0bb5c25" />

Tanquem la màquina i la tornem a obrir i hauriem de veure això:

<img width="607" height="441" alt="image" src="https://github.com/user-attachments/assets/a3ecbac8-5579-4cec-86d1-5e54774f57c0" />

A partir d'ara podre triar si volem usar el Windows o l'Ubuntu quan obrim la nostra màquina.


## Particions i punts de restauració
Anem a aprendre a fer instantànies de la màquina, les quals són com una imatge de com estava la màquina en un cert punt per si en algun moment necessitem tornar enrere.
El primer que farem serà anar a paràmetres i d'allí entrem a emmagatzematge i al apartat del Ubuntu en creem un altre Ubuntu. Ens quedarà així:

<img width="620" height="405" alt="image" src="https://github.com/user-attachments/assets/7dabda84-0a87-44fc-b8d9-adef2e4d20a8" />

Creem una partició:

<img width="620" height="405" alt="image" src="https://github.com/user-attachments/assets/6867dc0f-01c1-44ce-bea2-de50d7a54600" />

<img width="620" height="405" alt="image" src="https://github.com/user-attachments/assets/3326bb83-c0d5-42fc-88ce-ebf86c092310" />

<img width="620" height="405" alt="image" src="https://github.com/user-attachments/assets/f969fc50-2e4e-4c3c-9e19-33e8bcc4f2e3" />

<img width="620" height="405" alt="image" src="https://github.com/user-attachments/assets/5aea8707-161f-45e6-822a-26312502b70a" />

Entrem al timeshift:

<img width="620" height="405" alt="image" src="https://github.com/user-attachments/assets/44331f93-76b8-4a9e-8daf-3ba86b0ac11c" />

<img width="657" height="270" alt="image" src="https://github.com/user-attachments/assets/3275e1db-04c0-4a8d-b831-d92db0b4c494" />

<img width="658" height="713" alt="image" src="https://github.com/user-attachments/assets/c1e189d1-3a44-44e0-b13e-9d24a547d0cf" />

<img width="658" height="713" alt="image" src="https://github.com/user-attachments/assets/587e2f49-2215-4004-aeb4-82ef7db47961" />

Fem una còpia de l'usuari Cinta:

<img width="658" height="713" alt="image" src="https://github.com/user-attachments/assets/fe446f52-7c5c-4f23-9ac5-843dc153b7be" />

<img width="642" height="600" alt="image" src="https://github.com/user-attachments/assets/a0d44384-390a-4a61-9826-096bcc137270" />

Obrim terminal:

<img width="648" height="503" alt="image" src="https://github.com/user-attachments/assets/f5141023-e858-41a0-ab7d-1ac1689222e3" />

Restarurem:

<img width="666" height="547" alt="image" src="https://github.com/user-attachments/assets/cbf375c1-66ae-45b2-a16b-c1726f5027aa" />

Si ho hem fet tot bé veurem, això:

<img width="662" height="272" alt="image" src="https://github.com/user-attachments/assets/6504ec89-9152-44a4-818a-3268fd84e80d" />

<img width="662" height="272" alt="image" src="https://github.com/user-attachments/assets/2379fbfc-02ae-4500-ac33-4274e9bb0b58" />

<img width="662" height="272" alt="image" src="https://github.com/user-attachments/assets/dff55f1a-cdf0-4170-8d23-144e83c31fb7" />



## Cofiguració bàsica de la xarxa
1) Entrem al Ubuntu
2) Entem a configuració

3) <img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/30315e2a-380b-46db-89a2-504eb5d0d053" />

4) Obrim terminal
   
5) <img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/6eec5a45-d90c-4267-b79e-2284add10687" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/a96da78f-262e-4f40-aee9-1a47e5a7b4a1" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/51c31f5f-74f4-4366-ae1a-5b62c3cbea4d" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/3099fcc0-0e86-413c-b925-a5cebc9df526" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/d91da2a6-314f-481e-bbbe-d0b6d7b3f207" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/d0ddfcb8-51ff-4ecb-b756-dba056469806" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/e26ccefb-1fdb-4cb0-98de-8a6e9f60631d" />
<img width="663" height="389" alt="image" src="https://github.com/user-attachments/assets/1a9e6e30-f522-423a-98e5-7638c5e97ae7" />


## Comandes generals i instal·lació d'aplicacions

