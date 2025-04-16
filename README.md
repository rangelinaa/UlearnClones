# UlearnClones

## Диаграмма классов
![Диаграмма классов](https://www.mermaidchart.com/raw/377341e9-6cda-43c5-85d1-7ad16198d036?theme=light&version=v0.1&format=svg)

---

## Описание классов

### Класс `ImmutableStack<T>`
- **Основные методы**:
  - `Push` - возвращает новый стек с добавленным элементом
  - `Pop` - возвращает стек без верхнего элемента
  - `Peek` - читает верхний элемент без изменений

### Класс `Clone`
- **LearnedPrograms**: стек изученных программ (ImmutableStack<string>)
- **RollbackHistory**: стек отменённых программ (ImmutableStack<string>)
- **Copy()**: создаёт "поверхностную" копию (без дублирования стеков)

### Класс `CloneVersionSystem`
  - `learn`: создает новый стек программ + сбрасывает историю
  - `rollback`/`relearn`: переиспользует неизменяемые стеки
  - `clone`: мгновенное копирование (только ссылок)
