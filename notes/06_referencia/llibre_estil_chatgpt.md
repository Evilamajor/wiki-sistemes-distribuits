# Llibre d’estil del repositori “wiki-sistemes-distribuits”
Aquest document defineix com ChatGPT, Codex i GitHub Copilot han d’ajudar en el desenvolupament, millora i manteniment d’aquest repositori.

La finalitat del repositori és:
- Crear una base de coneixement personal i permanent sobre Sistemes Distribuïts.
- Documentar conceptes, protocols, arquitectures i pràctiques de l’assignatura.
- Preparar coneixement útil per al futur TFG i per a projectes professionals.
- Reutilitzar el contingut per estudiar, revisar i consolidar coneixements.

Aquest repositori **no és una PAC ni un exercici lliurat**, per tant l’ús d’IA és permès i recomanat.

---

## 1. Regles generals per a la IA
### 🔹 1.1. Quin tipus d’ajuda pot aportar ChatGPT?
ChatGPT pot:
- Explicar conceptes teòrics.
- Generar esquemes, resums i comparatives.
- Crear esquelets de documents Markdown.
- Millorar l’organització del repositori.
- Produir pseudocodi, diagrames Mermaid i estructures de codi.
- Ajudar a preparar entorns (devcontainers, scripts…).
- Fer revisió de contingut i suggerir millores.
- Completar carpetes i estructures d’apunts.
- Crear tasques per GitHub Projects (text).
- Millorar la qualitat pedagògica del contingut.
---

## 2. Estructura dels apunts
Quan ChatGPT contribueixi a un fitxer `.md`, ha de seguir aquesta estructura:

Títol del concepte
1. Definició clara

…

2. Motivació en sistemes distribuïts

…

3. Funcionament o regles

…

4. Exemple pràctic

…

5. Relació amb altres conceptes del repositori

Lamport clocks

Vector clocks

TSAE

6. Notes addicionals o comparativa

…


---

## 3. Esquema de diagrames amb Mermaid
ChatGPT pot generar diagrames utilitzant:

```mermaid
graph TD
    A[Node A] --> B[Node B]

4. Com ha de ser el codi generat

Simple, clar i ben comentat.

No més del necessari (minimal viable example).

Ha d’incloure instruccions d’execució.

Ha de situar-se dins codes/….

5. Estil de comunicació

Català correcte i formal, però pedagògic.

Explicacions pas a pas quan sigui necessari.

Evitar parrafades llargues.

Prioritzar esquemes, taules i punts.

6. Preguntes que pots fer a ChatGPT per utilitzar-lo com assistent del repo

Per exemple:

📄 Millora de documents

“Revisa aquest apunt i proposa millores segons el llibre d’estil.”

“Simplifica aquesta explicació seguint l’estructura dels apunts.”

🧠 Aprenentatge

“Explica’m Lamport clocks d’una manera que pugui afegir al meu apunt.”

🏗️ Organització

“Revisa l’estructura del repositori i proposa millores.”

“Genera la llista d’issues pendents segons el contingut actual.”

💻 Codi

“Genera un pseudocodi bàsic per mostrar com funciona TSAE fase 3.”

“Crea un script Python que simuli un vector clock senzill.”

7. Flux de treball recomanat

Crees un fitxer buit a notes/.

Demanes a ChatGPT:

“Omple aquest apunt seguint el llibre d’estil del repositori.”

Reviseu el contingut junts.

Fas git add, commit, push.

8. Objectiu final

Aconseguir que aquest repositori sigui un manual complet de Sistemes Distribuïts que et serveixi:

per repassar abans d’exàmens,

per preparar el TFG,

per recordar protocols i dissenys distribuïts en el futur.

9. Versió del document

Última actualització: 2025-12-03


---

# 🧠 **COM UTILITZAR AQUEST FITXER AMB CHATGPT O CODEX**

Cada cop que vulguis que ChatGPT treballi dins del repositori, només cal dir:

### 🟦 **Instrucció base**
> “Segueix el document *notes/06_referencia/llibre_estil_chatgpt.md* per generar aquest contingut.”

A partir d’aquí, pots demanar:

---

## 🟩 **Exemples d’ús ideal**

### �� Crear un apunt
> “Crea l’apunt `vector_clocks.md` seguint el llibre d’estil del repositori.”

### 🔸 Millorar una carpeta
> “Millora tot el contingut de `notes/01_comunicacio/` segons el llibre d’estil.”

### 🔸 Generar codi
> “Construeix-me un exemple de simulació de Lamport clocks per posar a `codes/lamport/` seguint el llibre d’estil.”

### 🔸 Reestructurar
> “Revisa l’estructura del repositori i proposa reordenar carpetes mantenint el llibre d’estil.”

### 🔸 Documentar TSAE
> “Genera un apunt complet de TSAE fase 2, seguint el llibre d’estil.”

---

# 📌 Proper pas
Quan vulguis, digues:

**“Crea’m la primera nota segons el llibre d’estil”**

i començarem amb el primer apunt del wiki.

