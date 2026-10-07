# Primera sessió de desenvolupament amb Claude

## Preparació

Cloneu el repositori privat, entreu a l'arrel i llegiu README.md i CLAUDE.md. Tot el context és a `docs/`; no cal copiar documents reals ni tenir accés a la Page.

Encara no hi ha dependències d'aplicació, comandes de build o una aplicació per executar. Comproveu que disposeu de Claude Code instal·lat i autenticat si aquesta és l'eina que fareu servir.

## Prompt inicial

Llegeix CLAUDE.md, docs/00-index.md, docs/01-context-projecte.md i docs/02-decisions-i-pendents.md.

Prepara el disseny tècnic de la primera entrega de Flower fins a la fase 4. Distingueix els acords de les propostes pendents. No necessites documents reals per a aquesta tasca. Abans d'escriure codi:

1. Resumeix el resultat funcional i les dependències.
2. Proposa components i responsabilitats per a correu, ingesta, arxiu, SQL i Marino.
3. Descriu el model lògic i el contracte d'escriptura sense inventar el motor SQL ni l'esquema intern de Marino.
4. Defineix recuperació d'errors parcials, reintents, correus repetits, fitxers repetits i possibles revisions.
5. Separa els camps automàtics dels que completa una persona.
6. Proposa un backlog ordenat amb criteris d'acceptació i identifica les tasques bloquejades per decisions, dades o accessos.
7. Indica què cal confirmar abans d'escollir stack i construir adaptadors reals.

La conciliació documental no acredita cobrament bancari ni aprovació de càrrecs. Les fases 5 a 7 són evolució posterior. Utilitza dades sintètiques quan necessitis exemples.

Escriu la proposta tècnica en anglès a docs/technical-design.md i el backlog a docs/development-backlog.md, identificant-los com a propostes. Aquests fitxers encara no existeixen. Mantén els acords funcionals en català.

## Resultat esperat i continuació

El primer resultat és un disseny revisable i un pla d'implementació, no una connexió amb producció. No presentis els documents proposats com una arquitectura aprovada.

Després de resoldre les decisions que condicionin el disseny, la primera construcció pot cobrir ingesta, conservació, registre i reintents, amb adaptadors simulats on falti accés real. El stack es decideix explícitament.

## Comprovació de la primera sessió

- [ ] Claude ha llegit el context versionat sense dependre de fitxers ignorats.
- [ ] Les hipòtesis sobre Marino, correu, SQL i arxiu estan identificades.
- [ ] El backlog distingeix treball executable de tasques bloquejades.
- [ ] Hi ha criteris per duplicats, errors parcials i traçabilitat.
- [ ] Cap document real ni credencial s'ha incorporat a Git.
- [ ] Les propostes tècniques es guarden a docs/ i mantenen el seu estat de proposta.
