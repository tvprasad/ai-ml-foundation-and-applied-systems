# ADR-001: AI vs ML and When to Use ML

**Date:** 2026-02-21
**Status:** Accepted

## Context

When approaching a problem, it is important to distinguish between Artificial Intelligence (AI) as a broad field and Machine Learning (ML) as a specific subset. Not every problem requires ML — traditional rule-based or algorithmic approaches are often simpler, more interpretable, and more maintainable. A clear decision framework helps guide when ML is the right tool.

## Decision

### AI vs ML

| | AI | ML |
|---|---|---|
| **Scope** | Broad field encompassing any technique that enables machines to simulate human intelligence | Subset of AI where systems learn patterns from data without being explicitly programmed |
| **Approach** | Rule-based systems, search, planning, expert systems, ML, deep learning | Statistical models trained on data |
| **Examples** | Chess engines, expert systems, robotics | Image classification, recommendation systems, NLP models |

### When to Use ML

Use ML when:
- The rules are too complex or numerous to hand-code (e.g., spam detection, image recognition)
- The problem involves patterns in large datasets that are not obvious to humans
- The system needs to adapt or improve over time with new data
- Traditional algorithms produce insufficient accuracy or scalability

Do **not** use ML when:
- A simple rule-based or algorithmic solution works well
- The dataset is too small to generalize from
- Interpretability and auditability are critical and cannot be traded off
- The cost of data collection, labeling, and model maintenance outweighs the benefit

## Consequences

- Establishes a shared vocabulary distinguishing AI from ML within this project
- Provides a reusable decision heuristic before committing to ML-based solutions
- Encourages starting simple and escalating to ML only when justified
