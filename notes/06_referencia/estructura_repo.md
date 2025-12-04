# Estructura del repositori “wiki-sistemes-distribuits”

Aquest document descriu l’estructura global del repositori, la funció de cada carpeta i les millors pràctiques per mantenir-lo organitzat i fàcil de navegar.

---

## 📁 Carpetes principals

### `notes/`
Conté tots els apunts teòrics en format Markdown organitzats per mòduls.  
Els subdirectoris segueixen l’ordre del curs i dels temes estudiats:

- `00_introduccio/` – definició i propietats bàsiques dels sistemes distribuïts.  
- `01_comunicacio/` – models de comunicació, sincronia/asincronia, middleware, acoblament.  
- `02_consistencia/` – consistència forta, eventual, rellotges de Lamport i vectorials.  
- `03_TSAE/` – fases del protocol TSAE, logs, vector clocks, purga de missatges, experiències.  
- `04_models/` – arquitectures i models de sistemes distribuïts (Chord, Spanner, hashing consistent...).  
- `05_aplicacions/` – plataformes com Kafka, RabbitMQ, DynamoDB i Cassandra.  
- `06_referencia/` – documents d’ús intern: glossari, llibre d’estil, estructura del repo, ordres git, etc.

---

### `codes/`
Inclou codi font de simuladors i exemples:

- Rellotges de Lamport  
- Vector clocks  
- Protocol TSAE (fases 1–4)  
- Experiments, scripts i utilitats d’estudi  

Cada subcarpeta hauria de tenir un `README.md` curt explicant l’objectiu del codi.

---

### `results/`
Resultats d’execució del codi i experiments:

- logs  
- sortides de programes  
- comparatives  
- anotacions dels experiments estudiats  

---

## 📐 Bones pràctiques de nomenclatura (naming)

- Fitxers Markdown → minúscules + guions baixos  
  Exemple: `consistencia_eventual.md`  
- Carpetes → `NN_tema/` on NN és ordre seqüencial  
  Exemple: `02_consistencia/`
- Fitxers de referència → dins `06_referencia/`

---

## 🔄 Manteniment de l’índex

Quan s’afegeixi un nou apunt:

1. Crear el fitxer dins la carpeta adequada  
2. Afegir-lo a `notes/README.md`  
3. Actualitzar aquest document si s’afegeix una nova carpeta o tema  

---

## 🧩 Filosofia d’organització

Aquest repositori funciona com un “wiki de sistemes distribuïts” amb objectius:

- Estudi personal aprofundit  
- Base de coneixement reutilitzable  
- Suport directe per al TFG  
- Exercici de documentació tècnica i estructura professional

Es recomana mantenir-lo modular, ordenat, i fàcil d’ampliar.

