# PREGUNTES I POSSIBLES PREGUNTES RECU TEÒRIC

1. **Si el servei DNS arrenca correctament i les comandes per comprovar la sintaxis dels fitxers no donen cap error, en quin dels següents fitxers podem tenir l’error?**
   - a) En qualsevol que haguéssim modificat.  **--> CORRECTE**
   - b) Als fitxers de zona inversa i directa i al named.conf.local.
   - c) Només als fitxers de zona inversa i directa.
   - d) Al fitxer named.conf.options i al named.conf.local.

2. **Quina de les següents afirmacions sobre el bind és la més certa? En el cas que quan acabem la instal·lació i reiniciem la màquina no ens funciona internet.**
   - a) El bind no s’ha posat en funcionament.
   - b) El bind no s’ha posat en funcionament perquè no hem creat el dimoni que fa que s’iniciï el servei en el nivell d’execució que volem.
   - c) El bind no s’ha posat en funcionament perquè no s’ha modificat el fitxer resolv.conf. **--> CORRECTE**
   - d) El bind no s’ha posat en funcionament perquè tenim qualsevol tipus d’error en la sintaxis dels fitxers de configuració.

3. **Quina de les següents no és funció principal alhora de tenir configurat un servidor DNS esclau?**
   - a) Fer el sistema més segur davant possibles caigudes d’algun dels servidors.
   - b) Poder gestionar el servidor DNS per diversos administradors a la vegada.  **--> CORRECTE**
   - c) Dividir la càrrega del sistema en quant a peticions sobre el servidor DNS.
   - d) Totes són falses.

4. **Quina és la funció del paràmetre forward only del fitxer named.conf.options?**
   - a) Fa que les consultes DNS externes només s’enviïn als forwarders.  **--> CORRECTE**
   - b) Permet fer consultes DNS a totes les màquines de la xarxa que indiquis.
   - c) Denega les consultes DNS a totes les màquines de la xarxa que indiques en una ACL.
   - d) Totes són falses.

5. **Quina de les següents afirmacions respecte la base de dades DNS és certa?**
   - a) Cada nom de domini és una rama d’un arbre invertit.  **--> CORRECTE**
   - b) Tots els nodes de l’arbre sempre han de tenir un nom que l’identifiquin.
   - c) Té forma d’arbre el qual comença al node arrel al nivell inferior.
   - d) Totes són certes.


6. **Quina de les següents definicions respecte els registres de recursos és certa?**
   - a) Els registres DNS permeten al servidor respondre a totes les peticions que li fan els clients.
   - b) Els registres A i CNAME són imprescindibles per a que funcioni el servei DNS.
   - c) Emmagatzemen informació relativa als noms de domini DNS.   **--> CORRECTE**
   - d) a i c són correctes.

7. **Quin dels següents fitxers crida primer el procés associat al servei DNS?**
   - a) named.conf.options
   - b) named.conf  **--> CORRECTE**
   - c) named.conf.local
   - d) db.named.hosts

8. **Quina és la funció del registre PTR?**
   - a) Estableix una correspondència entre un nom i una @IP del domini, amb la qual pots obtenir la seva IP.
   - b) Estableix l’equip servidor de noms autoritzat per a la zona del domini.
   - c) Estableix una correspondència entre un nom i una @IP del domini, amb la qual pots obtenir el seu nom.  **--> CORRECTE**
   - d) Totes són falses.

9. **Quina de les següents afirmacions respecte el paràmetre also-notify és correcta?**
   - a) Quan el configurem al mestre mantenim els DNS primari i secundari sincronitzats.
   - b) Permet enviar notificacions entre el servidor primari i secundari.
   - c) Quan el configurem a l’esclau permetem els canvis de zones de mestre a esclau.
   - d) a i c són correctes.  **--> CORRECTE**

10. **Quina de les següents afirmacions sobre el número de sèrie definit al registre SOA és falsa?**
   - a) En cas que el nº del servidor secundari sigui major que el del servidor primari, significa que el primari ha canviat la informació de la zona. **--> CORRECTE**
   - b) S’utilitza com a referència d’actualització per als servidors secundaris.
   - c) Aquest número l’ha de modificar manualment l’administrador cada cop que hi ha un canvi.
   - d) Totes són falses.

