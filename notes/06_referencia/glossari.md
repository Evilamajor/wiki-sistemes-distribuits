# Glossari de Sistemes Distribuïts

Referència ràpida de termes utilitzats als apunts. Els conceptes inclouen definicions breus i, quan escau, bones pràctiques o fórmules útils.

## Conceptes bàsics
- **Latença**: temps que triga un missatge a recórrer el camí complet entre emissor i receptor.
- **Amplada de banda**: quantitat de dades que es poden transmetre per unitat de temps.
- **Throughput**: volum de treball completat per unitat de temps; pot diferir de l'amplada de banda quan hi ha cues o bloquejos.
- **Disponibilitat**: probabilitat que un sistema respongui correctament en un interval donat (p. ex. "tres 9": 99,9%).
- **Tolerància a fallades**: capacitat de mantenir el servei tot i la presència de fallades parcials.

## Comunicació i sincronització
- **Rellotge lògic de Lamport**: comptador incrementat per cada esdeveniment local i en rebre un missatge; ordena causalment però no dona simultaneïtat real.
- **Rellotge vectorial**: llista de comptadors (un per procés) que permet determinar relacions de causa-efecte i detectar concurrència.
- **Acoblament temporal/espacial**: en acoblament temporal cal que els processos siguin actius simultàniament; en acoblament espacial cal conèixer l'adreça exacta del receptor.
- **FIFO**: garantia que els missatges entre dos processos arriben en l'ordre d'enviament.

## Consistència i replicació
- **Consistència forta**: totes les rèpliques observen el mateix ordre d'operacions (p. ex. serialització completa o linealitzabilitat).
- **Consistència eventual**: en absència de noves actualitzacions, les rèpliques convergeixen; pot haver-hi lectures estantisses temporalment.
- **Quòrum**: tècnica per assegurar intersecció entre lectures i escriptures; per a N rèpliques, sovint s'usa R + W > N.
- **Idempotència**: propietat d'una operació que pot repetir-se sense canviar el resultat (útil per reenviaments i reintents).

## Coordinació i tolerància a fallades
- **Leader election**: mecanisme per escollir un procés coordinador (p. ex. Bully, Raft).
- **Heartbeats**: missatges periòdics per comprovar vivacitat i detectar fallades ràpidament.
- **Partició de xarxa**: situació en què el sistema queda dividit en subconjunts incomunicats; obliga a escollir entre disponibilitat i consistència (CAP).
- **Split-brain**: cas en què dos subconjunts es creuen líders simultanis; cal prevenció (quòrum, fencing) per evitar conflictes.

## Emmagatzematge i dades
- **Shard**: fragment de dades distribuït entre nodes per escalar capacitat i throughput.
- **Replica primària-secundària**: model on un node central gestiona escriptures i els secundaris repliquen per a lectures o failover.
- **Event sourcing**: emmagatzematge de canvis com a seqüència d'esdeveniments immutables; l'estat es reconstrueix reproduint-los.
- **Log append-only**: estructura on només s'afegeixen registres al final; facilita replicació seqüencial i recuperació.

## Fiabilitat i observabilitat
- **MTTF/MTTR**: Mean Time To Failure / Mean Time To Repair; mesuren fiabilitat i velocitat de recuperació.
- **Backoff exponencial**: estratègia de reintents augmentant el temps d'espera per reduir congestió.
- **Circuit breaker**: patró que atura temporalment crides a un servei quan es detecten fallades repetides.
- **Tracing distribuït**: seguiment d'una petició a través de múltiples serveis amb identificadors de correlació (p. ex. `trace_id`, `span_id`).
