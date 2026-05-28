[‹ AI Playbook](/ai-playbook/README.md)
[‹ Discovery Phase](/ai-playbook/guides/discovery/README.md)

# Subphase #3 — Roadmap Definition

## Objetivo

Traducir research a prioridades de producto, recorte de MVP y secuencia inicial de trabajo.

Esta subfase no existe solo para listar features. Debe hacer visible:
- qué entra en MVP
- qué queda para later
- qué está fuera de alcance por ahora
- qué lógica sostiene esa priorización

---

## Skill principal

- `roadmap-definition`

---

## Inputs típicos

### Mínimo
- `product/RESEARCH.md`

### Recomendados
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- cierre de kickoff
- constraints comerciales o técnicos
- feature wishlist existente
- inputs de stakeholders

---

## Outputs y artefactos

### Canónicos
- `management/ROADMAP.md`
- actualización de `docs/PROJECT-SUMMARY.md`
- actualización de `management/RISKS.md`

### Muy recomendado
- `management/DECISIONS.md`

### Opcionales
- `product/artifacts/Feature-Prioritization.md`
- `product/artifacts/MVP-Cuts.md`

---

## Requisito importante del roadmap

`management/ROADMAP.md` debería combinar:

1. narrativa de prioridades y secuencia
2. tabla estructurada de features
3. visualización `Mermaid`

El objetivo no es solo registrar features, sino hacer comprensible el razonamiento del recorte.

---

## Criterio de cierre de la subfase

Roadmap Definition está cerrada cuando:
- existe `management/ROADMAP.md`
- el roadmap combina texto + estructura + Mermaid
- el MVP está diferenciado de `later`
- la lógica de priorización es visible
- los riesgos de secuencia o dependencias están visibles
- `scope-definition` puede empezar a bajar alcance a PRD y user stories
