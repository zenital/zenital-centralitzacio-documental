# Instruccions del projecte

## Context abans de desenvolupar

- Llegeix explícitament `info/00-index.md` i `info/01-context-projecte.md` abans de proposar arquitectura o canviar comportament funcional.
- Llegeix `info/02-decisions-i-pendents.md` per comprovar les dependències i `info/03-inici-desenvolupament.md` per a la primera tasca.
- `info/` és local i està ignorat per Git. Accedeix als fitxers pel camí exacte; no assumeixis que una cerca del repositori els inclou.
- Si falta el context local, indica quins fitxers falten i demana que es copiïn abans de decidir comportament de negoci.
- Distingueix requisits del client, acords, propostes i hipòtesis. No presentis una proposta com un acord.

## Desenvolupament

- El sistema operatiu final és Marino. Respecta els límits de la primera entrega descrits al context.
- No escullis un motor SQL, infraestructura, servei de correu o proveïdor d'IA com si ja estiguessin confirmats.
- Abans d'implementar una tasca, indica el requisit que cobreix, dependències i criteri d'acceptació.
- Amb dependències externes no disponibles, es poden proposar adaptadors i utilitzar dades sintètiques; no afirmis que la integració real està validada.
- Conserva originals, traçabilitat i recuperació de processaments segons l'especificació.
- Incorpora tests de comportament rellevants per ingesta repetida, errors parcials, relacions documentals i correccions quan aquestes funcions s'implementin.
- Documenta com executar i validar el codi quan hi hagi una implementació.

## Documentació i Git

- Context funcional i decisions de negoci en català.
- Mantén `info/`, documents reals i secrets fora dels commits. No facis `git add -f` d'aquests fitxers.
- Per registrar una nova decisió, separa-la de les propostes i afegeix data i justificació; no canviïs silenciosament els acords.
- Evita duplicar la mateixa especificació en diversos fitxers: `info/01-context-projecte.md` és la base funcional consolidada.
