<h1 align="center">APUNTS MP17 UF2</h1>

## Introducció

- • El correu electrònic sofreix constants ciberatacs i intents de frau per part dels ciberdelinqüents
- Usuari --> part més important de la seguretat. Ciberatacs enfocats a intentar enganyar a l'usuari.
- Principals atacs:
    - Phishing
    - Spoofing

# Servei DNS (Domain Name System)

# El correu Electrònic

## Inseguretat del servei DNS. Riscos

## UDP/TCP

## Atacs als protocols UDP/TCP i funcionament

## Capes servei DNS. Assegurament

## Assegurament del servei DNS. Contramesures als atacs.

## DNSSEC. En què consisteix, i funcionament.

## Xifratge DNS. DNS over TLS i DNS over HTTPS. Ports usats. 853/443 (53 UDP)


- **Com funciona un correu electrònic**
POSAR FOTO

1. L'usuari envia un correu, on consta l'emissor i receptor del correu, a un servidor SMTP per tal que aquest realitzi l'enviament.
2. El servidor SMTP realitza una consulta DNS al registre del domini per tal de saber on es troba el servidor de domini de la direcció de destí
3. El servidor DNS retorna la consulta, i com ja sap on s'ha d'enviar, entrega el correu al servidor de destí.
4. El servidor de destí deixa el correu en la bústia d'entrada per mitjà de
POP/IMAP.

## Vulnerabilitats
- Sniffing
- E-mail spoofing
    - Suplantació d'identitat.
    - Enviament de correus electrònics amb remitent fals per enviar spam, difondre malware o portar a cap atacs de phishing
    - Compres per internet (Molts cops la nostra targeta de crèdit està vinculada a un compte)
    - Col·lapsar xarxes d'empreses amb les corresponentes perdues econòmiques

- Phishing
    - Suplantació d'identitat
    - Aconseguir dades i credencials

## Mesures

- Protocols i estàndards de seguretat
    - Protocol SPF
    - Protocol DKIM
    - Estandard d'autenticació DMARC

### Protocol SPF (Sender Policy Framework)

- Protocol d'autenticació de correus
- Permet al propietari d'un domini especificar els servidors de correu que usarà per l'enviament d'un e-mail des del domini.
- Serveix també per a que el receptor confirmi que el servidor que envia els correus és legítim.
- Funcionament
    1. El propietari del domini defineix un registre SPF (en un fitxer .txt) que estarà en el servidor de noms del domini o DNS.
    2.  En el registre SPF s'inclouen les direccions IP legítimes dels servidors que poden usar-se per enviar correus electrònics.
    3. Quan un dels contactes rebi un correu electrònic des d'una direcció del nostre domini, usant el protocol SPF, mirarà que la IP del servidor de correu des d'on s'ha rebut, estigui en el registre SPF. L'enviament serà legítim.
    4. Si la validació SPF és positiva, s'afegirà a la capçalera del correu un resultat positiu de la verificació. Si no s'enviarà com a spam.

- Limitacions
    - Creació i manteniment del registre SPF.
POSAR FOTO diapositiva 11

### Protocol DKIM (Domain Keys Identified Mail)

- Protocol que permet associar un nom de domini a un missatge mitjançant tècniques criptogràfiques.
- S'inclou una signatura o empremta digital en la seva capçalera, marca única e intransferible difícil de falsificar.
- Quan el destinatari rep el missatge verifica la signatura inclosa en la capçalera validant el missatge i la seva procedència.
- Funcionament
    1. El remitent selecciona quines parts del missatge s'inclouran en el procés de signatura, per tal de verificar que no canvien.
    2. En el procés de xifrat es fa un resum digital (hash) de les parts a xifrar mitjançant un algoritme
    3. El resum es signa amb una clau privada pròpia per al domini i s'adjunta la signatura (hash xifrat) al missatge i s'envia.
    4. Quan el receptor rep el missatge amb una signatura DKIM, usa la clau pública del domini de l'emissor per comprovar la procedència del missatge, verificant que pot desxifrar la signatura.
    5. S'obté el resum fet per l'emissor i es compara amb el resum que calcula amb el mateix algoritme el receptor. També es verifica que els elements signats del missatge no s'hagin alterat.

- Quan s'usa el protocol es rep menys spam, no missatges falsos ni suplantació d'identitat
- Per cada possible domini que te un usuari --> Parell de claus (pública/privada). La pública compartir amb el servidor DNS.
- Problema: Difícil d'implementar, alguns proveïdors a lo millor no l'implementen.

FOTO DE DIAPOSITIVA 14

### Estandadrd d'autenticació DMARC

- 

## Mesures a prendre per part dels usuaris

## Capçaleres dels correus electrònics.

### Com interpretar les capçaleres i què contenen

## Com saber si ens han hackejat el correu

## Seguretat en el correu electrònic
**IMPORTANT: SEGURAMENT SORTIRA A L'EXAMEN**

# Servei FTP

## Vulnerabilitat del servei i en què consisteix

## Algoritmes

## Whitelist vs Blacklist

## Alternatives: FTPS SFTP

## FTP Actiu. Funcionament. Canals i ports usats

## FTP Passiu. Funcionament. Canals i ports usats.

## Mesures a prendre per assegurar el servei FTP.



# Servei Web

## Vulnerabilitat del servei i en què consisteix

## Fitxer WSDL

## Protocol SOAP

## UDDI

## Tipus d’atacs o vulnerablitats: Funcionament i propòsit



# Servei VoIP

## Funcionament

## Inconvenients i avantatges sobre la telefonia convencional.

## Elements que participen en el servei

## Protocol RTP i RTCP

## Protocol H323

## Protocol SIP

## Vulnerabilitats i atacs al servei VoIP