# UlearnClones

## Диаграмма классов
![Диаграмма классов](https://www.mermaidchart.com/app/projects/6ccb976d-2170-4695-80ad-c7016a1a6312/diagrams/87e96f4c-6ec9-41c1-a2bb-79fd15f9415b/version/v0.1/edit)

---

## Описание классов

### Clone
Клон с двумя стеками:
- `LearnedPrograms` — стек изученных программ.
- `RollbackHistory` — стек откатов.
- `Copy()` — создаёт копию клона.

### CloneVersionSystem
Система управления клонами:
- `clones` — хранит всех клонов.
- `nextCloneId` — номер следующего клона.
- `Execute(query)` — выполняет команды (`learn`, rollback, relearn, clone, `check`).
