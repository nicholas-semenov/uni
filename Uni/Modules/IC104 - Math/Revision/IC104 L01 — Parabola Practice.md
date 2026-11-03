---
type: revision-practice
module: IC104 - Math
lecture: "[[IC104 L01 — Introduction to Algebra]]"
topic: Quadratic vertex, maximum and minimum
assigned: 2026-11-03
status: reviewed-applications-open
reviewed: 2026-11-03
---

# IC104 L01 — Parabola Practice

[[IC104 — Revision Checklist|Checklist]] · [[IC104 — Tutor Log|Контекст]] · [[IC104 — Topics for Practice|Темы для банка]]

**Цель:** находить вершину параболы, отличать maximum от minimum и понимать разницу между точкой достижения экстремума и значением функции. Производные для этого набора не нужны.

**Начни с 1–3.** Если получаются — переходи к 4–6; 7–8 — применение в экономике, по результату и доступности. Не обязательно выполнять весь набор за один блок. Готовых ответов к упражнениям здесь нет.

## Короткая опора — открой, если забыл метод

> [!tip]- Vertex, maximum and minimum
> Для квадратичной функции $f(x)=ax^2+bx+c$, $a\ne0$:
>
> - $a>0$: парабола открыта вверх → **minimum**.
> - $a<0$: парабола открыта вниз → **maximum**.
> - Абсцисса вершины: $x_*=-\frac{b}{2a}$.
> - Ордината вершины: $y_*=f(x_*)$. Подставь найденное $x_*$ в исходную функцию.
> - Вершина — **точка** $(x_*,y_*)$. Значение maximum/minimum — это **$y_*$**, а достигается оно **at $x=x_*$**.
> - Axis of symmetry: $x=x_*$.
> - Для формы $f(x)=a(x-h)^2+k$: вершина $(h,k)$.
> - Roots отвечают на другой вопрос: где $f(x)=0$. Дискриминант для поиска вершины по формуле выше не требуется.
>
> **Форма ответа:** “The function has a minimum/maximum at $x=\ldots$. The minimum/maximum value is $\ldots$. The vertex is $(\ldots,\ldots)$.”
>
> Если использовал эту опору, отметь это рядом с решением. Затем проверим понимание другой задачей без подсказки.

