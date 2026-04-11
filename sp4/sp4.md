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




