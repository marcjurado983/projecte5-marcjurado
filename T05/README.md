# T05 – Instal·lació del domini (Active Directory)

[solucio de la tasca](SOLUCIO.md)

## Introducció

Com a continuació de la tasca **T04 – Instal·lació de Windows Server 2025**, es procedeix al desplegament del **Directori Actiu (Active Directory Domain Services)** sobre la màquina virtual creada prèviament.

Aquest procés té com a objectiu practicar el desplegament d’un domini abans de la seva implantació real en el client **TransLògic S.A.**.  
A més, aquesta instal·lació serveix com a **Prova de Concepte (PoC)** per poder mostrar el funcionament als responsables de l’empresa i ajustar la configuració a les necessitats reals del client.

---

## Objectius

- Instal·lar els rols necessaris per al Directori Actiu.
- Crear un **nou domini en un bosc nou**.
- Establir el **nivell funcional del domini a 2025**.
- Promocionar el servidor com a **Controlador de Domini (DC)**.
- Automatitzar el procés mitjançant **PowerShell**.
- Emmagatzemar l’script dins del repositori del projecte.

---

## 1. Instal·lació dels rols necessaris

### Rols instal·lats

- **Active Directory Domain Services (AD DS)**
- **DNS Server** (instal·lat automàticament)

### Procediment

1. Obrir **Server Manager**.
2. Seleccionar **Add roles and features**.
3. Tipus d’instal·lació: *Role-based or feature-based installation*.
4. Seleccionar el servidor local.
5. Marcar el rol **Active Directory Domain Services**.
6. Acceptar les característiques addicionals (DNS).
7. Iniciar la instal·lació.

📸 *Captura recomanada: selecció del rol AD DS*

---

## 2. Creació del domini

### Dades del domini

| Paràmetre | Valor |
|--------|------|
| Tipus | Nou bosc |
| Nom del domini | `translogicXX.test` |
| Nivell funcional | Windows Server 2025 |
| Servidor DNS | Sí |
| GC | Sí |

> **Nota:** `XX` correspon al número de llista de l’alumne.

---

## 3. Promoció del servidor a Controlador de Domini

### Procediment

1. Un cop instal·lat el rol, prémer **Promote this server to a domain controller**.
2. Seleccionar:
   - **Add a new forest**
   - Nom del domini: `translogicXX.test`
3. Establir:
   - Forest functional level: **Windows Server 2025**
   - Domain functional level: **Windows Server 2025**
4. Configurar la contrasenya del **Directory Services Restore Mode (DSRM)**.
5. Verificar els prerequisits.
6. Confirmar la configuració.

📸 **Important:**  
És obligatori documentar amb captura la **pantalla de resum** abans de finalitzar la promoció.

7. Iniciar el procés i reiniciar el servidor automàticament.

---

## 4. Automatització amb PowerShell

Per facilitar futurs desplegaments, s’ha creat un **script PowerShell** que automatitza el procés d’instal·lació del Directori Actiu i la promoció del servidor.



