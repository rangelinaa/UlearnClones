# UlearnClones

## Диаграмма классов
![Диаграмма классов]([https://www.mermaidchart.com/raw/87e96f4c-6ec9-41c1-a2bb-79fd15f9415b?theme=light&version=v0.1&format=svg](https://www.mermaidchart.com/raw/377341e9-6cda-43c5-85d1-7ad16198d036?theme=light&version=v0.1&format=svg))

---

## Описание классов

### Класс Clone 
Представляет отдельного клона с историей его обучения и откатов:

- LearnedPrograms (Stack<string>) - стек изученных программ (последняя изученная наверху)
- RollbackHistory (Stack<string>) - стек отменённых программ (последняя отменённая наверху)
- Copy() - создаёт глубокую копию клона, включая копии обоих стеков

### Класс CloneVersionSystem
Система управления всеми клонами:

- clones - словарь всех клонов (ключ - ID клона)
- nextCloneId - счётчик для генерации новых ID клонов
- Execute(query) - обрабатывает команды:
  - learn ci pi - обучение клона
  - rollback ci - откат последней программы
  - relearn ci - повторное применение отката
  - clone ci - создание нового клона
  - check ci - проверка последней изученной программы
