# Decisions i dependències per al desenvolupament

Aquest fitxer orienta la lectura de les taules d'acords i pendents de [la base consolidada](01-context-projecte.md).

## Abans de connectar sistemes reals

| Dependència | Evidència necessària |
| --- | --- |
| Correu | Plataforma, bústia central, mecanisme d'accés, permisos i conservació de l'original durant reenviaments. |
| Repositori de fitxers | Ubicació, permisos, referències estables i prova d'obertura des de Marino. |
| SQL | Motor i versió, entorn de prova, esquema auxiliar i permisos disponibles. |
| Marino | Responsable tècnic i demostració de consulta i actualització d'un registre auxiliar amb accés al document. |
| Dades del pilot | Correus i adjunts dels tres tipus, repetits, revisions i avisos amb línies pendents. |
| Operació | Qui completa dades, qui concilia i qui resol errors tècnics. |

Les mostres reals són opcionals per al disseny inicial i es conserven només a `info/`, fora de Git. Les conclusions que se'n derivin es documenten a `docs/`.

## Abans de tancar la fase 4

Cal confirmar camps obligatoris, introducció manual de línies d'avís, normalització de referències per client, signes, imports parcials, toleràncies i autoritat de tancament i reobertura. Els estats i pantalles del context funcional són propostes.

## Repartiment d'escriptura a definir

Proposta: la ingesta escriu origen, arxiu i estat tècnic; Marino gestiona dades de negoci, responsables i relacions. Cal definir qui pot modificar cada camp i com es resolen actualitzacions incompatibles.

## Treball que pot avançar

Es poden dissenyar interfícies per a correu, arxiu i registre, contractes lògics de dades, recuperació d'errors i consulta documental. Es poden planificar o implementar proves amb dades sintètiques un cop escollit el stack.

Les simulacions no validen els permisos ni el funcionament dels sistemes reals. Les decisions i el backlog es versionen a `docs/`; no van a `info/`.
