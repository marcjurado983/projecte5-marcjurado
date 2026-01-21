# T04 – Instal·lació de Windows Server 2025

[solucio de la tasca](SOLUCIO.md)

## Context del projecte

Després del nostre assessorament inicial, **TransLògic S.A.** ens encarrega el desplegament dels seus servidors basats en **Windows Server 2025**.

Amb l’objectiu de seguir bones pràctiques i optimitzar el procés, es realitza una **instal·lació de prova** mitjançant màquines virtuals. Aquesta instal·lació servirà tant per aprendre els procediments com per elaborar una **guia de referència**, que facilitarà la futura implantació als sistemes del client.

---

## Objectius

- Realitzar una instal·lació correcta de Windows Server 2025 en entorn virtualitzat.
- Documentar tot el procés seguint un format **Markdown**.
- Comparar la configuració de la màquina virtual amb els **requisits oficials de Microsoft**.
- Generar documentació reutilitzable per a futurs desplegaments.

---

## 1. Configuració de la màquina virtual

### Característiques de la VM

| Component | Configuració |
|--------|--------------|
| Memòria RAM | 8 GB |
| Processadors | 2 CPU |
| Disc principal | 32 GB (Sistema Operatiu) |
| Disc secundari | 10 GB |
| Xarxa 1 | NAT (no NAT intern) |
| Xarxa 2 | Host-only |
| Mode d’instal·lació | GUI |
| Idioma del sistema | English (US) |
| Configuració regional | Espanyol |
| Teclat | Espanyol |

---

## 2. Comparació amb els requisits de Microsoft

### Requisits mínims de Windows Server 2025 (Microsoft)

| Requisit | Mínim Microsoft | VM configurada |
|--------|----------------|----------------|
| CPU | 1.4 GHz, 64-bit, 2 cores | 2 cores ✔️ |
| RAM | 2 GB (GUI) | 8 GB ✔️ |
| Emmagatzematge | 32 GB | 42 GB totals ✔️ |
| Xarxa | Adaptador Ethernet | 2 adaptadors ✔️ |
| Firmware | UEFI amb Secure Boot | Compatible ✔️ |

### Conclusió

La configuració de la màquina virtual és **coherent i superior** als requisits mínims establerts per Microsoft.  
Aquesta configuració garanteix estabilitat, bon rendiment i marge suficient per a serveis addicionals (com Active Directory).

---

## 3. Procediment d’instal·lació

### 3.1 Creació de la màquina virtual

1. Crear una nova màquina virtual al programari de virtualització.
2. Assignar:
   - 8 GB de RAM
   - 2 CPU
3. Afegir dos discos virtuals:
   - Disc 1: 32 GB (principal)
   - Disc 2: 10 GB (secundari)
4. Configurar dues interfícies de xarxa:
   - Adaptador 1: NAT
   - Adaptador 2: Host-only

📸 *Captura recomanada: configuració general de la VM*

---

### 3.2 Instal·lació de Windows Server 2025

1. Arrencar la VM amb la ISO de Windows Server 2025.
2. Seleccionar:
   - Language: **English (United States)**
   - Time & currency format: **Spanish**
   - Keyboard: **Spanish**
3. Escollir **Windows Server 2025 Standard (Desktop Experience)**.
4. Acceptar la llicència.
5. Seleccionar instal·lació personalitzada.
6. Instal·lar el sistema al disc de 32 GB.

📸 *Captura recomanada: selecció de versió i disc*

---

### 3.3 Configuració inicial del sistema

1. Establir la contrasenya de l’usuari **Administrator**.
2. Accedir al sistema.
3. Canviar el nom de l’equip:
   - Nom: **DCxx** (xx = número de lli
