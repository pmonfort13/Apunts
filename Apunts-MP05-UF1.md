# APUNTS FINALS UF1

## Introducció als sistemes informàtics

- **Informació**: Resultat de manipular i processar un conjunt de dades per obtenir nou coneixement per a un individu o sistema
  - Com és? → gràfica, textual, audio, multimèdia…

- **Comunicació**: Procés on dos o més elements es relacionen intercanviant missatges per mitjà d’un canal. Elements:
  - Emissor
  - Receptor
  - Missatge
  - Canal
  - Codi

- **Informàtica**: Ciència que estudia el tractament automàtic i racional de la informació.
  - Permet automatitzar treballs rutinaris i repetitius.
  - Tasques amb més precisió i rapidesa.

- **Sistema informàtic**: Conjunt d’elements que permeten la realització i utilització d’aplicacions informàtiques. Permet el tractament de la informació automàticament:
  - Entrada: Recollir dades
  - Processament: aritmètic i lògic
  - Sortida: recollida i transmissió del resultat.

- **Elements d’un sistema informàtic**:
  - Part física: Hardware (maquinari)
  - Part lògica: Software (Programari)
  - Part humana

- **Hardware**: Format per:
  - Monitor
  - Teclat
  - CPU
  - Targetes de memòria
  - Dispositius de xarxa
  - Emmagatzament (HDD, SSD…)

- **Software**: No podem veure ni tocar → Fa referència a les idees i conceptes.
  - Sistemes operatius, aplicacions, jocs, eines d’internet….

- **Part Humana**: Element que permet la manipulació del hardware i software. Rols dins d’un sistema informàtic:
  - Usuari directe: Utilitza la informàtica per fer el seu treball.
  - Usuari indirecte: Reben els resultats del sistema informàtic.
  - Personal informàtic: Controlen i manipulen el hardware i software per poder donar servei als usuaris.

## Unitats funcionals de l’ordinador

- **Característiques d’un ordinador**:
  - Capacitat de fer càlculs matemàtics i operacions lògiques
  - Opera a alta velocitat
  - Exacte, precís i fiable
  - Executa programes
  - Capacitat per manipular grans quantitats d’informació

- **Arquitectura Von Neumann**: Funcionament
  - Programes i dades → Guardats en una memòria comuna (Memòria principal)
  - Execució de programes de forma seqüencial
  - Cada cel·la de memòria s’identifica amb una adreça
  - Tots els elements es comuniquen amb els busos del sistema
  - Altres dispositius (controladors), gestionen aquesta comunicació per l'eficiència del sistema.

- **Esquema**:
  
  ![Esquema](esquema.png)

- **Unitat central de processament (CPU)**:
  - Cervell de l’ordinador
  - Tasques:
    - Agafa cadascuna de les ordres del programa que hi ha a la memòria.
    - Les analitza i les interpreta.
    - Dóna les ordres necessàries per a executar-les.
  - Formada per circuits electrònics que en un microordinador es troben integrats en un xip denominat microprocessador.

- **Components de la CPU (Arquitectura Neumann)**:
  - *EXPLICAR LES PARTS I ESQUEMA DE CADA COMPONENT D’AQUESTA CPU*
    - Registres interns
    - ALU
    - Unitat de control (CU)
    - Arquitectures

- **Fabricants de CPU**: Intel, AMD, ARM, TSMC, IBM, Apple, Motorola, Entre altres.

## Tipus d’ordinadors

- **Segons la mida**
- **Segons l’ús**
- **SuperOrdinadors**
- **Mainframes**
- **Miniordinador**
- **Microordinador**
- **Quin maquinari ha de conèixer un AdminSis?**
  - Components físics de l’ordinador

## Placa Base