Теория: [[IC104 L01 — Slides.pdf#page=45|L01, страница PDF 45 / напечатанный слайд 47]]. Короткая опора составлена тьютором по теме лекции.

## A. Core practice — авторские задания 1–6

**For Questions 1–4:** identify $a$, $b$ and $c$; state whether the function has a maximum or a minimum; find the vertex and the extreme value. Show your substitutions and calculations.

### 1. Positive leading coefficient

$$
f(x)=x^2-6x+5.
$$

**My working:**


**Answer (max/min; vertex; extreme value):**
min because a >1
(3; -4)
-4


**Used the reference box?**


### 2. Negative leading coefficient

$$
f(x)=-x^2+8x-7.
$$

**My working:**


**Answer (max/min; vertex; extreme value):**
max a = -1
(4, 9)
9

**Used the reference box?**
x

### 3. Non-unit leading coefficient
()
$$
f(x)=2x^2+4x+1.
$$

**My working:**


**Answer (max/min; vertex; extreme value):**
min a = 2
(-1, -1)
-1 

**Used the reference box?**


### 4. Fractional vertex coordinate

$$
f(x)=-2x^2-6x+5.
$$

**My working:**


**Answer (max/min; vertex; extreme value):**


**Used the reference box?**


### 5. Vertex form

$$
g(x)=3(x+2)^2-4.
$$

**Without expanding the brackets, find the vertex, the axis of symmetry and the minimum value. Explain how you read the vertex from the formula.**

**My working and explanation:**


**Answer:**


**Used the reference box?**


### 6. A vertex is not a root

$$
h(x)=x^2-4x+7.
$$

**Find the vertex and the minimum value. Does the equation $h(x)=0$ have any real solutions? Explain using the minimum value.**

**My working and explanation:**


**Answer:**


**Used the reference box?**


## B. Applications — задания из учебных материалов

> [!warning] Разобрать: задания 7 и 8
> 3 ноября пользователь сообщил, что не понимает именно раздел B. **№7 (пункты 1–5) и №8 (пункты 1–4) оставлены для разбора и банка задач.** Ответов на них пока нет; какая конкретно стадия вызывает трудность, отдельно ещё не установлено.
> Навыки: revenue $R(Q)=P(Q)Q$ → profit $\pi(Q)=R(Q)-C(Q)$ → квадратная функция → оптимальный выпуск через вершину → максимальная прибыль и проверка ограничений.

### 7. Lecture L01 — profit maximisation

**Источник:** [[IC104 L01 — Slides.pdf#page=46|страница PDF 46 / напечатанный слайд 48]]. Условие переформулировано по-английски, исходные функции сохранены. На слайде приведено решение — не открывай его до своей попытки; это практика по примеру лекции, не новый unseen exam question.

A firm sells $Q$ units at the price per unit

$$
P(Q)=102-2Q.
$$

Its total cost is

$$
C(Q)=2Q+\frac12Q^2.
$$

**Tasks:**

1. Write the total revenue $R(Q)$.
2. Write and simplify the profit function $\pi(Q)=R(Q)-C(Q)$.
3. Use the vertex formula to find the production level that maximises profit.
4. Calculate the maximum profit.
5. Explain why your result is a maximum, and check that your chosen output and price are non-negative.

**My working:**


**Answer (optimal Q and maximum profit):**


**Used reference box / original solution?**


### 8. Problem Set 3 — adapted method

**Источник:** [[IC104 L05 — Problem Set 03.pdf#page=1|Problem Set 3, страница PDF 1, textbook page 280, Question 4(i)]]. В исходном семинарском задании предлагается метод производных. **Здесь сохранены исходные функции, но инструкция адаптирована для L01:** реши через вершину квадратичной функции. Дополнительные пункты на profit value и проверку — тьюторские.

A firm's total revenue and total cost are

$$
R(Q)=1840Q,\qquad C(Q)=2Q^2+40Q+5000,\qquad Q\geq0.
$$

**Tasks:**

1. Write and simplify $\pi(Q)=R(Q)-C(Q)$.
2. Find the production level that maximises profit, using the vertex formula.
3. Calculate the maximum profit.
4. Explain why this is a maximum.

**My working:**


**Answer (optimal Q and maximum profit):**


**Used the reference box?**


## Progress

Галочка — своя попытка записана; оценка и использование подсказки учитываются отдельно.

- [x] 1
- [x] 2
- [x] 3
- [ ] 4
- [ ] 5
- [ ] 6
- [ ] 7 — **Разобрать все пункты 1–5: lecture profit maximisation**
- [ ] 8 — **Разобрать все пункты 1–4: Problem Set 3 Q4(i), adapted method**

## Tutor review — 3 November 2026

| Задания | Результат / статус |
|---|---|
| 1 | Minimum, vertex $(3,-4)$, minimum value $-4$ — верно. **Причину исправить:** minimum при $a>0$, а не $a>1$. В этой задаче $a=1$ |
| 2 | Maximum, vertex $(4,9)$, maximum value $9$ — верно. В поле про reference box стоит `x`; использование подсказки однозначно не установлено |
| 3 | Minimum, vertex $(-1,-1)$, minimum value $-1$ — верно. Исправлен заголовок упражнения: $b=4>0$, прежнее “Negative b” было ошибкой тьютора |
| 4–6 | Пользователь сообщил, что понимает, как решать часть A. Письменных ответов нет, поэтому эти задания не отмечены решёнными/проверенными; это не ошибки |
| **7 — B** | **Нужно разобрать, пункты 1–5.** Ответа пока нет; включено в список для банка |
| **8 — B** | **Нужно разобрать, пункты 1–4.** Ответа пока нет; включено в список для банка |

**Итог:** все три записанные вершины и экстремальные значения верны; базовый расчёт показан правильными результатами. Одна содержательная поправка — условие minimum $a>0$. Шаги вычислений почти не записаны; их отдельно не оценивали. Не считать весь раздел A независимо проверенным по самоотчёту.

**Основная доработка:** применение параболы к максимизации прибыли, **B №7 и №8**. При разборе сначала выяснить, где возникает затруднение: перевод условия, составление revenue/profit, раскрытие скобок, выбор $a,b,c$ или интерпретация оптимума. Пока не приписывать конкретную причину без попытки.

**Для банка:** [[IC104 — Topics for Practice|темы и номера задач]].

**My corrections after feedback:**


**Следующий шаг:** разобрать B №7 по этапам, затем самостоятельно применить метод к B №8 или новому аналогичному примеру. Exp/log остаётся отдельной открытой темой. Отложенный recall ещё не выполнен.
