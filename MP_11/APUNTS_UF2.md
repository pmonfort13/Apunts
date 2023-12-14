# Mecansimes de Seguretat Activa

## Introducció

- Protecció de la informació --> Conseqüència de l'aplicació de mecanismes o estratègies de seguretat.

- Principis que han de considerar els mecanismes de seguretat:
    - La seguretat com un **Objectiu global**.
    - Seguretat dissenyada com quelcom que és part de l'organització.
    - El marc legal --> considerat com una part més del disseny de les polítiques de seguretat

- **Seguretat activa:** Aquells mecanismes, físics i lògics que pernmetens prevenir i detectar possibles intents de comprometre els components d'un sistema informàtic.

## Sistemes personals
### Atacs i contramesures

- Atacs segons l'objectiu
    - **Interrupció:** Contra la disponibilitat en el qual es destrueix, o queda deshabilitat, un recurs del sistema.
    - **Intercepció:** Contra la confidencialitat en el qual un elemnt no autoritzat aconsegueix l'accés a un recurs.
    - **Modificació:** Contra la integritat en el qual a més d'aconseguir l'accés no autoritzat a un recurs, pot modificar, esborrar o alterar el recurs de qualsevol forma
    - **Fabricació:** Contra la integritat en el qual un elemnt aconsegueix crear o inserir objectes falsificats en el sistema.

- Atacs segons la seva forma
    - **Atacs passius:** No modifica ni destrueix cap recurs del sistema, simplement observa amb la finalitat d'obtenir informació no autoritzada.
    - **Atacs actius:** Altera o destrueix un recurs del sistema. Podria causar problemes molt seriosos:
        - **Suplantació d'identitat**
        - **Re-actuació:** Un o diversos missatges legítims són interceptats i reenviats diverses vegades per produir un efecte no desitjat.
        - **Degradació fraudulenta del servei:** Evita el funcionament normal dels recursos del sistema informàtic.
        - **Modificació de missatges:** Modifica un part del missatge interceptat i es reenvia a la persona a qui anava adreçat.

- Atacs segons el tipus d'atacant
    - **Insiders/Outsiders** Un atac pot provenir tant de l'interior de la xarxa (insiders) com de l'exterior (outsiders)
    - Podem pensar que la majoria d'atacs provenen de l'exterior d'una organització i són escassos, però no és així:
        - **Atacs externs més nombrosos** que els interns.
        - **Percentatge d'èxit major en els interns** que en els externs.
        - **Dany més grans causats pels atacs interns**.
    - **Principals possibles atacants** d'un sistema informàtic:*
        - **Personal de la mateixa organització**
        - **Antics treballadors**
        - **Intrusos informàtics o hackers**
        - **Intrusos renumerats**

## Anatomia dels atacs

- Un atac informàtic sol constar de **cinc fases**:
    **1. Reconeixement**
    **2. Escaneig**
    **3. Accés al sistema**
    **4. Manteniment de l'accés**
    **5. Esborrat d'emprenents**

- Aquest coneixement ajuda a preveure activats que podrien comprometre a un sistema informàtic.

### Reconeixement

- Primera fase: **Recopil·lació de tota la informació possible** del sistema que pretén comprometre.

- Diverses tècniques de recopil·lació
    - **Enginyeria social o trashing**
    - **Recerques a internet**
    - **Sniffing (Capturar el trànsit de xarxa)**
    - **ordre whois**

### Exploració

- L'atacant usarà aquesta informació per sondejar el sistema i **detectar vulnerabilitats** que pugui aprofitar per tal d'accedir al sistema.

- Vulnerabilitats que busca l'atacant: Trobar comptes d'usuari, versions de sistema operatiu i aplicacions, ports oberts...

- Eines d'exploració: tracert (en entorns Windows) o traceroute (en entorns Linux/Unix).

### Accés

- Fase on es fa l'atac de manera efectiva aprofitant les vulnerabilitats

