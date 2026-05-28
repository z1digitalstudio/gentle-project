[‹ AI Playbook](/ai-playbook/README.md)
[‹ Discovery Phase](/ai-playbook/guides/discovery/README.md)

# Subphase #1 — Onboarding & Kickoff

## Objetivo

Llegar al kickoff con framing suficiente y salir de él con contexto operativo mejorado.

Esta subfase no se mide por cuántos documentos genera, sino por si el equipo logra:
- entender mejor el encargo
- exponer riesgos y huecos importantes
- preparar una conversación útil
- aterrizar lo aprendido en memoria canónica del proyecto

---

## Secuencias válidas

### Flujo completo
1. `discovery-onboarding`
2. `kickoff-prep`
3. `kickoff-closeout`

### Flujo abreviado
1. `kickoff-prep`
2. `kickoff-closeout`

### Flujo tardío
1. `kickoff-closeout`

---

## Inputs típicos

- sales notes
- proposal / deck comercial
- emails o resúmenes
- transcript o rough notes
- links a producto o prototipo
- `Opportunity Brief` externo
- `Vision & Collaboration Goals` externo `opcional`

---

## Outputs y artefactos

### Artefactos de trabajo
- `product/artifacts/Opportunity-Brief.md` `condicional`
- `product/artifacts/Kick-off-Meeting-Prep.md` `estable`
- `product/artifacts/Kickoff-Closeout-Summary.md` `opcional`

### Documentos canónicos que se actualizan
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/ROADMAP.md` `solo si el kickoff justifica una nota preliminar`

---

## Regla de entrada

### Si el kickoff ya ocurrió
- usar `kickoff-closeout` si hay evidencia usable
- o pasar a `design-research` si el contexto ya quedó suficientemente claro

### Si el kickoff no ocurrió
- si el framing ya es usable → `kickoff-prep`
- si el framing todavía es débil o disperso → `discovery-onboarding`

---

## Qué hace cada skill

### `discovery-onboarding`
Normaliza contexto disperso y deja framing usable.
No debería forzar un `Opportunity Brief` si ya existe framing suficiente.

### `kickoff-prep`
Convierte framing usable en agenda, preguntas estratégicas, riesgos y decisiones esperadas.

### `kickoff-closeout`
Convierte notas, transcript o decisiones del kickoff en memoria operativa confiable.

---

## Criterio de cierre de la subfase

Onboarding & Kickoff está cerrada cuando:
- hubo framing suficiente para preparar el kickoff
- el kickoff tuvo agenda y preguntas claras
- las decisiones, incertidumbres y riesgos fueron capturados
- `docs/PROJECT-SUMMARY.md` y `management/RISKS.md` reflejan mejor el proyecto real
- `design-research` puede empezar sin depender de contexto oral disperso
