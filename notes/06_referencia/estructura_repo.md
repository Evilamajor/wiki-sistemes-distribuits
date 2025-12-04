# Estructura del repositori

Guia ràpida de la disposició de carpetes i fitxers per mantenir els apunts organitzats.

## Carpeta arrel
- `README.md`: resum del projecte i enllaç a les carpetes principals.
- `.git/`: metadades de git (no s'edita manualment).

## notes/
Apunts i resums del curs. Cada mòdul disposa de la seva carpeta amb fitxers Markdown.
- `notes/README.md`: índex amb enllaços a cada mòdul i recomanacions per afegir nous apunts.
- `notes/0X_*`: carpetes numerades per mòdul (introducció, comunicació, consistència, etc.).

## codes/
Exemples de codi, simuladors i snippets relacionats amb els continguts del curs.
- `codes/README.md`: descriu què s'hi pot trobar (Lamport, rellotges vectorials, TSAE...).
- Subcarpetes opcionals per agrupar experiments o llibreries específiques.

## results/
Sortides, logs i resultats generats quan s'executen els experiments o simulacions.
- `results/README.md`: explica l'objectiu de la carpeta i què s'hi hauria de guardar.

## Bones pràctiques
- Usa noms de fitxer en minúscules i amb guions baixos per facilitar la lectura.
- Mantén els índexs (`README.md`) actualitzats quan s'afegeixin nous materials.
- Col·loca el codi i els resultats a les carpetes corresponents per mantenir la separació entre teoria i experiments.
