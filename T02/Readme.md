# T02: Control de versions. Treballant amb git

# Treball amb Git Local + GitHub

Fins ara hem gestionat el control de versions utilitzant directament el repositori des de la web de GitHub. Tot i que això ens ha solucionat força problemes, és evident que aquesta metodologia té diverses limitacions:

## Limitacions de treballar només des de GitHub Web

### 🐌 Lentitud a l’hora d’editar
L’editor web no és tan versàtil com un editor local, ja sigui:

- editors de codi com **Visual Studio Code**,
- o editors específics de Markdown com **Ghostwriter**.

### 📁 Gestió complicada del repositori
Afegir:

- arxius,
- carpetes,
- reorganitzar contingut,

pot resultar força feixuc i requereix accions poc eficients.

---

# Nova metodologia de treball

Per aquest motiu, començarem a treballar de la forma habitual en entorns professionals:

- combinant el control de versions local amb **git**,
- i un gestor de repositoris remots, en aquest cas **GitHub**.

GitHub no és l’única solució existent. Hi ha alternatives molt utilitzades com:

- GitLab,
- Bitbucket,
- Azure DevOps,
- entre d’altres.

---

# Una mica d’història

De fet, **git** va aparèixer abans que GitHub.

Va néixer com un sistema de control de versions descentralitzat que va revolucionar el model centralitzat que predominava en aquell moment.

Va ser creat per **Linus Torvalds**, creador del sistema operatiu Linux.

---

# Flux de treball que seguirem

## 1️⃣ Repositori remot a GitHub

Sempre partirem d’un repositori existent a GitHub.

## 2️⃣ Clonar el repositori en local

El primer pas serà tenir una còpia sincronitzada al nostre ordinador:

```bash
git clone URL_DEL_REPOSITORI
