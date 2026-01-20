# REPTE: MALWARE I PROGRAMARI ANTIMALWARE

## Marc jurado

## per veure el resultat de la tasca: (guia.md)
---

## Instruccions generals

**Molt important**

- Poseu el nom i cognoms al document.
- Copieu l’enunciat.
- Poseu les preguntes ressaltades i la resposta a sota.
- Responeu a totes les preguntes, si cal cercant informació als apunts del mòdul, manuals, fitxers d’ajuda (`man`) o, com a últim recurs, a Internet.
- Abans de començar feu un **snapshot (instantània)** de la màquina virtual.
  - Nom del snapshot: **"Abans de (l'acció que aneu a fer)"**
- En acabar cada prova, revertiu la instantània.
- Comproveu **sempre** que els canvis produeixen l’efecte desitjat.

---

## Referències i ajuda

- Apunts del mòdul (secció de malware)
- ISO de Windows 11 (comuna)
- Mesures davant ransomware:
  - https://www.lmgsecurity.com/download/655360/
  - https://www.groupsense.io/services/ransomware-negotiation

---

## Objectius

L’objectiu d’aquesta pràctica és:
- Comprovar el funcionament del malware
- Treballar amb programari de protecció antimalware
- Analitzar mecanismes de protecció contra ransomware a Windows 11

---

## Activitat 1: Verificació del funcionament d’un programari antimalware

### Desactivació de SmartScreen

El navegador web de Windows incorpora **SmartScreen**, un sistema de detecció de llocs i fitxers potencialment perillosos.

**Pregunta:**  
**Expliqueu com desactivar SmartScreen a Windows 11 i al navegador.**

**Resposta:**  
_(Resposta de l’alumne)_

---

### Test EICAR

Seguiu les instruccions de https://www.eicar.org per descarregar el fitxer de prova EICAR.

Pot ser necessari desactivar temporalment:
- Protecció del navegador
- Antimalware de Windows

**Pregunta:**  
**Expliqueu com heu desactivat temporalment la protecció del navegador i de Windows Defender.**

**Resposta:**  
_(Resposta de l’alumne)_

---

### Detecció del fitxer EICAR

1. Activeu l’antimalware.
2. Comproveu si detecta el fitxer EICAR.

**Pregunta:**  
**L’antimalware detecta el fitxer EICAR? Quin missatge mostra?**

**Resposta:**  
_(Resposta de l’alumne)_

---

### EICAR comprimit

1. Desactiveu la detecció en temps real.
2. Comprimiu el fitxer EICAR en diferents formats.
3. Torneu a activar l’antimalware.

**Indiqueu si l’amenaça és detectada en cada cas:**

- **ZIP:**  
  _(Resposta)_

- **TAR:**  
  _(Resposta)_

- **7ZIP:**  
  _(Resposta)_

---

## Activitat 2: Sistemes de protecció de Windows 11

### Protecció antivirus i contra amenaces

**Pregunta:**  
**Quines proteccions incorpora Windows 11 a la secció "Protección antivirus y contra amenazas"?**

**Resposta:**  
_(Resposta de l’alumne)_

---

### Control d’aplicacions i navegador

**Pregunta:**  
**Quines opcions hi ha a "Control de aplicaciones y navegador"?**

**Resposta:**  
_(Resposta de l’alumne)_

---

### Protecció contra ransomware

**Pregunta:**  
**Quines opcions específiques hi ha per la protecció contra ransomware a Windows 11?**

**Resposta:**  
_(Resposta de l’alumne)_

---

## Activitat 3: Prova pràctica de protecció contra ransomware

### Preparació

1. Afegiu diversos fitxers `.txt` dins la carpeta **Documents**.
2. Desactiveu la protecció contra ransomware (si està activa).

---

### PSRansom (simulació de ransomware)

Repositori:  
https://github.com/JoelGMSec/PSRansom

Canvieu la política d’execució de PowerShell:

```powershell
Set-ExecutionPolicy -ExecutionPolicy unrestricted