- És l’element més important de l’ordinador
- Plena de components electrònics, xips, connectors, jumpers, sòcols, etc., que permeten.
- El factor de forma determina la mida i orientació de la placa dins la caixa, tipus de font d’alimentació i perifèrics que s’hi poden integrar.
  - Quina placa base tinc?
    - Per obtenir model de la placa base
      - Windows → obrir cmd.
      - Executar: `wmic baseboard get product, Manufacturer,version,serialnumber, Model, Name`
    - També es pot obtenir a la utilitat
    - També es pot obtenir a la utilitat System Information o amb aplicacions com CPU-Z
    - A Linux `dmidecode -t 2` o amb eines com hardinfo.

- **Factors de forma**:
  - ATX
    - 1995
    - Mides màximes
      - ATX
      - MicroATX
      - MiniATX
      - FlexATX
      - ExtendedATX
  - ITX
    - 2001
    - Equips petits amb molts components
    - Mides màximes
      - Mini-ITX:
      - Nano-I9TX
      - PIco-ITX
      - Mobile-ITX

- **Sòcol CPU**:
  - Espai de la placa base on es connecta el processador (CPU).
  - Cada tipus de sòcol accepta una llista de processadors compatibles i generalment un mateix fabricant (Intel o AMD).

- **Tipus de sòcol**:
  - Tipus LGA (Land Grid Array)
    - Els pins que connecten la placa base i la CPU es troben al sòcol.
    - Disposa d’un sistema per fixar el processador que subjecta tota la CPU
  - Tipus PGA
    - Els pins es troben al processador i al sòcol trobem els forats on s’insereixen
    - El sistema de retenció només té una palanca lateral

- **Models de sòcol més recents**
  - **INTEL**
    - LGA 4189
    - LGA 1200
    - LGA 1700 
    - LGA 4677 (servidor)

  - **AMD**
    - Socket AM4 
    - Socket SP3 (servidor)
    - Socket TR4/TRX4 
    - Socket AM5
    - Socket SP5 (servidor)

## Sòcols de memòria
Lloc on s’instal·la la memòria RAM Actualment →  de tipus DIMM (Dual in line Memory) Trobem els tipus DDR4 i DDR5 de 288pins. En cas de múltiples ranures, cal seguir les especificacions que indiquen quines ranures utilitzar per aprofitar tecnologies com DUAL CHANNEL.

## Xipset

## Caixa i Font d’alimentació

### Caixa:
- Part que serveix de suport i d’esquelet per allotjar les peces bàsiques d’un ordinador
- Pot ser fibra o titani, temperat, fins d’alumini o acer
- Parts d’una caixa:
  - Badies
    - S’utilitzen per muntar-hi unitats de disquetera, discs durs, CD ROM..
  - Mides:
    - 2,5 polzades (disc dur, disc SSD)
    - 3,5 polzades (disquetera de 3 ½, lector de targetes, discs durs, etc.)
    - 5,5 polzades (DVD ROM)
  - Tipus
    - Internes: disc dur, disc SSD
    - Externes: DVD ROM, lector targetes..
  - Interruptors
    - POWER (botó d’engegada)
    - RESET: reinicia l’ordinador.
    - Botó d’interrupció de la font d’alimentació per tallar l’entrada d’electricitat a la font.
  - LEDs
    - PWR_LED: s'il·lumina quan l’ordinador està encès.
    - HDD_LED: s'il·lumina quan s’accedeix al disc dur.

### Tipus de caixes:
- Torre servidor
  - S’usen en les instal·lacions de servidors
  - Múltiples badies externes e internes
  - Ventilació addicional 
  - Preparades per a plaques de servidor i fonts d’alimentació més potents.
- Armari Rack
  - Usades per a muntar servidors en rack
  - Excel·lent fluxe de l’aire
  - Flexibilitat en el cablejat
  - Solen tenir portes amb clau
  - Cada rack és independent.
  - No permet canvi en calent.
- Xassís Blade
  - Petits i fins.
  - Optimitza l’ordre i l’espai.
  - Xassís flexible i escalable
  - Major eficiència energètica
  - Habituals en data centers
  - Cada blade pot funcionar conjuntament amb altres servidors del mateix xassís.
  - Permeten canvis en calent.

