---
type: dashboard
---

# Dashboard

**[[Тьютор — Прогресс и следующий шаг|Тьютор: мой прогресс, что повторить и следующий шаг]]**

Модули: [[IC101 - Finance]] · [[IC102]] · [[IC103 - Economics]] · [[IC104 - Math]] · [[IC105]] · [[MM1F27]]

Справка: [[Дедлайны]] · [[Цели — Семестр 1]] · [[Модули программы]] · [[Общая информация]] · [[Правила университета]]

Подготовка: [[Reading Week — 2–8 ноября 2026|План на reading week]] · [[Экзамены — Семестр 1|Формат экзаменов и даты]]

Revision: [[Revision Pipeline|Порядок работы]] · [[IC101 — Revision Checklist|IC101]] · [[IC102 — Revision Checklist|IC102]] · [[IC103 — Revision Checklist|IC103]] · [[IC104 — Revision Checklist|IC104]] · [[IC105 — Revision Checklist|IC105]] · [[MM1F27 — Revision Checklist|MM1F27]]

## Лекции

```base
filters:
  and:
    - file.inFolder("Uni/Modules")
    - type == "lecture"
properties:
  file.name:
    displayName: Лекция
  note.module:
    displayName: Модуль
  note.number:
    displayName: Номер
  note.date:
    displayName: Дата
  note.understood:
    displayName: Понял
views:
  - type: table
    name: Все лекции
    groupBy:
      property: module
      direction: ASC
    order:
      - file.name
      - number
      - date
      - understood
    sort:
      - property: number
        direction: ASC
    columnSize:
      file.name: 423
      note.number: 30
      note.date: 119

```

## 🧮 Семинары

```base
filters:
  and:
    - file.inFolder("Uni/Modules")
    - type == "seminar"
formulas:
  progress: if(tutorial, 1, 0) + if(mcq_why, 1, 0) + if(vocab_review, 1, 0) + if(practice, 1, 0) + if(questions, 1, 0) + if(redo_errors, 1, 0) + if(anki_errors, 1, 0)
properties:
  file.name:
    displayName: Семинар
  note.module:
    displayName: Модуль
  note.date:
    displayName: Дата
  note.tutorial:
    displayName: Туториал
  note.mcq_why:
    displayName: MCQ почему
  note.vocab_review:
    displayName: Vocab
  note.practice:
    displayName: Доп. задачи
  note.questions:
    displayName: Вопросы
  note.redo_errors:
    displayName: Ошибки перерешал
  note.anki_errors:
    displayName: Anki ошибки
  formula.progress:
    displayName: Готово /7
views:
  - type: table
    name: 🔥 Не доделано
    filters:
      and:
        - formula.progress < 7
    order:
      - file.name
      - module
      - date
      - tutorial
      - mcq_why
      - vocab_review
      - practice
      - questions
      - redo_errors
      - anki_errors
      - formula.progress
    sort:
      - property: date
        direction: DESC
  - type: table
    name: Все семинары
    groupBy:
      property: module
      direction: ASC
    order:
      - file.name
      - date
      - tutorial
      - mcq_why
      - vocab_review
      - practice
      - questions
      - redo_errors
      - anki_errors
      - formula.progress
    sort:
      - property: date
        direction: ASC

```
