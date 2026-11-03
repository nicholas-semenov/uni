---
type: revision-practice
module: IC101 - Finance
lecture: "[[IC101 L01 — Introductory Securities & Markets]]"
seminar: "[[IC101 S01 — Finance basics, three pillars, time value of money]]"
created: 2026-11-01
---

# IC101 S01 — Practice

**Putting a price on time and risk**

[[IC101 — Revision Checklist|Revision checklist]] · [[IC101 L01 — Cheat Sheet|Cheat sheet]] · [[IC101 S01 — Slides.pdf|Original seminar slides]]

> [!info] Как работаем
> Решай по порядку, сначала без слайдов и cheat sheet. Калькулятор можно. Записывай ход расчётов и короткое объяснение смысла ответа. Отмечай задание после решения и проверки; ответы находятся в сворачиваемых блоках в конце заметки.
>
> Условия и числа взяты из Seminar 1, страницы PDF 5–10 и 12. Разобранные примеры превращены в самостоятельные задания; вопросы на объяснение добавлены для проверки понимания. Нумерация 1–8 — для этой заметки. Условия оставлены на английском; объяснение можно сначала написать по-русски.

## 1. Compounding — future value

Источник: [[IC101 S01 — Slides.pdf#page=5|Slide 5 — worked example]].

**Put £100 in an account paying 5% a year. What is it worth in 3 years?**

Assume annual compounding. Show your calculation and explain what compounding means.

**My working and answer:**

115.76

- [x] Решено самостоятельно и проверено.

## 2. Discounting — present value

Источник: [[IC101 S01 — Slides.pdf#page=6|Slide 6 — worked example]].

**What is £1,000 received in 3 years worth today, at an annual discount rate of 8%?**

Show your calculation and briefly explain why the present value differs from the future amount.

**My working and answer:**

793.8322
- [x] Решено самостоятельно и проверено.

## 3. Discounting — your turn

Источник: [[IC101 S01 — Slides.pdf#page=6|Slide 6 — Your turn]].

**What is £500 received in 2 years worth today at an annual discount rate of 10%?**

Show your calculation. Optional: try the slide's two-minute practice limit after you understand the method.

**My working and answer:**


413,22
- [x] Решено самостоятельно и проверено.

## 4. NPV — accept or reject?

Источник: [[IC101 S01 — Slides.pdf#page=7|Slide 7 — NPV]].

**A project costs £1,000 now and pays £600 at the end of year 1 and £600 at the end of year 2. The annual discount rate is 10%. Should the project be accepted?**

1. Calculate the present value of each future payment.
2. Calculate the total present value of the future payments.
3. Calculate NPV.
4. State your decision and explain what the NPV means under these assumptions.

| Time | Cash flow | Present value |
|---|---:|---|
| Now | −£1,000 | |
| End of year 1 | +£600 | |
| End of year 2 | +£600 | |

**My working, NPV and decision:**

So our DCF: 1041.32 
NPV: 1041.32 - 1000(initiual investment) = 41.32(so my decision invest )

- [x] Решено самостоятельно и проверено.

## 5. Bond valuation — two market yields

Источник: [[IC101 S01 — Slides.pdf#page=8|Slide 8 — price a bond]].

**A bond pays a £5 coupon at the end of each year for 3 years and returns its £100 face value at the end of year 3. What is it worth today?**

1. Calculate its price at a **5% annual market yield**.
2. Recalculate its price at a **7% annual market yield**. Use the same payments and the same three-year period.
3. Explain the price difference. Does the £5 coupon change?

**My cash-flow timeline and calculations:**



**My explanation:**

100 - PV by **5% annual market yield**
94.75 - PV by **7% annual market yield**

была сложноть именно с 3 вот отчет от чата - 1. Что такое market yield — откуда берётся эта ставка и кто её определяет.
    
2. Почему цена облигации падает — если рынок требует 7%, а купон остаётся £5.
    
3. Что значит выгодная цена — ты думала, что покупать облигацию дешевле £100 всегда выгоднее.
    
4. Откуда берётся доходность 7% — если облигация ежегодно платит только £5.
    

Главный пробел: ты путала фиксированный купон (£5) с доходностью инвестора (market yield). Ты не сразу поняла, что доходность может увеличиться без изменения купона — за счёт снижения цены покупки облигации.


- [ ] Решено самостоятельно и проверено.

## 6. Expected return

Источник: [[IC101 S01 — Slides.pdf#page=9|Slide 9 — risk and return]].

**A share has a 50% chance of returning +20% and a 50% chance of returning −10%.**

1. Calculate its expected return.
2. Is the expected return guaranteed?
3. Which realised returns are possible in this example?
4. Explain why a risk-averse investor may require a risk premium.

**My calculation and explanation:**

1)expected return = 0.05(почему то сразу побежал в cheat sheet хотя сам я понмиаю как это делаеться)
2)never
3)we can't say
4)because if investor take a risk, he want to get more money for this


- [ ] Решено самостоятельно и проверено.

## 7. Where would the money go?

Источник: [[IC101 S01 — Slides.pdf#page=10|Slide 10 — group discussion]]. Для revision запиши собственный ответ на групповое задание.

**Your group has £10,000 to invest for 10 years. Agree how to split it across a savings account, bonds, a global shares fund, and crypto.**

Explain your allocation using:

- **Time:** what could inflation do to cash over 10 years?
- **Risk and return:** which investments would you expect to offer higher returns, and why?
- **Diversification:** why would you spread the money, or why would you choose not to?
- **Expected outcome:** roughly what return are you hoping for? State your assumptions.
- **Main risk:** what is the single biggest risk in your proposed allocation?

There is no single correct allocation. Defend your choice using the lecture's concepts.

| Investment         | Amount      | Share of portfolio | Reason                                  |
| ------------------ | ----------- | ------------------ | --------------------------------------- |
| Savings account    | 1 000       | 10%                | liquidity                               |
| Bonds              | 2000        | 20%                | basically more staible                  |
| Global shares fund | 5 000       | 50%                | more staible and can bring good return  |
| Crypto             | 2 000       | 20%                | take a risk for higher return           |
| **Total**          | **£10,000** | **100%**           |                                         |

**My explanation and assumptions:**
1)Infulation over 10 yearh make cahs worth less then today
2) crypto os risk one but can bring higher returns because this speculative assests
 3)diversfication help to spread your money betwen a lot of different investments to bring your risk on low level 
 4)higher then infulation and hopifly then interest rate
 

- [ ] Решено самостоятельно и проверено.

## 8. Exam-style MCQ

Источник: [[IC101 S01 — Slides.pdf#page=12|Slide 12 — exam-style question]].

**At a discount rate of 10%, which is worth the MOST today?**

- **A)** £100 received today.
- **B)** £110 received in one year.
- **C)** £121 received in two years.
- **D)** They are all worth the same today.

Choose one answer and show the present-value calculations that support it.

**My answer and explanation:**
D - они все одинаковве если сичтаь их PV


- [x] Решено самостоятельно и проверено.

---

## Проверка ответов — 1 ноября 2026

**Числовые результаты верные. Главная доработка — объяснения в заданиях 5–7.** Исходные ответы сохранены. Орфография английского не снижает оценку понимания.

| Задание | Результат проверки | Что дополнить |
|---|---|---|
| **1. FV** | £115.76 — верно | Запиши $100(1.05)^3$ и поясни, что проценты начисляются также на ранее начисленные проценты. |
| **2. PV £1,000** | £793.8322 — верно; итог £793.83 | Запиши $1000/(1.08)^3$. Объясни discounting через opportunity cost, не только inflation. |
| **3. PV £500** | £413.22 — верно | Для полной записи достаточно добавить $500/(1.10)^2$. Десятичная запятая допустима. |
| **4. NPV** | PV £1,041.32, NPV +£41.32, accept — верно | Заполни PV по годам: £545.45 и £495.87; PV первоначального расхода сегодня −£1,000. Решение означает ожидаемое создание стоимости сверх required return 10%, не гарантированную прибыль. |
| **5. Bond** | Обе цены верны: £100.00 при 5% и £94.75 при 7% | Вставленный отчёт другого чата описывает трудности, но не заменяет твоего объяснения. Нужен свой ответ о yield, цене, фиксированном coupon и principal. |
| **6. Expected return** | 0.05 = 5% — верно; расчёт выполнен с подсказкой. «Не гарантирован» — верно | Ответ «we can’t say» неполон: возможны **+20% или −10%**, неизвестно заранее, какой из двух исходов реализуется. Risk premium — дополнительная ожидаемая/требуемая компенсация за риск. |
| **7. Allocation** | Суммы и доли сходятся: £10,000 и 100%. Liquidity, inflation и diversification учтены | Нужен один явно названный главный риск; уточни смысл stable и отдели желаемую доходность от прогнозируемой/гарантированной. Само распределение не имеет единственного правильного ответа. |
| **8. MCQ** | **D — верно**, объяснение через одинаковые PV верное | Для полной записи покажи £100, $110/1.10=100$ и $121/(1.10)^2=100$. |

### Что исправить перед тестом

**5 — Coupon, market yield и цена покупки.** Coupon остаётся **£5**. При более высокой требуемой market yield те же будущие платежи имеют меньшую present value, поэтому цена падает. Для покупки за £94.75 yield to maturity связан со всеми платежами **£5, £5, £105**, включая возврат £100 principal; это не просто $5/94.75$. Более низкая цена сама по себе не гарантирует выгодность или фактический результат: нужно учитывать риск и альтернативы. Кратко объясни это своими словами, а не копируй ключ.

**6 — Возможные исходы и среднее ожидание.** В условии заданы только два возможных realised returns: **+20% и −10%**. **5%** — их probability-weighted average. Мы не знаем, какой исход случится, но знаем список возможных исходов. «Хочу больше денег за риск» уточни как **higher expected return**, а не обещанную выплату. Повторный расчёт нужно сделать без cheat sheet; правильный ответ с подсказкой отдельно не подтверждает самостоятельность.

**7 — Обоснование, не изменение долей.**

- Global shares fund обычно диверсифицирован по компаниям, но может заметно упасть вместе с рынком. Уточни, с чем сравниваешь его стабильность.
- Риски bonds зависят от issuer, maturity и других условий; не все облигации одинаково стабильны.
- Фраза «crypto может принести более высокую доходность» допустима. Добавь, что возможны и крупные убытки; высокая volatility сама по себе не доказывает высокую ожидаемую доходность.
- «Выше inflation и interest rate» — цель. Для приблизительного численного ожидания нужны обозначенные предположения о доходности частей портфеля; данные для расчёта в семинаре не даны, поэтому произвольный процент не требуется.
- Назови **один главный риск** и обоснуй его. Например, рыночный спад для 50% в equities или крупный убыток в 20% crypto; выбор причины должен быть твоим.

### Мои исправления после проверки

**5. Why does the bond price fall when the market yield rises, even though the £5 coupon stays fixed? How can buying below face value contribute to the yield to maturity?**



**6. Show the expected-return calculation without the cheat sheet. Which realised returns are possible, and which outcome is unknown in advance?**



**7. What is the single biggest risk in your allocation, and why? Clarify what you mean by a global shares fund being “stable”.**



**Статус:** задания 1–4 и 8 проверены; в 1–4 и 8 полезно дописать ход расчётов. Задания 5–7 пока открыты для уточнения и проверки без подсказок. Семинар проверен; перечисленные доработки ещё открыты. После этих исправлений переходи к [[IC101 L01 — Test|HTML-тесту]].

---

## Проверка решений

Открывай соответствующий блок после своей попытки. Если ответ совпал, проверь также метод и объяснение. В задании 7 вместо единственного ответа — критерии проверки.

> [!success]- 1. Future value
> $$FV=100(1.05)^3=\boxed{£115.76}$$
> Year 1: £105.00; year 2: £110.25; year 3: £115.7625 before rounding.
>
> Compounding means earning interest on the original amount and on previously earned interest. Округляй окончательный денежный ответ до двух знаков.

> [!success]- 2. Present value of £1,000
> $$PV=\frac{1000}{(1.08)^3}=\boxed{£793.83}$$
> The discount rate represents the relevant opportunity cost of capital. At a positive discount rate, the future amount has a lower present value.

> [!success]- 3. Present value of £500
> $$PV=\frac{500}{(1.10)^2}=\boxed{£413.22}$$
> The cash flow arrives in two years, so the denominator must include two periods.

> [!success]- 4. NPV and decision
> $$PV_1=\frac{600}{1.10}=£545.45$$
> $$PV_2=\frac{600}{(1.10)^2}=£495.87$$
> $$PV(\text{future payments})\approx £1,041.32$$
> $$NPV=-1000+\frac{600}{1.10}+\frac{600}{(1.10)^2}=\boxed{+£41.32}$$
> **Accept under the stated assumptions:** the project is expected to create £41.32 of value today above the 10% required return. Это не гарантия фактического результата.

> [!success]- 5. Bond prices
> The payments are £5 at the end of year 1, £5 at the end of year 2, and £105 at the end of year 3.
>
> At 5%:
> $$P=\frac{5}{1.05}+\frac{5}{(1.05)^2}+\frac{105}{(1.05)^3}=\boxed{£100.00}$$
> At 7%:
> $$P=\frac{5}{1.07}+\frac{5}{(1.07)^2}+\frac{105}{(1.07)^3}\approx\boxed{£94.75}$$
> **Примечание к исходнику:** на слайде указано £94.76. Если сохранять точность промежуточных вычислений и округлять только итог, получается £94.75. Разница в одну пенни не меняет метод или вывод.
>
> A higher market yield reduces the present value of the same payments. **The fixed £5 coupon does not change.** Face value is repaid only at maturity and is discounted too.

> [!success]- 6. Expected return
> $$E(R)=0.5(20\%)+0.5(-10\%)=\boxed{5\%}$$
> The realised return in the stated example is either **+20% or −10%**. The expected return is not guaranteed and is not itself one of these two possible outcomes.
>
> A risk-averse investor prefers less risk for the same expected return and generally requires compensation for accepting additional risk. Это ожидаемая компенсация, не обещание более высокой фактической доходности.

> [!success]- 7. Criteria for the allocation
> There is no single correct answer. Check that:
> - Your amounts total **£10,000**, and portfolio shares total **100%**.
> - Your explanation uses the **10-year horizon**, inflation, risk and diversification.
> - You distinguish expected returns from guaranteed outcomes.
> - You state assumptions behind your hoped-for return; the seminar does not provide asset-return forecasts.
> - You identify one clear main risk and explain why it matters.
>
> Это учебное обсуждение; текущие рыночные прогнозы для его выполнения не требуются.

> [!success]- 8. MCQ answer
> **D — they are all worth the same today.**
> $$PV_A=£100$$
> $$PV_B=\frac{110}{1.10}=£100$$
> $$PV_C=\frac{121}{(1.10)^2}=£100$$
> Comparing the nominal amounts alone would ignore their different dates.

## Финальная самопроверка

По [[IC101 S01 — Slides.pdf#page=11|слайду 11]]:

- Верно ли посчитал количество периодов до каждого cash flow?
- Дисконтировал ли каждый будущий платёж перед сложением?
- Различаю ли expected и realised return?

**Ошибки, которые нужно перерешать:**

- №5: объяснить coupon / market yield / price и роль возврата principal.
- №6: назвать возможные realised returns и самостоятельно восстановить weighted-average calculation.
- №7: назвать главный риск портфеля и уточнить stable / expected return.

Когда закончим, отметим этап «Практика» в [[IC101 — Revision Checklist]]. Создание этой заметки само по себе не означает, что задания уже выполнены.

**Следующий шаг после семинара:** [[IC101 L01 — Test|Topic 1 + вопросы по пробелам — HTML-тест]].
