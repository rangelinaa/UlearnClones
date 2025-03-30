# UlearnClones

## Диаграмма классов
![Диаграмма классов](https://www.mermaidchart.com/raw/87e96f4c-6ec9-41c1-a2bb-79fd15f9415b?theme=light&version=v0.1&format=svg)

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
