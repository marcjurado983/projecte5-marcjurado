# P02 — Llicenciament Windows Server 2025

https://docs.google.com/presentation/d/1qGmhKzN4H3WoyzyCgwpLoRYyg9aacayynR99o5SL_4o/edit?usp=sharing

## Context del projecte

Mentre inicieu la vostra aventura emprenedora, cal continuar generant ingressos.  

Gràcies a la bona feina desenvolupada a **EverPia**, la consultora ha decidit donar-vos suport derivant-vos projectes de clients que actualment no poden assumir.

---

# Introducció al client

## 🏢 Empresa: TransLògic S.A.

Empresa dedicada a la logística regional que vol renovar completament la seva infraestructura de servidors migrat a **Windows Server 2025**.

Actualment disposen d’un servidor físic antic que ha quedat obsolet i volen:

- modernitzar la infraestructura,
- virtualitzar els serveis,
- millorar disponibilitat,
- i facilitar l’escalabilitat futura.

---

# Infraestructura actual

## 🖥️ Servidor físic (Host)

### Característiques:
- 1 servidor físic
- 2 processadors (CPU)
- 12 nuclis físics per processador

### Total:
- **24 cores físics**

---

# Càrrega de treball virtualitzada

## 🧩 Màquines virtuals (VMs)

### Serveis principals:
- 1 VM — Controlador de Domini (Active Directory)
- 1 VM — Servidor de Fitxers
- 1 VM — Servidor d’Impressió i Gestió Documental
- 1 VM — SQL Server (ERP)

### Serveis de suport:
- 8 VMs per aplicacions de logística i terminals de magatzem

---

## 🔢 Total:
- **12 màquines virtuals amb Windows Server**

---

# Usuaris i dispositius

## 👥 Personal
- 45 empleats totals

### Oficina
- 30 treballadors
- Cada treballador disposa de:
  - PC
  - portàtil

### Magatzem
- 15 mossos de magatzem
- Comparteixen:
  - 5 tauletes robustes
- Funcionament:
  - 3 torns de treball

---

# Encàrrec del client

Com a consultors informàtics, haureu de:

## 1️⃣ Analitzar el model de llicenciament per nucli
Estudiar el funcionament del model de llicenciament **per core** de Windows Server 2025.

---

## 2️⃣ Calcular el cost total

Comparar les dues edicions principals:

- Windows Server 2025 Standard
- Windows Server 2025 Datacenter

Caldrà calcular:
- llicències per nucli,
- drets de virtualització,
- cost total aproximat.

---

## 3️⃣ Analitzar les CALs

Determinar quin model és més econòmic:

- User CAL
- Device CAL

Justificant:
- nombre d’usuaris,
- nombre de dispositius,
- ús compartit.

---

## 4️⃣ Justificar la proposta final

La decisió final haurà d’incloure:

### 💰 Costos
- cost inicial,
- costos futurs,
- impacte en ampliacions.

### 📈 Escalabilitat
- possibilitat de créixer,
- noves VMs,
- alta disponibilitat.

### ⚙️ Funcionalitats avançades
Exemple:
- Storage Spaces Direct
- Software Defined Networking (SDN)
- virtualització avançada
- seguretat millorada

---

## 5️⃣ Presentació al client

Crear una presentació oral de:
- entre 5 i 10 minuts

Objectiu:
- explicar la proposta de manera clara,
- orientada a un perfil no tècnic,
- pensada per al gerent de TransLògic.

---

# Materials i recursos de suport

## 📘 Moodle
- UD6.AA1 — Introducció a Windows Server  
  *(Moodle 0224 SOX)*

---

## 🌐 Microsoft
- Preus i llicències de Windows Server
- Documentació oficial de llicenciament
- Comparativa Standard vs Datacenter****
