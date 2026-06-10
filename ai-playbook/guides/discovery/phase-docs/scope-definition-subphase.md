[‹ AI Playbook](/ai-playbook/README.md)
[‹ Discovery Phase](/ai-playbook/guides/discovery/README.md)

# Subphase #4 — Scope Definition

## Objetivo

Convertir el roadmap priorizado en requisitos accionables para diseño y desarrollo.

Esta subfase cierra Discovery. Su trabajo es hacer visible:
- qué entra realmente en MVP
- qué no entra
- qué flujos importan más
- qué dudas siguen abiertas aunque el proyecto ya pueda avanzar

---

## Skill principal

- `scope-definition`

---

## Inputs típicos

### Mínimo
- `management/ROADMAP.md`

### Recomendados
- `product/RESEARCH.md`
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md`
- notas de negocio o validaciones adicionales

---

## Outputs y artefactos

### Canónicos
- `product/PRD.md`
- `product/USER-STORIES.md`

### Opcionales
- `product/artifacts/MVP-Scope-Notes.md`
- `product/artifacts/Open-Product-Questions.md`

### Actualizaciones posibles
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md`

---

## Qué debería dejar resuelto

- MVP definido con claridad suficiente
- `non-goals` explícitos
- flujos principales visibles
- historias accionables para diseño y desarrollo
- dudas abiertas importantes sin esconderse

---

## Criterio de cierre de la subfase

Scope Definition está cerrada cuando:
- `product/PRD.md` existe y contiene las secciones: Contexto, Problema, Objetivo, Alcance MVP, Non-goals y Criterios de éxito
- `product/USER-STORIES.md` existe y tiene al menos una historia por flujo principal, cada una con el formato "Como [rol], quiero [acción], para [objetivo]"
- los `non-goals` están listados explícitamente en el PRD —no ausentes por silencio
- cada historia de usuario tiene criterios de aceptación definidos, o una nota que indica que se definirán en la fase de diseño
- las dudas abiertas críticas están registradas en `product/artifacts/Open-Product-Questions.md` o en una sección dedicada del PRD —ninguna ambigüedad queda escondida
- `management/DECISIONS.md` refleja las decisiones de alcance tomadas durante esta subfase
- diseño y desarrollo pueden iniciar sin necesidad de revisar los outputs de Discovery para entender qué construir