## Ventilació
- Cal monitorizar la temperatura de l’interior de la caixa
- Ventilador a la part posterior de la caixa que expulsi l’aire calent de CPU i targeta gràfica
- S’ha de crear un flux d’aire que faciliti l’expulsió d’aire calent.
- La majoria de caixes incorporen ventiladors addicionals.

## Font d’alimentació
- Transformen els 220 alterns de la xarxa elèctrica en valors inferiors de corrent continu.
- Disposa d’un fusible que es fon en cas de consum excessiu o curtcircuit per a protegir l’ordinador.
- **Tipus de font**
  - ATX
    - Entrada: 180/264V
    - Sortida: 3,3V,5V,12V,-12V,-5V
    - Potències: 350W,450W,6502,750W,850W,950W
  - Altres
    - SFX
      - Dimensions inferiors a les ATX
      - Usades en barebones o equips de perfil baix
    - EPS
      - Estàndard SSI (Server System Infrastructure)
      - Connector de 24 pins i de 8 pins (1 de cada)
- **Factor de pòtencia**
  - Relació entre potència activa (real) i aparent (nominal)
  - Exemple: si una font de 500W entrega 500W reals, el seu factor de potència seria 1
  - Un factor de potència és millor quan més a prop d’1 es troba.
- Power Factor Correction: Mesura de correcció que la font realment entrega per per aproximar-la a un factor de potència 1.

- **Certificacions:**
  - Diferents nivell en base a la seva eficència (menys a més)
    - 80 PLUS
    - 80 PLUS Bronze
    - 80 PLUS Silver
    - 80 PLUS Gold
    - 80 PLUS Platinum
    - 80 PLUS Titanium
- **Fonts d’alimentació: Modulars**
  - Sèrie de connectors dels quals només es connecten els cables que usem.
  - Millor ventilació
  - Millor aprofitació de la potència subministrada
- **Fonts d’alimentació: Redundants**
  - Usats sobretot en servidors
  - Dues fonts connectades a diferents sistemes elèctrics per tal de garantir el subministrament a l’equip
- **Potència d'una font d’alimentació**
  - Totes les fonts d’alimentació tenen una potència nominal de treball per damunt de la qual no poden funcionar
  - Es mesura en Watts (W)
  - Sol estar entre 500 i 800 W
  - És difícil que la font arribi a entregar la potència indicada per l’etiqueta
  - En el cas que passi pot causar el següent:
    - Sistema inestable
    - Còpia de dades entre discos realitzada incorrectament.
- **Consells sobre la font d’alimentació**
  - Anar amb compte de tocar el selector de voltatge (si existeix)
  - És convenient revisar periòdicament l’estat del ventilador de la font


- Còpia de dades entre discos realitzada incorrectament.
  - Consells sobre la font d’alimentació
    - Anar amb compte de tocar el selector de voltatge (si existeix)
    - És convenient revisar periòdicament l’estat del ventilador de la font

## BIOS (Basic Input-Output System)

- Programa o conjunt de programes elementals gravats en un circuit integrat.
- És Firmware i el xip on està emmagatzemat sol ser de tipus EEPROM.
- Primer programa que s’executa al arrencar l’ordinador.

### Funcions de la BIOS:
- Principal: comprovar que tot el hardware estigui OK per a posteriorment donar pas a la càrrega del sistema operatiu en la memòria RAM.
- Carrega les funcions de gestió d’energia i temperatura del ordinador.
- El sistema operatiu està emmagatzemat en el disc dur encara que també es pot arrencar des d’un DVD/CD
- Al arrancar l’ordinador caldrà comprovar:
  - A quin dispositiu està el S.O. (CD, HDD, etc.).
  - Si està correctament connectat.
  - Reconèixer el seu tipus.

### Procés d’arrencada
- Test del Hardware (anomenat POST)
- S’activa la targeta gràfica
- Proves sobre el sistema
- Configuració dels dispositius detectats
- Inici de la càrrega del S.O

