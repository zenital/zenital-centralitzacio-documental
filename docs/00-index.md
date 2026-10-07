# Índex de context per al desenvolupament

Actualització: 8 d'octubre de 2026. Tot el context explicatiu és versionat i arriba amb un clon.

## Ordre de lectura

1. [Context funcional consolidat](01-context-projecte.md): objectiu, abast, acords, arquitectura, fases, model lògic i funcionament diari.
2. [Decisions i dependències](02-decisions-i-pendents.md): què falta confirmar per implementar integracions.
3. [Primera sessió de desenvolupament](03-inici-desenvolupament.md): prompt inicial, resultat esperat i comprovacions.

## Base de treball

- Marino és el sistema operatiu final.
- Bústia corporativa central amb reenviaments de transició.
- Ingesta inicial sense interfície pròpia.
- Correus i adjunts fora de SQL; metadades, estats i referències a SQL des de la primera ingesta.
- Consulta auxiliar des de Marino prevista; mecanisme d'actualització pendent de prova.
- Primera fita proposada: fases 1 a 4, amb compleció i conciliació documental manuals, sense dependència d'IA.
- Fases 5 a 7: extracció amb IA, validació humana i generació ERP.
- Stack, motor SQL, infraestructura, proveïdors, calendari i pressupost pendents.
- Els estats, pantalles i criteris d'acceptació funcionals encara són propostes per validar amb Flower.

## Context i documents reals

`docs/` conté context, instruccions, decisions i pla de treball. `info/` només conté documents reals locals, ignorats per Git; no conté context explicatiu. No cal la carpeta `info/` per començar el disseny ni per treballar amb dades sintètiques.

El plantejament i les observacions del PDF original estan resumits al context consolidat. La font original opcional és `info/documents/Centralizacion-Documentos.pdf`. Les mostres reals es comparteixen per separat només quan una prova les necessita.

## Fonts i manteniment

`docs/01-context-projecte.md` és la referència versionada per al desenvolupament. La [Page de revisió](https://chatgpt.com/space/page_3db37fd6c35c8191904f5ffa5e6a842d) no és un requisit d'accés i no es sincronitza automàticament. Els acords nous es reflecteixen en els dos suports.

El PDF del client aporta el procés original; les propostes funcionals i d'arquitectura són elaboració posterior. Manteniu aquesta distinció quan es prenguin decisions.
