## MONITORITZACIÓ, CONNEXIÓ I LLICENCIAMENT


Per enviar un missatge als logs del que han de fer:

logger[opcions][p-prioritat][missatge]

logger -i -s -p mail.err Aturant el sistema


Servei.prioritat accio:

auth
mail
lpr
cron
kern
cron
…

(prioritat de més petita a més gran)

debug
infor
notice
warning, warn
err, error
crit
alert
emerg, panic



.crit djiwqodj (* equival a tot, el critic, etc)


Sistema de processos:


<img width="597" height="143" alt="image" src="https://github.com/user-attachments/assets/7440324f-f3ad-45ea-90db-d6e342e19ac7" />


<img width="601" height="65" alt="image" src="https://github.com/user-attachments/assets/7615f600-0f7c-49d3-9492-0585af5ef9a1" />


Aquí hi va tots els logs(q no tenen pq estar tots pq depen de q baixem poden estar a carpetes a bada), els aurh són d’autentificació o de auditoria, el kernel simplement kernel, i tots van al syslog.
El .gz és la rotació de logs. Hi han logs q generen més entrades q altres, i per no ocupar tant d’espai se comprimeixen cada x temps i quan ens guarda tb ho decidim natros
**Se fa amb: nano/ etc/logrotate.conf**


<img width="606" height="36" alt="image" src="https://github.com/user-attachments/assets/2f576fae-c0e6-4cb4-8552-00bd5c0716d1" />


Aquí dins hi ha els directoris del logrotate.



<img width="604" height="46" alt="image" src="https://github.com/user-attachments/assets/a24e5bc1-a94d-4e3e-986a-97e7374e5cd5" />
<img width="423" height="37" alt="image" src="https://github.com/user-attachments/assets/7786f98e-ffdd-46cc-9856-4a34692fc4cf" />


[]=identificador process
missatge



<img width="604" height="34" alt="image" src="https://github.com/user-attachments/assets/eb200282-117f-4c41-9afc-40a959290f59" />
<img width="571" height="30" alt="image" src="https://github.com/user-attachments/assets/98790605-7d12-4d60-91da-aaa7b3dd6e78" />
<img width="571" height="37" alt="image" src="https://github.com/user-attachments/assets/b9bbc64d-acd2-4051-b057-89c92b768256" />
<img width="601" height="329" alt="image" src="https://github.com/user-attachments/assets/ed6dee1c-6c99-4e18-96a7-15adc5a42e26" />
<img width="479" height="63" alt="image" src="https://github.com/user-attachments/assets/d98d0213-f0c6-42bc-b144-20af3d259bdb" />
<img width="598" height="27" alt="image" src="https://github.com/user-attachments/assets/cabe5aae-4ed6-4094-8bd8-15776e76b366" />
<img width="611" height="100" alt="image" src="https://github.com/user-attachments/assets/8f693dfe-a6b5-4905-917d-615325dcd2c8" />
<img width="582" height="97" alt="image" src="https://github.com/user-attachments/assets/1b9b2848-3bfe-41ec-aa1a-d1f544f89972" />
<img width="582" height="97" alt="image" src="https://github.com/user-attachments/assets/ace75b5d-4b72-4458-afbf-2927d119e92b" />


(només el del crit)


<img width="603" height="180" alt="image" src="https://github.com/user-attachments/assets/489014ae-9e62-4562-9a25-be6f7940807e" />



Sol hauria de funcionar la 5 (funciona)





<img width="594" height="79" alt="image" src="https://github.com/user-attachments/assets/1026582b-1078-4863-b9db-9cad7c1b18c2" />
<img width="495" height="43" alt="image" src="https://github.com/user-attachments/assets/27658209-2570-4869-afb0-e9233d6fdaf2" />
<img width="603" height="186" alt="image" src="https://github.com/user-attachments/assets/fd221ddf-ea8d-41ea-89f9-339725216dd9" />