### Test POST (Power On Self Test)
- S’encarrega de verificar i inicialitzar els components d’entrada i sortida al arrencar l’ordinador
- Si detecta un error, emet avisos sonors
- Cada BIOS té el seu propi codi/idioma per a identificar el tipus de problema 

### DualBIOS
- Incorporar 2 unitats físiques
  - Un xip → BIOS “Principal”
  - Segon xip → BIOS “Backup”
- Si la BIOS “Principal” falla:
  - La BIOS “backup” copia la BIOS “Principal”

### Actualitzar BIOS
- Substituir el programa emmagatzemat en el xip de la BIOS o firmware
- És possible configurar alguna característica de la BIOS en el menú setup al que es pot accedir just al arrencar l’ordinador
- Aquest menú és imprescindible per a canviar els paràmetres del CMOS 

### CMOS (Complementary Metal-Oxide-Semiconductor)
- Quan parlem de CMOS ens referim a un xip de la placa base el qual conté totes les dades de configuració necessàries per a l’arrencada de l’ordinador
- En la placa base BIOS i CMOS són xips diferents.
- És memòria volàtil per lo qual necessita estar contínuament alimentada per a no perdre les dades que conté. Per tant, es necessita una bateria o pila.

### Pila
- Bateria subministra energia a la CMOS i es carrega de corrent quan l’equip es troba encès
- Si la pila deixa de funcionar, la CMOS s’esborra.
- Actualment, encara que es segueix anomenant CMOS a aquest xip també s’implementa amb tecnologia EEPROM.
- Quan es desitja voluntàriament esborrar la CMOS cal utilitzar el resetejador de la placa base. Abans era suficient amb treure la pila durant uns segons amb l’ordinador apagat.

### CMOS/BIOS Setup 
- Aquest menú bàsicament permet les següents accions:
  - Configurar el hardware de l’equip
  - Establir la data i l’hora del sistema
  - Activar o desactivar certs components del sistema
  - Escollir quins dispositius i en quin ordre es cridaran per a carregar el sistema operatiu (seqüència d’arrencada)
  - Establir passwords per a restringir l’accés al computador.

## UEFI (Unified Extensible Firmware Interface)
- Escrit en C
- Funcions addicionals:
  - Interfície gràfica més moderna.
  - Sistema d’inici segur.
  - Major velocitat al arrencar.
  - Suport per discos de més de 2TB.

### UEFI vs BIOS 
- BIOS aspecte d’MS-DOS. UEFI Interfície gràfica més moderna.
- BIOS utilitza 16 bits, mentre que UEFI 32 o 64 bits.
- BIOS suporta fins a 4 particions i discs durs de 2,2 TB.
- Utilitzen l’esquema de particions MBR. UEFI utilitza el GPT (GUID Partition Table) més modern. El límit seria discos amb capacitat de fins a 9,4 zettabytes, i fins a 128 particions.
- Amb UEFI l’arrancada és més ràpida.
- UEFI implementa l’opció Secure Boot. Evita l’inici de sistemes operatius que no estiguin autenticats, per protegir-se dels bootkits.
- El xip de memòria en que ve instal·lada la UEFI no està bloquejat en la placa base. Es poden afegir extensions, com eines d’overclocking o software de diagnòstic

## Microprocessadors

### Característiques:
- Component principal de l’ordinador
- Fa les operacions matemàtiques i lògiques i coordina els elements de l’ordinador.
- Composat de milers o, fins i tot, milions de transistors. 
- Sol ser rectangular i disposa d’una sèrie de potes, connectors o contactes per tal de comunicar informació amb la resta de components

### Arquitectura
- Processadors CISC (Complex Instruction Set Computer)
  - Joc d’instrucció molt ampli
  - Format variable d’instrucció
  - Algunes instruccions més llargues que altres i amb diferents nombres de camps.
  - Unitat de control microprogramada.
  - Disseny electrònic complex pel seu gran nombre d’instruccions
  - Fa complicat augmentar la freqüència de funcionament.
- Processadors RISC (Reduced Instruction Set Computer)
  - Joc d’instruccions més reduït i simple 
  - Electrònica més simple