- Es sol iniciar amb el crackeig de contrasenyes el qual es pot usar **Online** (tests en viu com Hydra) o **Offline** (arxius on s'emmagatzemen les contrasenyes encriptades recorrent a tècniques de diccionari, força bruta o criptoanàlisi)

- És una fase complicada, ja que s'ha d'**evadir els Firewalls, realitzar evasió d'IDS, IPS i Honeypots per fer la penetració**. Ús d'eines com 007 Shell, ICMP Shell o AckCmd.

### Manteniment de l'accés

- Fase on s'intenta preservar la possibilitat d'efectuar nous accessos al futur.

- Eines: Programes de codi maliciós (malware), com els **cavalls de Troia i rootkits**

- L'atac també pot servir per:
    - **Instal·lar malware que monitori les accions** que estem fent (keylogger).
    - Capturar tot el trànsit de la xarxa (**Sniffing**).
    - Instal·lar un **FTP de contingut il·lícit**.
    - Utiltzar el sistema com a plataforma per **atacar altres sistemes informàtics**.

- **rootkit:** Eines informàtics emprades amb finalitats malicioses que permeten l'accés il·licit al sistema.¡
    - Usen tècniques per ocultar la seva presència i la d'altres processos
    - Molt perillosos ja que cedeixen el control del sistema a l'atacant
    - Actuen en tres nivells:
        - **Kernel**
        - **Llibreries**
        - **Aplicacions**


### Esborrat d'emprentes

- És vital per a l'atacant borrar les emprentes del que ha fet el sistema

- Independement del sistema operatiu atacat, queden registrades les seves accions en els logs del sistema.

- Per evitar ser culpat fan el següent:
    - **Deshabilitar l'auditoria** del sistema
    - **Esborrar tots els logs** del sistema i aplicacions compromeses
    - **Esborrar l'evidència o pistes de les eines utilitzades**.

# Seguretat en la Xarxa Corportativa

## Introducció

- Seguretat de xarxa --> Eines i polítiques adoptaqdes per l'administrador del sistema per prevenir i controlar l'accés no autoritzat, mal ús, modificació o inhabilitació.

- Monitoratge de trànsit --> aspectes més importants en la seguretat en la xarxa - Classificat en:
    - **Monitoratge passiu:** escolta i anàlisi del trànsit real de la xarxa. Recull informació i analitza.
    - **Monitoratge actiu:** Injectar paquets de prova a la xarxa, o enviar-ne als servidors i aplicacions i a mesura el temps de resposta obtingut.

## Eines de monitoratge passiu

- **Detectors o sniffers:** Permeten la captura i enregistrament de la informació que circula per una xarxa.
    - Manera de detectar sniffers: Cercar la presència de targetes en **mode promiscu.**
    - Diverses eines: ifconfig, ifstatus o Network Promiscous Ethernet Detector (NEPED).

- **Mesures de protecció**
    - **Xifratge de documents** que s'envien per la xarxa amb PGP
    - Eines criptogràfiques: **protegiexen la informació** que circula, pero no estableixen connexions segures.
    - **Secure Shell (SSH):** Permet l'establiment d'inicis de sessió segurs.

## Eines de monitoratge Actiu

- Escàners --> Serveixen per detectar les vulnerabilitats d'un sistema informàtic.
- Escaneig de ports --> Esbrinar els ports TCP/UDP que estan oberts en una màquina remota pertanyent a una xarxa determinada.
- Ports oberts --> Informació molt interessant per als atacants, ja que les vulnerabilitats del processos que estan en funcionament poden permetre l'accés no autoritzat al sistema.
- TCP i UDP --> Protocols que comparteixen tots els ordinadors connectats a Internet per poder connectar-se entre ells.

## Esquema de funcionament d'un escàner

![Esquema_escaner](/img/prova.png)

## Ordres del sistema

- Diagnosi ràpida de possibles errors --> **ping** (determinar si una màquina està connectada) i **traceroute** (Obtenir descripció del camí que es va seguint per arribar a una màquina).

- Eines que faciliten el monitoratge de la xarxa --> MRTG (Multi Router Traffic Grapher) o Nagios

## Seguretat en xarxes sense fil

- **Comunicacions sense fil** --> basades en ones de ràdio o infroges, permeten connectar-se des de qualsevol lloc sense necessitat d'estendre cap cablejat.
- **Wifi** --> wireless fidelity - Xarxes locals sense fils --> WLAN
- Les  xarxes  locals  sense  fil  poden  operar  en  mode  ad  hoc  o  en  mode infraestructura:
    - **Mode ad hoc**
    - **Mode infraestructura**

## Riscos potencials dels serveis de xarxa

### Seguretat de les topologies i el tipus de xarxa

- **Topologia** --> S'enten per la forma o estructura de xarxa des del punt de vista lògic.

### Seguretat del maquinari de xarxa

- Commutadors, concentradors i encaminadors --> Prendre les següents precaucions:
    - **Activació del xifratge**
    - **Desactivar el control remot d'administració**
    - **Canviar les contrasenyes d'administració dels dispositius**
    - **Usar llistes d'accés** (permeten sol els protocols, ports i IP que es necessitin)

## Control d'accés a la xarxa basat en autenticació

- Requereix de tres components:
    - **Client**
    - **Autenticador**
    - **Servidor d'autenticació**

## Atacs als serveis de la xarxa

### Atacs de denegació de servei

- Objectiu --> Inutliitzar el maquinari o programa de manera que els recursos del sistema no siguin accesibles desde la xarxa.
- Basat en el modus operandi del protocol d'establiment de sessió.
![Esquema Atac DDoS](/img/ddos-attack-1-1024x694.png)

## Atacs de falsejament d'identitat o spoofing

- Formes de suplantació d'identitat:
    - **Falsejament de IP**
    - **Falsejament d'ARP** --> Usades per realitzar atacs man-in-the-middle
    - **Falsejament de DNS** --> Usades per realitzar atacs pharming
- Amb aquestes tècniques es poden aconseguir atacs de denegació de servei.

## Sistemes de detecció d'intrusos (IDS)

- Monitoren els continguts del flux d'informació de la xarxa a la recerca i rebuig de possibles atacs.
- Capacitat de combinar hardware i software.
- Tipus de classificacions:
    - Segons la **font de la informació**
        - **Basats en xarxa**
        - **Basats en màquina**
        - **Basats en aplicacions**
    - Segons el **tipus d'anàlisi**
        - Basats en **firmes**
        - Basats en **anomalies**
    - Segons el **tipus de reposta d'IDS**
        - **Resposta passiva**
        - **Resposta activa**

## Les xarxes públiques

### Seguretat en la connexió

- **Xarxa pública** --> Gestionada per una operador de telecomunicacions, per tant la informació que viatja és propensa de ser 'observada'
- Ús: Requereix l'establiment de relacions de confiança en un entorn gairebé anònim i intangible per definició
- **Signatura electrònica** --> permet que un emissor pugui enviar missatges a un receptor complint les tres propietats següents:
    - **Autenticitat**
    - **Integritat**
    - **No repudi**

# IDS (SNORT)

## SNORT IDS

- Funció de **detectar comportaments anòmals** dins de la 
nostra xarxa o intents d'accés no desitjats.


### Què és SNORT?

- Es un IDS capaç d'analitzar el tràfic de la nostra xarxa a temps real i reaccionar a partrons detectats.

## Funcionament dels IDS

- Eines que utilitza:
    - Recollida de dades o sniffing
    - Aplicació de regles per detectar riscos
    - Filtratge on compara patrons de tràfic observat amb patrons d'atacs predifinits
    - Detecció d'esdeveniments no esperats a la xarxa
    - Generació d'alarmes
    - Actuació sobre el tràfic detectat

## SNORT

### Modes de funcionament

- Monitorització (sniffer)(-v capçaleres -d dades)
    - Exemple: **sudo snort -v -i eth0**
- Enregistrament de paquets de la Xarxa
    - Exemple: **sudo snort  -l ./log  -i eth0**
- HIDS (Host IDS) / NIDS (Network IDS)
    - Exemple: **sudo snort -A console -c /etc/snort/snort.conf -i eth0**

## Ubicació dels IDS

- S'ha de situar en un lloc on pugui capturar tot el tràfic a monitorar
- La ubicació dependrà del seu us com a IDS/IPS
    - s'ha de situar inline al mig de la comunicació
- De vegades es posa un IDS abans del firewall i un altre després o un IPS

## SNORT Inline (IPS)

- Permet blocar el tràfic entre 2 interfície
- Paràmetre -Q indica que ha de funcionar inline

### Modes de funcionament:
- Alertes per consola
- Enregistrar alertes

## Fitxers de configuració

- L'arxiu de configuració es troba /etc/snort/snort.conf

## Regles a Snort

- Les regles base es troben a /etc/snort/rules
- Des de l'arxiu de configuració poden activar i desactivar regles.
ACABAR DE MIRAR

## Variables SNORT

- Snort diposa d’una sèrie de variables globals amb les que podem 
configurar de forma senzilla l’estructura de la nostra xarxa
    - **HOME_NET**
    - **EXTERNAL_NET**
    - **SERVERS**
    - **PORTS**
    - **Llista Blanca**
    - **Llista negra**

## Regles SNORT

- Les regles es divideixen en dues parts, La, capçalera i els camps espécifics
- Parts de la capçalera:
![Capçalera](/img/Capçalera.png)

- Acció: Indica que succeix a la regla
    - Alert
    - Log
    - Pass
    - Drop
    - Reject
    - sdrop

- Protocol
- Origen i destí
- Ports
- Direcció

- Camps específics: ns permeten ajustar més concretament que busquem, es troben entre parèntesi i separats per ‘’;’’
    - msg:
    - sid:
    - rev:
    - classtype:
    - priority
    - flow:

## Creant les nostres Regles SNORT

- **Objectiu:** Es necessari saber quin es l’objectiu de la regla:
    - Detectar un tipus de tràfic.
    - Bloquejar tràfic a llocs no permesos.
    - Crear perfiles de navegació
    - Buscar connexions de noves amenaces.
    - Detectar fugues d’informació.
- **Acció:** que volem que passi.
    - Informar al nostre SOC (Centre d’Operacions de Seguretat).
    - Escriure en un log amb informació.
    - Actuar sobre el Firewall.
- **Abast:** Area d’actuaciñio de la regla.
    - Interna.
    - Externa.
    - Comunicació de fora a dins.
   -  En Ambdós sentits.
Tota la xarxa o alguns equips.
- **Optimització:** Quina es la millor forma de buscar.
    - Valor Hexadecimals.
    - Cadenes de text.
    - Text en la URL.

## Revisió d’alertes

- Els arxius de log de les alertes, així com la resta de logs generats per Snort, es troben per defecte a /var/log/snort

## Exemples regles SNORT

- `alert tcp $HOME_NET 21 → any any (msg:"Error autenticació FTP"; content:"Login or password incorrect"; sid:1000003;  rev:1;)`
- `Alert tcp $EXTERNAL_NET any → $HOME_NET 3306 (msg:"MYSQL  show  databases  attempt";  flow:  to_server,  established; content:"|0F 00 00 00 03 | show databases"; sid:1000004; rev:1;)`


# Xarxes Privades Virtuals

## Introducció

- **Exemple:**

![Interconnexió de xarxes](/MP_11/img/Captura%20de%20pantalla%202023-12-14%20110020.png)

- S'establerix una VPN entre dos gateways, cadascun d'una xarxa privada
- Les màquines de les xarxes utilitzen aquests gateways com routers
- Quan una gateway rep un paquet dirigit a la xarxa privada l'altre extrem el paquet s'envia a través de la VPN de manera segura
- El trànsit sol es protegit per la VPN entre els dos gateways.

## Treballadors remots

- Exemple:

![Treballadors remots](/MP_11/img/Captura%20de%20pantalla%202023-12-14%20110710.png)

- Qualsevol persona amb permís pot connectar-s'hi des de qualsevol lloc.
- L'ordinador ha de comptar amb un client VPN, que estableix una connexió al concentrador de VPNs de la xarxa corporativa
- Tot el trànsit des de l'ordinador fins la xarxa corporativa queda protegit per la VPN.

## Avantatges i inconvenients VPN

- **Avantatges**
    - **Seguretat**: És possible assegurar diversos serveis amb aquest mecanisme
    - **Mobilitat**: Connexió segura entre usuaris mòbils i la xarxa fixa, independentment de la localització geogràfica
    - **Transperència**: Interconnexió d'ordinadors en un sistema informàtic i de difrerents xarxes. Transparent per l'usuari, Configuració només a l'entorn servidor
    - **Simplicitat**: Una VPN aconsegueix que l'equip sigui vist per tota la xarxa, la qual cosa simplifica l'administració d'equips remots.
    - **Estalvi econòmic**: Trànsit segur de paquets per xarxes púibliques --> cost econòmic menor que la creació de xarxa dedicada.

- **Inconvenients**: 
    - **Fiablitat**: Depèndencia del proveïdor de xarxa (ISP) --> Fallades en la xarxa que poden incomunicar recursos de la nostra VPN.
    - **Confiança**: Si la seguretat d'un node o subxarxa que forma part d'una VPN queda compromesa es veurà afectada la seguretat de tots els components de la xarxa.

## Tunneling

- Mètode que consisteix a utilitzar la infrestructura de xarxes per transportar dades d'una zrxa a una altra.
- Les dades que han de ser transportades poden ser paquets de protocol diferent al que gestioni internet
- Els paquets encapsulats són llavors encaminats sobre Internet entre els extrems del túnel. Aquesta ruta l'ogica se l'anomena 'túnel'.

![Paquets tunneling](/MP_11/img/Captura%20de%20pantalla%202023-12-14%20113345.png)

## Protocols de Tunneling

- **IP Security (IPSec)**: : garanteix la seguretat de la transmissió i autenticació d’ususaris sobre xarxes públiques
- **Protocol de Tunneling Punt a Punt (PPTP)**: alternativa a IPSec. Treballa en la capa d’enllaç i s’utilitza per a transmissions segures de tràfic basat en Windows.
- **Layer 2 Tunneling Protocol**: combinació de reenviament de
capa 2 i PPTP, i es utilitzat per a encapsular trames de tipus PPP (Protocol Punt a Punt).
- **OpenVPN**: protocol de codi obert. Totes les dades son
xifrades amb una clau AES-256 i autenticació RSA.

## Secure Shell

- Protocol que permet establir una connexió segura, de manera que un client pot obrir una sessió interactiva en una màquina remota per enviar ordres o fitxers a través d’un canal segur.
- Les dades que circulen estan **xifrades**
- **El client i el servidor s'autentifiquen mútuament.**
- **Fases** d'una connexió0 SSH:
    - Es determina la **identitat del servidor i del client** (capa segura de transport). El client inicia sessió en el servidor
    - Establiment d’un **canal segur**. Fase de negociació entre el client i el servidor per posar-se d’acord en els mètodes de xifratge que volen utilitzar. 
    - **Autenticació**. Un cop s’ha establert la connexió segura entre el client i el servidor, el client s’ha de connectar al servidor per obtenir un dret d’accés. Hi ha diversos mètodes: 
        - El mètode més conegut és la **contrasenya** tradicional.
        - Ús de **claus públiques**. 
