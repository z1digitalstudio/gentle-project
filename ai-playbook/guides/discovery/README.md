[‹ AI Playbook](/ai-playbook/README.md)
# Discovery Phase

> Esta guía explica cómo recorrer Discovery de punta a punta en este template: qué subfases existen, qué skills las soportan, qué artefactos produce cada una y cuándo se considera cerrada la fase.

## Para quién es esta guía

Esta guía es para los humanos del equipo: Product Managers, Product Designers y Developers. Está pensada para quienes corren o participan del proceso de discovery, y necesitan entender cómo moverse por las subfases, cuándo usar cada skill y qué documentos se esperan como resultado.

---

## Objetivo de la fase

Discovery no existe para generar documentos por rutina.

Su objetivo es dejar una base suficientemente clara para:
- entender el problema y la oportunidad
- distinguir evidencia de supuestos
- priorizar MVP vs. later
- bajar el alcance a PRD y user stories
- pasar a diseño, especificación o desarrollo con menos ambigüedad

---

## Estructura de la fase

| # | Subfase | Objetivo | Documentación |
|---|---|---|---|
| 1 | **Onboarding & Kickoff** | Llegar al kickoff con framing suficiente y salir con contexto operativo capturado | [Ver doc](/ai-playbook/guides/discovery/phase-docs/onboarding-kickoff-subphase.md) |
| 2 | **Design Research** | Convertir contexto usable en evidencia, señales e insights diferenciados | [Ver doc](/ai-playbook/guides/discovery/phase-docs/design-research-subphase.md) |
| 3 | **Roadmap Definition** | Traducir research en prioridades, MVP y secuencia de producto | [Ver doc](/ai-playbook/guides/discovery/phase-docs/roadmap-definition-subphase.md) |
| 4 | **Scope Definition** | Bajar el roadmap a PRD y user stories accionables para diseño y desarrollo | [Ver doc](/ai-playbook/guides/discovery/phase-docs/scope-definition-subphase.md) |

---

## Skills core de la fase

| Subfase | Skill | Rol | Documentación |
| --- | --- | --- | --- |
| Onboarding & Kickoff | `discovery-onboarding` | Normaliza framing disperso antes del kickoff | [Ver doc](/ai-playbook/guides/discovery/skills-docs/discovery-onboarding.md) |
| Onboarding & Kickoff | `kickoff-prep` | Convierte framing usable en agenda, preguntas, riesgos y decisiones esperadas | [Ver doc](/ai-playbook/guides/discovery/skills-docs/kickoff-prep.md) |
| Onboarding & Kickoff | `kickoff-closeout` | Convierte evidencia del kickoff en memoria operativa del proyecto | [Ver doc](/ai-playbook/guides/discovery/skills-docs/kickoff-closeout.md) |
| Design Research | `design-research` | Convierte contexto usable en research, insights y oportunidades | [Ver doc](/ai-playbook/guides/discovery/skills-docs/design-research.md) |
| Roadmap Definition | `roadmap-definition` | Traduce research en prioridades, MVP y secuencia | [Ver doc](/ai-playbook/guides/discovery/skills-docs/roadmap-definition.md) |
| Scope Definition | `scope-definition` | Baja roadmap a PRD y user stories accionables | [Ver doc](/ai-playbook/guides/discovery/skills-docs/scope-definition.md) |

---

## Artefactos canónicos de la fase

Estos son los documentos vivos que el template debería poder sostener durante Discovery:

| Artefacto | Descripción |
| --- | --- |
| `docs/PROJECT-SUMMARY.md` | Resumen vivo del proyecto: problema, oportunidad, estado actual, decisiones clave, riesgos y próximo paso recomendado. |
| `management/RISKS.md` | Registro de riesgos del proyecto con evidencia actual, impacto, probabilidad, mitigación, owner y siguiente revisión. |
| `management/ROADMAP.md` | Roadmap canónico con narrativa de prioridades, tabla estructurada de features y visualización Mermaid de MVP / later / secuencia. |
| `management/DECISIONS.md` | Registro de decisiones relevantes de producto y alcance para no perder criterio entre sesiones o cambios de contexto. |
| `product/RESEARCH.md` | Síntesis canónica de research con inputs, señales de usuario, pains, contexto competitivo, evidencia vs supuestos y oportunidades. |
| `product/PRD.md` | Definición funcional del producto y del MVP: objetivo, scope, non-goals, flujos principales, constraints y señales de éxito. |
| `product/USER-STORIES.md` | Historias priorizadas y agrupadas por feature/epic con suficiente claridad para diseño y desarrollo. |

Artefactos de trabajo frecuentes:

| Artefacto | Skill que lo genera | Tipo |
| --- | --- | --- |
| `product/artifacts/Opportunity-Brief.md` | `discovery-onboarding` | condicional |
| `product/artifacts/Kick-off-Meeting-Prep.md` | `kickoff-prep` | principal |
| `product/artifacts/Kickoff-Closeout-Summary.md` | `kickoff-closeout` | opcional |
| `product/artifacts/Discovery-Insights.md` | `design-research` | opcional |
| `product/artifacts/Personas.md` | `design-research` | opcional |
| `product/artifacts/User-Journeys.md` | `design-research` | opcional |
| `product/artifacts/Feature-Prioritization.md` | `roadmap-definition` | opcional |
| `product/artifacts/MVP-Cuts.md` | `roadmap-definition` | opcional |
| `product/artifacts/MVP-Scope-Notes.md` | `scope-definition` | opcional |
| `product/artifacts/Open-Product-Questions.md` | `scope-definition` | opcional |

---

## Criterio de cierre de la fase

Discovery se considera suficientemente cerrada cuando:

- existe contexto inicial alineado y útil
- hay research con evidencia, señales y supuestos diferenciados
- el roadmap distingue MVP, later y secuencia
- existen `product/PRD.md` y `product/USER-STORIES.md`
- diseño y desarrollo pueden empezar con bastante menos ambigüedad

Discovery no termina cuando “hay muchos docs”.
Termina cuando el proyecto ganó claridad operativa real.
