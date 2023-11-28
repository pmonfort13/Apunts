# PREGUNTES 

- **Si el servei DNS arrenca correctament i les comandes per comprovar la sintaxis dels fitxers no donen cap error, en quin dels següents fitxers podem tenir l’error?**
a) __En qualsevol que haguéssim modificat.__
b) Als fitxers de zona inversa i directa i al named.conf.local.
c) Només als fitxers de zona inversa i directa.
d) Al fitxer named.conf.options i al named.conf.local.

- **Quina de les següents afirmacions sobre el bind és la més certa? En el cas que quan acabem la instal·lació i reiniciem la màquina no ens funciona internet.**
a) El bind no s’ha posat en funcionament.
b) El bind no s’ha posat en funcionament perquè no hem creat el dimoni que fa que s’iniciï el servei en el nivell d’execució que volem.
c) __El bind no s’ha posat en funcionament perquè no s’ha modificat el fitxer resolv.conf.__
d) El bind no s’ha posat en funcionament perquè tenim qualsevol tipus d’error en la sintaxis dels fitxers de configuració.

- **Quina de les següents no és funció principal alhora de tenir configurat un servidor DNS esclau?**
a) Fer el sistema més segur davant possibles caigudes d’algun dels servidors.
b) Poder gestionar el servidor DNS per diversos administradors a la vegada.
c) Dividir la càrrega del sistema en quant a peticions sobre el servidor DNS.
d) Totes són falses.

- **Quina és la funció del paràmetre forward only del fitxer named.conf.options?**
a) Fa que les consultes DNS externes només s’enviïn als forwarders.
b) Permet fer consultes DNS a totes les màquines de la xarxa que indiquis.
c) Denega les consultes DNS a totes les màquines de la xarxa que indiques en una ACL.
d) Totes són falses.

- **Quina de les següents afirmacions respecte la base de dades DNS és certa?**
a) Cada nom de domini és una rama d’un arbre invertit.
b) Tots els nodes de l’arbre sempre han de tenir un nom que l’identifiquin.
c) Té forma d’arbre el qual comença al node arrel al nivell inferior.
d) Totes són certes.


- **Quina de les següents definicions respecte els registres de recursos és certa?**
a) Els registres DNS permeten al servidor respondre a totes les peticions que li fan els clients.
b) Els registres A i CNAME són imprescindibles per a que funcioni el servei DNS.
c) Emmagatzemen informació relativa als noms de domini DNS.
d) a i c són correctes.

- **Quin dels següents fitxers crida primer el procés associat al servei DNS?**
a) named.conf.options
b) named.conf
c) named.conf.local
d) db.named.hosts

- **Quina és la funció del registre PTR?**
a) Estableix una correspondència entre un nom i una @IP del domini, amb la qual pots obtenir la seva IP.
b) Estableix l’equip servidor de noms autoritzat per a la zona del domini.
c) Estableix una correspondència entre un nom i una @IP del domini, amb la qual pots obtenir el seu nom.
d) Totes són falses.

- **Quina de les següents afirmacions respecte el paràmetre also-notify és correcta?**
a) Quan el configurem al mestre mantenim els DNS primari i secundari sincronitzats.
b) Permet enviar notificacions entre el servidor primari i secundari.
c) Quan el configurem a l’esclau permetem els canvis de zones de mestre a esclau.
d) a i c són correctes.

- **Quina de les següents afirmacions sobre el número de sèrie definit al registre SOA és falsa?**
a) En cas que el nº del servidor secundari sigui major que el del servidor primari, significa que el primari ha canviat la informació de la zona.
b) S’utilitza com a referència d’actualització per als servidors secundaris.
c) Aquest número l’ha de modificar manualment l’administrador cada cop que hi ha un canvi.
d) Totes són falses.

- **Quin arxiu no s’ha d’editar per a unir bind i dhcp?**
a) named.conf.local i named.conf.options
b) named.conf i named.conf.local
c) named.con i dhcpd.conf
d) a i c son falses

- **Quin port actúa al dhcp per al servidor i client?**
67 Servidor i 68 Client


- **Quins arxius s’han de configurar al client?**
resolv.conf i nsswitch.conf
resolv.conf i interfaces 
nsswitch i algo
hosts i interfaces 

- **Per a que serveix la clausula authoritative de la configuracio del DHCP?**
la clàusula authotitative indica que el servidor està autoritzat, això significa que l’assignació que ofereix als clients és correcta (DHCPACK), és a dir, que la utilitat que té és identificar el servidor DHCP com aquell autoritzat dins la xarxa enfront d’altres servidors DHCP instal·lats. 

- **Quina funció fa lo DHCPREQUEST?**
Renovació: Un client DHCP utilitzarà el missatge DHCPREQUEST per renovar l'arrendament d'una adreça IP ja assignada. 

Canvi d'adreça IP: Si un client DHCP vol canviar l'adreça IP assignada, pot enviar un missatge DHCPREQUEST per sol·licitar una nova adreça IP al servidor DHCP.

Confirmació: Un client que ha rebut diverses ofertes d'adreces IP dels servidors DHCP pot enviar un missatge DHCPREQUEST per confirmar l'adreça IP que ha seleccionat.

Quins arxius de configuració fan que encara que estiguin mal el servei pugui esta actiu

Paràmetre option host-name

Que es el teams d'Actualització (Refresh Time)