11. **Quin arxiu no s’ha d’editar per a unir bind i dhcp?**
     - a) named.conf.local i named.conf.options **--> CORRECTE**
     - b) named.conf i named.conf.local
     - c) named.con i dhcpd.conf
     - d) a i c son falses  

12. **Quin port actúa al dhcp per al servidor i client?**
      - 67 Servidor i 68 Client


13. **Quins arxius s’han de configurar al client?**
   - resolv.conf i nsswitch.conf **--> CORRECTE**
   - resolv.conf i interfaces 
   - nsswitch i algo
   - hosts i interfaces 

14. **Per a que serveix la clausula authoritative de la configuracio del DHCP?**
   - La clàusula authoritative indica que el servidor està autoritzat, això significa que l’assignació que ofereix als clients és correcta (DHCPACK), és a dir, que la utilitat que té és identificar el servidor DHCP com aquell autoritzat dins la xarxa enfront d’altres servidors DHCP instal·lats. 

15. **Quina funció fa lo DHCPREQUEST?**
   - Renovació: Un client DHCP utilitzarà el missatge DHCPREQUEST per renovar l'arrendament d'una adreça IP ja assignada. 
   
   - Canvi d'adreça IP: Si un client DHCP vol canviar l'adreça IP assignada, pot enviar un missatge DHCPREQUEST per sol·licitar una nova adreça IP al servidor DHCP.
   
   - Confirmació: Un client que ha rebut diverses ofertes d'adreces IP dels servidors DHCP pot enviar un missatge DHCPREQUEST per confirmar l'adreça IP que ha seleccionat.

16. Quins arxius de configuració fan que encara que estiguin mal el servei pugui esta actiu?


17. **Paràmetre option host-name**
   - Configura el nom del host.

18. **Que es el teams d'Actualització (Refresh Time)?**
   - Indica cada quan temps (en segons) un servidor secundari
ha de contactar amb el primari per a comprovar els canvis de la zona.

19. **Quina és la funció del registre A?**
   - Estableix una correspondència entre una @IP i un nom de domini. Cada registre A identifica un nom de màquina, i el client DNS pot obtenir a través d’ell la seva direcció IP.

20. **Quina és la funció del registre NS?**
   - Estableix l’equip servidor de noms (DNS) autoritzat per a la zona del domini
informaticaASIX2.com.

21. **Què és el registre SOA?**
   - És un registre de recursos d'inici d'autoritat.
   
22. **Quina és la funció del registre CNAME?**
   - Defineix un 'àlies' com a segon nom reconegut d’una IP ja definida
anteriorment

23. **Perquè l'ús de la notació in.addr.arpa?**
  - La resolució dels noms de domini es fa mitjançant consultes que van de dreta
a esquerra
  - Els primers octets d’una @IP identifiquen la xarxa a la qual pertany i la diferència d’altres xarxes.

24. **Quin és el procès que utilitza DNS?**
  - SOL el procès named
  
25. **Perquè es imprescindible un servei de noms?**
    - . Podem accedir als serveis dels equips adreçant-nos a ells amb un nom 'clar' i fent  les configuracions dels serveis amb aquests noms s'aconsegueix flexibilitat.

26. **Quins dos tipus de configuració del servei de DNS hi ha?**
    - Per a Internet (públic) i dins d'una xarxa local (privat)

27. **Com podem comprovar que el servei DNS es troba en execució?**
    - nmap -sU localhost -p 53

28. **Amb quina comanda s'activa el servidor DHCP?**
    - /etc/init.d/isc-dhcp-server start

29. **Amb quines comandes fem les comprovacions de sintaxi?
    - named-checkconf i named-checkzone

30. **Que s'ha de fer cada cop es fa un canvi als arxius .hosts i .rev del bind al mestre?**
    - Cal actualitzar el paràmetre serial (incrementar-lo en una unitat)
