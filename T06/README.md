
## T06: Configuració del domini

[solucio de la tasca](SOLUCIO.md)

# Desplegament del domini

## Introducció
Un cop tenim ja el nostre domini creat, el següent pas és desplegar el domini, és a dir, crear els diferents objectes que el formen: grups, usuaris i màquines.  
En aquesta pràctica veurem la utilitat d’organitzar els objectes mitjançant **unitats organitzatives (OU)**.

## Procediment pràctic

### 1. Creació de les unitats organitzatives
Crear una estructura d’unitats organitzatives que sigui coherent i **justificar la decisió** presa.

### 2. Definició de l’estructura de grups
Definir la següent estructura de grups:
- **gestio**
- **magatzem**
- **gerencia**
- **personal**

> Tots els grups anteriors han de ser membres del grup **personal**.

### 3. Creació de plantilles d’usuari
Crear una plantilla d’usuari per a cadascun dels grups següents:
- Gestio  
- Magatzem  
- Gerencia  

Cada plantilla ha de tenir:
- Definida la **pertinença al grup corresponent**
- Configurada la **creació de la carpeta personal**

### 4. Usuaris de prova
Definir un **usuari de prova** per cadascuna de les plantilles creades.

### 5. Aprovisionament d’un equip
- Aprovisionar un equip anomenat **PC1** dins la **OU equips**.
- Crear una **màquina virtual amb Windows 11** amb les característiques següents:
  - 4 GB de RAM
  - Disc dur amb capacitat suficient
  - Xarxa configurada en **NAT**
- Un cop creat l’equip, **afegir-lo al domini**.

### 6. Comprovació del funcionament
Comprovar el correcte funcionament iniciant sessió a l’equip client (**PC1**) amb:
- L’usuari de prova de Gestio
- L’usuari de prova de Magatzem
- L’usuari de prova de Gerencia

## Materials i enllaços de suport
- **UD6.AA3 Desplegament**  
  Moodle 0224 SOX
