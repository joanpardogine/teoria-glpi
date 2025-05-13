# Importació de dades a GLPI amb fitxers CSV

Aquest document explica com importar diferents tipus de dades a GLPI mitjançant fitxers CSV. Cal que tinguis permisos d'administrador i que estigui instal·lat el plugin **"Import from CSV"** (o similar).

---

## Requisits previs

1. Accedeix a GLPI com a **administrador**.
2. Assegura't que tens el plugin **<kbd>Import from CSV</kbd>** activat.
3. Ves a **Eines > Import from CSV**.
4. Tria el tipus d'element que vols importar (components, software, usuaris, etc.).

---

## Fitxers CSV disponibles

|Nom del fitxer|Contingut del fitxer|
|-----|-----|
|[**`components.csv`**](./components.csv)|components de maquinari|
|[**`software.csv`**](./software.csv)|aplicacions i programes|
|[**`connexions.csv`**](./connexions.csv)|relacions entre equips|
|[**`usuaris.csv`**](./usuaris.csv)|dades d'usuaris|
|[**`plantilles.csv`**](./plantilles.csv)|plantilles per a ordinadors|

Els fitxers tenen capçalera i utilitzen el separador **`;`** (punt i coma).

---

## Com importar cada tipus de dades

### 1. Components

1. Ves a **Eines > Import from CSV**.
1. Selecciona <kbd>Components</kbd>.
1. Puja el fitxer [**`components.csv`**](./components.csv).
1. Associa cada columna a un camp de GLPI.
1. Revisa la previsualització i confirma la importació.

### 2. Software
1. Ves a **Eines > Import from CSV**.
1. Selecciona <kbd>Software</kbd> com a tipus d'element.
1. Puja el fitxer [**`software.csv`**](./software.csv).
1. Posa atenció als camps: nom, versió, tipus de llicència.
1. Posa <kbd>Sí</kbd> o <kbd>No</kbd> si el software és lliure.

### 3. Connexions

1. Ves a **Eines > Import from CSV**.
1. Selecciona <kbd>Connexions entre ítems</kbd>.
1. Puja el fitxer [**`connexions.csv`**](./connexions.csv).
2. Aquest fitxer fa referència a equips existents. Cal que abans s'hagin importat.
3. Inclou camp origen, destí i tipus de connexió.

### 4. Usuaris

1. Ves a **Eines > Import from CSV**.
1. Selecciona <kbd>Usuaris</kbd>.
1. Puja el fitxer [**`usuaris.csv`**](./usuaris.csv).
1. Les columnes bàsiques són: **nom**, **cognoms**, **correu**, **nom d'usuari**, **perfil**, **entitat**.
1. Pots deixar en blanc camps com **telèfon** o **comentaris**.

### 5. Plantilles

1. Ves a **Eines > Import from CSV**.
1. Ves a <kbd>Plantilles</kbd> dins del menú de configuració d'ítems.
1. Puja el fitxer [**`plantilles.csv`**](./plantilles.csv).
1. En alguns casos cal importar des del mateix menú de l'ítem (ex: **Ordinadors** > **Plantilles**).
1. Pots definir valors per defecte (**SO**, **ubicació**, **departament**, ...).

---

## Recomanacions

- Utilitza fitxers amb **codificació `UTF-8`**.
- Assegura't que els **noms d'usuari**, **ubicacions** o **elements** ja existeixen si es referencien.
- Revisa bé les associacions de columnes abans d'importar.

---

## Prova

Prova d'importar cada fitxer en un entorn de proves. Un cop verificat, pots fer-ho en l'entorn real de producció.
