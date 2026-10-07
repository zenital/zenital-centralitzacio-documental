# zenital-centralitzacio-documental

Servei d'ingesta i gestió documental per a Flower, amb Marino com a sistema operatiu final.

## Estat i inici

El repositori inclou el context per començar el disseny tècnic i planificar la primera entrega fins a la fase 4. Encara no hi ha aplicació executable, stack escollit, esquema SQL aprovat ni integracions validades.

```bash
git clone https://github.com/zenital/zenital-centralitzacio-documental.git
cd zenital-centralitzacio-documental
```

Llegiu [l'índex](docs/00-index.md), [la definició funcional](docs/01-context-projecte.md), [les dependències](docs/02-decisions-i-pendents.md) i [la primera tasca](docs/03-inici-desenvolupament.md).

Amb Claude Code instal·lat i autenticat, inicieu-lo des de l'arrel i utilitzeu el prompt de la primera tasca. `CLAUDE.md` orienta la lectura del context versionat. No cal cap fitxer de `info/` per a aquesta sessió.

No hi ha encara comandes de build, execució o tests de l'aplicació. Es documentaran amb la primera implementació.

## On va cada contingut

| Ubicació | Contingut | Versionat |
| --- | --- | --- |
| docs/ | Context, requisits, acords, propostes, decisions, pla de treball i documentació tècnica. | Sí |
| CLAUDE.md | Instruccions compartides de desenvolupament. | Sí |
| info/ | Exclusivament documents reals locals: factures, notes, avisos, correus i adjunts originals. | No |
| .env i .env.* | Configuració i credencials locals; una futura .env.example només contindrà valors de mostra. | No |

Un clon ja inclou tot el context explicatiu. `info/` no es crea amb Git i no és obligatòria per començar el disseny. Quan calguin mostres reals, creeu `info/documents/` i copieu-hi els fitxers autoritzats. No hi poseu notes, decisions, especificacions ni instruccions: van a `docs/`.

El PDF original `Centralizacion Documentos.pdf` conté el plantejament i exemples reals; la informació necessària ja està resumida a `docs/01-context-projecte.md`. La còpia original es conserva localment a `info/documents/Centralizacion-Documentos.pdf`.

Les dades sintètiques de prova podran versionar-se amb els tests. No pugeu documents reals ni forceu la inclusió de `info/` amb `git add -f`.

## Continuïtat

`docs/` és la referència versionada per al desenvolupament. La [Page del projecte](https://chatgpt.com/space/page_3db37fd6c35c8191904f5ffa5e6a842d) és un suport de revisió i no cal tenir-hi accés per començar. Els canvis acordats s'han de reflectir en els dos suports; no hi ha sincronització automàtica.

La primera tasca és proposar el disseny tècnic i el backlog. Les connexions reals depenen de les dades i accessos de correu, repositori, SQL i Marino detallats a la documentació.
