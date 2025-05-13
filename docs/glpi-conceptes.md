# Conceptes bàsics de GLPI

Aquest document explica els principals conceptes de GLPI (Gestionnaire Libre de Parc Informatique) perquè els puguis entendre de manera autònoma. GLPI és una eina de gestió d’inventari i serveis TIC molt utilitzada per administradors de sistemes.

---

## 1. Components

Els **components** són les peces físiques que formen part d’un equip informàtic (com ara un ordinador o un servidor). No són equips sencers, sinó parts internes.

### Exemples de components:
- Memòria RAM
- Discos durs (HDD o SSD)
- Targetes gràfiques
- Processadors (CPU)

**Per a què serveixen?**  
Permeten tenir un control precís del maquinari de cada dispositiu i gestionar reemplaçaments, errors o ampliacions.

---

## 2. Software

El **software** inclou tot el programari instal·lat als dispositius de l’organització.

### Dades que es poden gestionar:
- Nom del programa
- Versió
- Llicència (quantitat permesa, clau, caducitat)
- Ordinadors on està instal·lat

**Per a què serveix?**  
Per controlar quins programes hi ha als equips, evitar incompliments de llicències i organitzar les instal·lacions.

---

## 3. Connexions

Les **connexions** mostren com es relacionen els dispositius entre ells, ja sigui a nivell físic (xarxa, cables) o lògic (dependències).

### Exemples:
- Un ordinador connectat a una impressora
- Un switch connectat a diversos ordinadors
- Un servidor relacionat amb una unitat d’emmagatzematge externa (SAN)

**Per a què serveixen?**  
Per visualitzar i entendre la infraestructura i resoldre problemes de connexió o dependències.

---

## 4. Usuaris

Els **usuaris** són les persones que poden fer servir els serveis de GLPI o que hi tenen associació com a sol·licitants, tècnics o administradors.

### Informació habitual:
- Nom i cognoms
- Correu electrònic
- Departament
- Rol dins l’organització (usuari, tècnic, administrador)
- Autenticació (GLPI local, LDAP...)

**Per a què serveixen?**  
Per saber qui fa què, controlar permisos i gestionar tickets o assignacions.

---

## 5. Plantilles (Templates)

Les **plantilles** són models predefinits que ajuden a crear elements ràpidament i de forma estandarditzada.

### Exemples:
- Una plantilla per nous ordinadors (amb sistema operatiu, ubicació i departament per defecte)
- Una plantilla per tickets recurrents (com ara incidències habituals)

**Per a què serveixen?**  
Per estalviar temps, mantenir la coherència i evitar errors humans.

---

## 6. Ordinadors

Els **ordinadors** són dispositius informàtics registrats al sistema GLPI.

### Informació típica:
- Marca i model
- Número de sèrie
- Sistema operatiu
- Components associats
- Software instal·lat
- Ubicació
- Usuari assignat

**Per a què serveixen?**  
Per tenir un registre complet i ordenat de tot el parc informàtic.

---

## 7. Tasques de manteniment

Les **tasques de manteniment** són accions periòdiques o puntuals que es programen per garantir el bon funcionament dels equips.

### Exemples:
- Revisió d’impressores cada 6 mesos
- Neteja interna d’ordinadors
- Renovació d’antivirus

**Per a què serveixen?**  
Per evitar problemes futurs, mantenir els equips en bon estat i fer seguiment del manteniment preventiu.

---

## 8. Incidències (Tickets)

Les **incidències** o **tickets** són peticions o problemes que els usuaris comuniquen a l’equip tècnic.

### Informació d’un ticket:
- Descripció del problema
- Prioritat i estat
- Equip afectat
- Usuari que el reporta
- Tècnic assignat
- Historial de seguiment

**Per a què serveixen?**  
Per gestionar el servei tècnic, registrar els problemes i garantir una resposta organitzada i eficaç.

---

## Resum ràpid

| Concepte       | Descripció                                 | Exemple pràctic                         |
|----------------|---------------------------------------------|------------------------------------------|
| Components     | Peces internes dels equips                  | Disc SSD, RAM, CPU                       |
| Software       | Programes instal·lats                       | Microsoft Office, antivirus              |
| Connexions     | Relacions entre dispositius                 | PC connectat a una impressora            |
| Usuaris        | Persones vinculades a GLPI                  | Maria López, tècnica informàtica         |
| Plantilles     | Models per crear elements ràpidament        | Plantilla per ordinadors nous            |
| Ordinadors     | Dispositius informàtics                     | Portàtil Lenovo amb Windows 11           |
| Manteniment    | Accions tècniques programades               | Revisió semestral d’equips               |
| Incidències    | Peticions i problemes dels usuaris          | "El correu no funciona", ticket ID 2345  |

---

Aquest document està pensat per ajudar-te a entendre les bases de GLPI. Si tens dubtes, pots revisar la documentació oficial o consultar amb el teu professor o professora.
