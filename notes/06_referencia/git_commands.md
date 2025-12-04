# Ordres Git bàsiques

Recull ràpid d'ordres Git per al flux de treball habitual amb aquest repositori.

## Configuració i estat
- `git status -sb`: estat curt de la branca actual.
- `git branch -vv`: llista de branques i referència remota.
- `git config --list --show-origin`: comprova configuració i valors per fitxer.

## Flux de treball diari
- `git pull --ff-only`: actualitza la branca local evitant merges implícits.
- `git add <fitxers>`: prepara els canvis per al commit.
- `git commit -m "Resum curt"`: crea un commit amb un missatge breu i descriptiu.
- `git push`: publica els commits a l'origen.

## Exploració de canvis
- `git diff`: mostra els canvis no indexats.
- `git diff --staged`: mostra els canvis que aniran al proper commit.
- `git log --oneline --graph --decorate -n 15`: historial compacte de les últimes revisions.

## Treball amb branques
- `git switch <branca>`: canvia de branca.
- `git switch -c <nova-branca>`: crea i canvia a una branca nova.
- `git merge <branca>`: fusiona una branca a l'actual (assegura't d'estar al dia abans de fusionar).

## Desfer i netejar
- `git restore <fitxers>`: descarta canvis locals no indexats.
- `git restore --staged <fitxers>`: treu fitxers de l'índex mantenint els canvis al directori de treball.
- `git checkout <commit> -- <fitxer>`: recupera la versió d'un fitxer a partir d'un commit antic.
- `git revert <commit>`: crea un commit que desfà els canvis d'un altre commit.
- `git clean -fd`: esborra fitxers no seguits (vigila abans d'executar-ho).

## Estalviar canvis temporals
- `git stash push -m "context"`: guarda canvis no commitats temporalment.
- `git stash list`: mostra les entrades guardades.
- `git stash pop`: recupera i elimina l'entrada més recent.

Mantén aquesta referència actualitzada si afegeixes noves pràctiques o eines al flux de treball.