### Exercici Logs dos Maquines


<img width="611" height="434" alt="image" src="https://github.com/user-attachments/assets/798ea6c0-4ded-4d6f-932d-1b1782aa0351" />




Fiquem les dos màquines en Xarxa NAT I Xarxa interna.
M’asseguro de que les dos màquines no tinguin la mateixa IP (10.0.2.15 i 10.0.2.4).



<img width="592" height="227" alt="image" src="https://github.com/user-attachments/assets/7bfd5d64-103d-44a1-b7ea-4bd2a8b3421f" />


<img width="604" height="104" alt="image" src="https://github.com/user-attachments/assets/255ca98c-1311-4556-bbbe-9b9b7eb03852" />




Mirem el número que té el port que està escoltant (4096).





<img width="598" height="39" alt="image" src="https://github.com/user-attachments/assets/762b407d-5592-42b6-a62d-5c56d5c19976" />
<img width="597" height="66" alt="image" src="https://github.com/user-attachments/assets/f8449f81-c7c6-456e-889c-e8c5e28cb5ca" />



Executem aquestes comandes (la segona en una altra terminal) en la que ha d’escoltar i anem a l’altra màquina i executem el següent per comprovar si funciona correctament:



<img width="601" height="129" alt="image" src="https://github.com/user-attachments/assets/d88e3f8f-8a3c-4074-ad51-87ced174f9c0" />




Ara anem a la màquina que envia els missatges i escrivim el que volem enviar:




<img width="588" height="32" alt="image" src="https://github.com/user-attachments/assets/58a175d0-d35c-4ef1-a3de-6f5b85d42bdc" />





Si ara tornem a la màquina receptora veurem això a la terminal:



<img width="337" height="51" alt="image" src="https://github.com/user-attachments/assets/a0f4ec7a-7fbc-48d7-94dc-e40f926c0fc2" />




I si anem a fitxers i obrim la carpeta de l'usuari veurem el fitxer .txt. que hem creat. L’obrim i veurem el missatge:




<img width="589" height="200" alt="image" src="https://github.com/user-attachments/assets/827d1167-c7f3-45a3-a9ea-90b1fd1e6073" />




### Exercici connexió dos màquines


SSH:
al client (el que vull accedir):


<img width="599" height="331" alt="image" src="https://github.com/user-attachments/assets/7a9044ca-34f7-4067-91ee-e5c37f848401" />


Instal·lem el x11vnc.


<img width="509" height="41" alt="image" src="https://github.com/user-attachments/assets/021be492-f50d-4e92-ab0b-1f9e232cdb97" />


<img width="468" height="92" alt="image" src="https://github.com/user-attachments/assets/bbbba1af-247e-447e-83b2-977925dc33fd" />


Fiquem la contrasenya del VNC i la confirmem.


<img width="497" height="550" alt="image" src="https://github.com/user-attachments/assets/902e4743-17c1-440b-b8f8-8b337022c543" />


Sel·leccionem els següents botons que es poden veure a la captura.



<img width="544" height="54" alt="image" src="https://github.com/user-attachments/assets/0175ddd3-d1aa-4d29-b851-cc55ac0655f7" />


<img width="593" height="564" alt="image" src="https://github.com/user-attachments/assets/aaf39713-ad22-4130-a8c5-933d0cc13429" />



Comentem el WaylandEnable=false (li treiem el #)

I fem Reboot.




<img width="594" height="246" alt="image" src="https://github.com/user-attachments/assets/f1cb0238-abb4-44d7-a080-3bdadab6e900" />



<img width="588" height="430" alt="image" src="https://github.com/user-attachments/assets/8222c205-e02d-413b-b875-21232ac96ff5" />




Ja ho tenim connectat.



Al amfitrio:



<img width="591" height="315" alt="image" src="https://github.com/user-attachments/assets/75a41e63-2512-4d61-b6ea-3a151bda77ee" />
