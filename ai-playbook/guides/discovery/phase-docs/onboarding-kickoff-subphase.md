[‹ AI Playbook](/ai-playbook/README.md)
[‹ Discovery Phase](/ai-playbook/guides/discovery/README.md)

# Subphase #1 — Onboarding & Kickoff

## Objetivo

Llegar al kickoff con framing suficiente y salir de él con contexto operativo mejorado.

Esta subfase no se mide por cuántos documentos genera, sino por si el equipo logra:
- Entender mejor el encargo
- Exponer riesgos y huecos importantes
- Preparar una conversación útil
- Aterrizar lo aprendido en memoria canónica del proyecto

---

## Cómo elegir el flujo

### ¿El kickoff ya ocurrió?

- **Sí, y hay evidencia usable** (notas, transcript, decisiones) → usar flujo tardío
- **Sí, y el contexto ya quedó claro** → pasar directo a `design-research`

### ¿El kickoff todavía no ocurrió?

| Situación | Flujo |
|---|---|
| Hay un Opportunity Brief claro y vigente | Flujo abreviado |
| Hay un brief pero está desactualizado, incompleto o contradictorio | Flujo completo |
| No hay brief — contexto disperso en notas, mails, decks | Flujo completo |

---

## Secuencias válidas

### Flujo completo
**Cuándo:** el contexto está disperso y el kickoff todavía no ocurrió.

1. `discovery-onboarding` — consolida notas, mails y decks en framing usable
2. `kickoff-prep` — convierte ese framing en agenda y preguntas estratégicas
3. `kickoff-closeout` — captura lo aprendido en memoria canónica

### Flujo abreviado
**Cuándo:** ya existe un Opportunity Brief claro y vigente, pero el kickoff todavía no ocurrió.

1. `kickoff-prep` — el framing ya está, se prepara la reunión directamente
2. `kickoff-closeout` — captura decisiones y próximos pasos

### Flujo tardío
**Cuándo:** el kickoff ya ocurrió y hay evidencia usable (notas, transcript, decisiones).

1. `kickoff-closeout` — procesa lo que quedó registrado y lo convierte en contexto operativo

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

## Qué debería dejar resuelto

- framing del proyecto entendido por todo el equipo
- riesgos e incógnitas iniciales explicitados
- contexto suficiente para que `design-research` arranque sin depender de conversaciones orales
- decisiones del kickoff capturadas y separadas de las preguntas aún abiertas

---

## Criterio de cierre de la subfase

Onboarding & Kickoff está cerrada cuando:
- `product/artifacts/Kick-off-Meeting-Prep.md` existe y contiene: agenda, al menos 5 preguntas estratégicas priorizadas, riesgos a validar y decisiones esperadas durante la reunión
- `docs/PROJECT-SUMMARY.md` existe y tiene las secciones: Contexto, Problema, Objetivo, Stakeholders, y al menos un campo de Próximo paso recomendado
- `management/RISKS.md` existe y tiene al menos un riesgo identificado con descripción, impacto estimado y mitigación posible
- las decisiones tomadas en el kickoff están capturadas explícitamente (en `Kickoff-Closeout-Summary.md` o directamente en `PROJECT-SUMMARY.md`), separadas de las preguntas aún abiertas
- `design-research` puede iniciarse sin necesidad de recuperar contexto de conversaciones orales o documentos dispersos
