# REPÀS FINAL EXAMEN TEÒRIC UF1

1. Quins fitxers es necessita configurar en un client?
  -  resolv.conf i nsswithch.conf
  
2. Quina és la funció del paràmetre **forward only** a l'arxiu named.conf.options?
  - Fa que les consultes DNS externes només s’enviïn als forwarders

3. Quina de les següents no és funció principal alhora de tenir configurat un servidor DNS esclau?
  - Poder gestionar el servidor DNS per diversos administradors a la vegada

4. Quina de les següents afirmacions sobre el bind és la més certa? En el cas que quan acabem la instal·lació i reiniciem la màquina no ens funciona internet
  - El bind no s’ha posat en funcionament perquè no s’ha modificat el fitxer resolv.conf

5. Si el servei DNS arrenca correctament i les comandes per comprovar la sintaxis dels fitxers no donen cap error, en quin dels següents fitxers podem tenir l’error?
  - En qualsevol que haguéssim modificat

6. Quina de les següents afirmacions respecte la base de dades DNS és certa?
  - Cada nom de domini és una rama d’un arbre invertit
 
7. Quina de les següents definicions respecte els registres de recursos és certa?
  -  Emmagatzemen informació relativa als noms de domini DNS

8. Quin dels següents fitxers crida primer el procés associat al servei DNS?
  - named.conf

9. Quina és la funció del registre PTR?
  -  Estableix una correspondència entre un nom i una @IP del domini, amb la qual pots obtenir el seu nom.

10. Quina de les següents afirmacions respecte el paràmetre also-notify és correcta?
  - Quan el configurem al mestre mantenim els DNS primari i secundari sincronitzats i Quan el configurem a l’esclau permetem els canvis de zones de mestre a esclau

11. Quina de les següents afirmacions sobre el número de sèrie definit al registre SOA és falsa?
  -  En cas que el nº del servidor secundari sigui major que el del servidor primari, significa que el primari ha canviat la informació de la zona

12. Quin arxiu no s’ha d’editar per a unir bind i dhcp?
  - named.conf i named.conf.local

13. Quin port actúa al dhcp per al servidor i client?
  - 67 Servidor i 68 Client

14. Quina funció fa lo DHCPREQUEST?
  -  Renovació: Un client DHCP utilitzarà el missatge DHCPREQUEST per renovar l'arrendament d'una adreça IP ja assignada

15. Parametre per al host nombrar el nom del host
  - Option host-name

16.  Què es el teams d'Actualització (Refresh Time)?
  - 

- Quins arxius de configuració fan que encara que estiguin mal el servei pugui esta actiu
  - 
