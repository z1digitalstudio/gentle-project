[‹ Discovery Phase](/ai-playbook/guides/discovery/README.md)
# Skill: scope-definition

## Propósito

Convertir el roadmap priorizado en PRD y user stories accionables para diseño y desarrollo.

## Cuándo usarla

- cuando `management/ROADMAP.md` ya es usable
- cuando el MVP ya tiene recorte suficiente
- cuando hace falta bajar el alcance a requisitos claros

## Inputs típicos

- `management/ROADMAP.md`
- `product/RESEARCH.md`
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md`

## Outputs

### Canónicos
- `product/PRD.md`
- `product/USER-STORIES.md`

### Opcionales
- `product/artifacts/MVP-Scope-Notes.md`
- `product/artifacts/Open-Product-Questions.md`

## Qué debe dejar resuelto

- MVP claramente acotado
- `non-goals` visibles
- historias accionables
- dudas abiertas importantes sin esconder

## Ejemplo de estructura del PRD

Un `product/PRD.md` válido tiene al menos estas secciones:

```
# PRD: [Nombre del producto o feature]

## Objetivo
Qué problema resuelve y para quién.

## Scope del MVP
Qué funcionalidades entran en la primera versión.

## Non-goals
Qué queda explícitamente fuera del alcance.

## Flujos principales
Los flujos de usuario más importantes que el MVP debe soportar.

## Constraints
Limitaciones técnicas, de negocio o de tiempo conocidas.

## Señales de éxito
Cómo se va a saber que el MVP funcionó.

## Preguntas abiertas
Dudas que siguen sin respuesta pero no bloquean el avance.
```

No hace falta que todas las secciones estén completas al 100%. Lo importante es que existan y que las respuestas sean honestas sobre lo que se sabe y lo que no.

## Qué viene después

Después de esta skill, Discovery puede dar paso a:
- diseño
- especificación
- desarrollo
