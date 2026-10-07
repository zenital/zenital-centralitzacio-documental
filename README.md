# zenital-centralitzacio-documental

Repositori inicial per preparar el desenvolupament del servei d'ingesta i la integració amb Marino.

## Estat

Context i proposta funcional preparats. Encara no hi ha aplicació, stack escollit, esquema SQL aprovat ni desplegament.

## Context local

La carpeta `info/` està exclosa de Git. Cal copiar-la al directori arrel de cada clon abans de treballar amb el context complet. No es recupera amb `git clone` ni amb `git pull`.

Llegiu `info/00-index.md` i `info/01-context-projecte.md`. La guia per a Claude Code és `CLAUDE.md`. `CLAUDE.local.md`, també ignorat, carrega l'índex local de context.

El PDF original és a `info/fonts/Centralizacion-Documentos.pdf`.

## Primera sessió de desenvolupament

Obriu Claude Code des de l'arrel i feu servir el prompt de `info/03-inici-desenvolupament.md`. El primer resultat és un disseny tècnic basat en els requisits, amb les hipòtesis pendents identificades.

Les comandes de build, execució i tests es documentaran quan s'hagi definit la implementació.

## Separació de continguts

- Git: codi futur, configuració sense secrets, proves i documentació tècnica que s'acordi versionar.
- `info/`: context del client, fonts originals, decisions i propostes funcionals.
- `docs/`: ubicació futura per a decisions tècniques aprovades i documentació de l'aplicació.

No forceu la inclusió de `info/` amb `git add -f`.
