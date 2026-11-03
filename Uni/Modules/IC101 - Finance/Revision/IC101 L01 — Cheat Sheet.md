---
type: cheat-sheet
module: IC101 - Finance
lecture: "[[IC101 L01 — Introductory Securities & Markets]]"
created: 2026-10-31
---

# IC101 L01 — Cheat Sheet

[[IC101 L01 — Introductory Securities & Markets|Лекция]] · [[IC101 L01 — Study Guide|Study Guide]] · [[IC101 — Revision Checklist|Revision checklist]]

> [!abstract] The big picture
> Finance moves resources between people and across time, while managing risk. Its three pillars are **time value of money, risk management and asset pricing**.

## What is finance?

**Finance allocates money from savers to borrowers and helps people move resources across time, while managing risk.**

![[IC101 L01 — Finance Flow.png]]

**Across time** — между настоящим и будущим:

- **Borrowing:** use money today and repay from future income.
- **Saving:** set aside money today to spend in the future.
- **Life cycle:** borrow when young → save during working life → use savings in retirement. Это типичная модель, а не правило для каждого человека.

**Prices act as signals that help allocate scarce resources.**

| Participant | Role | Example |
|---|---|---|
| **Buy side** | Invest funds, including funds managed for others | Pension funds, asset managers |
| **Sell side** | Facilitate issuance, distribution and trading | Investment banks, brokers |
| **Issuers** | Raise funding by issuing securities | Companies, governments |

## Three pillars of finance

| Pillar | Main idea | Question |
|---|---|---|
| **1. Time value of money** | Money today can earn a return; timing matters | When will I receive the money? |
| **2. Risk management** | Returns are uncertain, so risk must be measured and managed | How uncertain are the cash flows? |
| **3. Asset pricing** | Combine time and risk to estimate asset values | What are those cash flows worth today? |

**Estimated value is the present value of expected future cash flows, discounted at a rate that reflects time and risk.**

Это принцип DCF-оценки активов с ожидаемыми cash flows. Полученная оценка может отличаться от фактической **market price**.

## Time value of money

**Money today is generally worth more than the same amount in the future because it can earn a return.**

Инфляция влияет на покупательную способность. Даже без инфляции существует **opportunity cost**: деньги сегодня можно вложить в подходящую альтернативу.

| Concept | Meaning | Direction |
|---|---|---|
| **PV — Present Value** | The value today of a future amount | Future → today: **discounting** |
| **FV — Future Value** | The amount an investment grows to in the future | Today → future: **compounding** |

$$
\boxed{FV=PV(1+i)^n}
$$

$$
\boxed{PV=\frac{FV}{(1+i)^n}}
$$

- $i$ = interest or discount rate **per period**, expressed as a decimal.
- $n$ = **number of periods**.
- Ставка и количество периодов должны соответствовать друг другу: например, annual rate и число лет.

> [!example] Forward and backward
> At 5% per year, £100 today grows to £105 in one year:
> $$FV=100(1.05)=£105$$
> Conversely, £105 received in one year has a present value of £100:
> $$PV=\frac{105}{1.05}=£100$$

**Nominal return** — доходность без корректировки на инфляцию. **Real return** — после корректировки: положительная nominal return может не покрыть рост цен.

## Risk and return

| Term                | Meaning                                                                     |
| ------------------- | --------------------------------------------------------------------------- |
| **Expected return** | The anticipated return; a probability-weighted average of possible outcomes |
| **Realised return** | The actual return over a period                                             |
| **Risk aversion**   | Preferring less risk for the same expected return                           |
| **Risk premium**    | The additional expected return required for bearing risk                    |


> [!warning] Exam distinction
> **Higher risk does not guarantee a higher realised return.** Investors require compensation for taking risk, but actual outcomes can include losses.

### Three ways to tame risk

| Method              | How it works                                                            | Example                                   |
| ------------------- | ----------------------------------------------------------------------- | ----------------------------------------- |
| **Diversification** | Spread investments across different assets to reduce concentration risk | Invest across companies and sectors       |
| **Hedging**         | Take an offsetting position to reduce a specific exposure               | An airline hedges fuel costs with futures |
| **Insurance**       | Transfer a specified risk in exchange for a premium                     | Insure business property against fire     |

Diversification **does not eliminate all risk**. A farmer can hedge against falling wheat prices by **selling futures** or **buying a put option**. A futures contract creates obligations; an option gives its holder a right.

> [!example]- Seminar extension — expected return
> $$E(R)=\sum_i p_iR_i$$
> A 50% chance of +20% and a 50% chance of −10% gives:
> $$E(R)=0.5(20\%)+0.5(-10\%)=5\%$$
> The expected return is 5%, but the stated possible outcomes are +20% and −10%.

## What are we pricing?

| Category | Main idea | Examples |
|---|---|---|
| **Capital assets** | Financial claims with expected cash flows | Shares, bonds, loans |
| **Derivatives** | Value or payoff depends on an underlying asset, rate or index | Options, futures, swaps |
| **Real assets** | Physical assets with economic use | Property, commodities |
| **Purely speculative assets** | Value mainly depends on future resale demand | Some crypto, art |

**Property = недвижимость.** Это учебная классификация: категории могут пересекаться. Высокая volatility сама по себе не определяет speculative asset. DCF напрямую применим там, где можно оценить cash flows; не каждый актив создаёт такие потоки.

## DCF — Discounted Cash Flow

**DCF is a valuation method used to estimate an asset’s value today by discounting its expected future cash flows at a rate that reflects time and risk.**

$$
\boxed{V_0=\sum_{t=1}^{N}\frac{CF_t}{(1+r)^t}}
$$

$$
V_0=\frac{CF_1}{1+r}+\frac{CF_2}{(1+r)^2}+\cdots+\frac{CF_N}{(1+r)^N}
$$

| Symbol | Meaning |
|---|---|
| $V_0$ | Estimated value today |
| $CF_t$ | Expected cash flow in period $t$ |
| $r$ | Discount rate per period |
| $t$ | Period in which the cash flow occurs |
| $N$ | Number of periods |
| $\sum$ | Add up the discounted cash flows |

**Сначала дисконтируем каждый cash flow на его срок, затем складываем present values.** Для тех же положительных cash flows более высокая discount rate означает меньшую оценку сегодня.

### Discount rate vs interest rate

> [!important] Required ≠ guaranteed
> **The discount rate is the return investors require, not necessarily the return they will receive.**

В упрощённой модели:

$$
\boxed{r=r_f+\text{Risk premium}}
$$

- **Risk-free rate** $r_f$ — доходность условно безрисковой альтернативы.
- **Risk premium** — дополнительная доходность, которую инвесторы требуют за риск проекта.
- Например: $4\%+3\%=7\%$. Это required return, используемая в знаменателе DCF.

**Interest rate** — ставка, установленная условиями вклада или кредита. Она может использоваться как discount rate, если подходит для оцениваемых cash flows; совпадение не обязательно.

## NPV — Net Present Value

**NPV is the present value of expected future net cash flows minus the initial investment. A positive NPV means the project is expected to add value.**

$$
\boxed{NPV=\sum_{t=1}^{N}\frac{CF_t}{(1+r)^t}-I_0}
$$

$I_0$ = первоначальное вложение сегодня.

**DCF:** сколько ожидаемые будущие поступления стоят сегодня.  
**NPV:** эта стоимость **минус первоначальное вложение**.

> [!example] Invest £100; expect £121 in one year; discount rate 10%
> $$PV=\frac{121}{1.10}=£110$$
> $$NPV=110-100=\boxed{+£10}$$
> Ты платишь £100 за ожидаемые поступления, которые при требуемой доходности 10% оцениваются сегодня в £110. Проект ожидаемо создаёт £10 дополнительной стоимости сегодня.
>
> Номинальная разница $121-100=£21$ отличается от NPV: NPV учитывает время и риск через discount rate.

| NPV | Interpretation | Decision under the assumptions |
|---|---|---|
| **NPV > 0** | Expected to create value above the required return | Accept |
| **NPV = 0** | Expected to meet the required return | No additional value above that return |
| **NPV < 0** | Expected cash flows do not justify the investment at the required return | Reject |

**NPV = 0 не означает отсутствие заработка.** Отрицательный NPV возможен даже при положительной номинальной прибыли. Положительный NPV зависит от прогнозов и не гарантирует отсутствие убытков.

## Bond pricing

| Term | Meaning |
|---|---|
| **Principal / face value** | Сумма, которую эмитент обещает вернуть при погашении |
| **Coupon** | Обещанный периодический процентный платёж |
| **Coupon rate** | Ставка, по которой coupon рассчитывают от face value |
| **Maturity** | Дата погашения |
| **Market yield** | Рыночная доходность, используемая как discount rate для этих платежей |
| **Bond price** | Сегодняшняя стоимость обещанных платежей |

$$
\boxed{P=\sum_{t=1}^{N}\frac{C}{(1+y)^t}+\frac{F}{(1+y)^N}}
$$

- $C$ = coupon per period; $F$ = face value; $y$ = market yield per period; $N$ = periods to maturity.
- **Final payment = final coupon + principal.** Обе части дисконтируются.
- Обещанные платежи предполагают, что эмитент выполнит обязательства.

> [!important] Bond prices and yields
> **Market yields rise → existing fixed-coupon bond prices fall.**  
> **Market yields fall → prices rise**, other things equal.  
> **The coupon remains fixed.** Coupon rate и market yield — разные величины.

Старый фиксированный coupon становится менее привлекательным, когда новые облигации предлагают более высокую доходность. Цена старой облигации снижается.

> [!example]- Lecture example — £4 annual coupon, £100 face value, 5 years, yield 6%
> $$PV(\text{coupons})=\sum_{t=1}^{5}\frac{4}{(1.06)^t}\approx £16.85$$
> $$PV(\text{principal})=\frac{100}{(1.06)^5}\approx £74.73$$
> $$P=16.85+74.73=\boxed{£91.58}$$

## P/E — Price-to-Earnings ratio

**P/E shows how many times annual earnings per share investors pay for a share.**

$$
\boxed{P/E=\frac{\text{Share price}}{\text{Annual EPS}}}
$$

**EPS — earnings per share:** прибыль компании на одну акцию. В базовом расчёте:

$$
\text{Basic EPS}=\frac{\text{Profit attributable to ordinary shareholders}}{\text{Weighted-average number of ordinary shares}}
$$

В простом случае без дополнительных корректировок числитель — **net income**. EPS — прибыль на акцию; **dividends** — выплаты акционерам. Это разные показатели.

> [!example] Share price £60; annual EPS £3
> $$P/E=\frac{60}{3}=\boxed{20}$$
> Цена акции в **20 раз больше её годовой EPS**. Инвесторы платят £20 за каждый £1 годовой прибыли на акцию. Это не £20 дохода инвестору.

### How P/E helps an investor

P/E помогает оценить, оправдана ли цена покупки прибылью и перспективами бизнеса:

1. Сравнить P/E с похожими компаниями на сопоставимой основе.
2. Выяснить причины различий: growth, risk, временно высокая или низкая прибыль.
3. Оценить, оправдывают ли эти перспективы цену.

**Low P/E** может указывать на недооценённый бизнес, но также на ожидание падения прибыли. **High P/E** может отражать сильный ожидаемый рост или чрезмерно оптимистичные ожидания. Универсального «хорошего P/E» нет.

> [!example]- Two shops — price relative to annual profit
>
> | | Shop A | Shop B |
> |---|---:|---:|
> | Business price | £1,000 | £2,000 |
> | Current annual profit | £200 | £200 |
> | **P/E** | **5** | **10** |
> | Outlook | Profit may remain around £200 | Profit may grow to £400 |
>
> Shop B дороже относительно текущей прибыли. Более высокая цена может быть оправдана будущим ростом. Если будущая прибыль, риски и остальные условия одинаковы, более низкая цена A привлекательнее.

P/E не показывает цели руководства и не даёт точного прогноза роста. Сам по себе он не является сигналом «покупать» или «не покупать».

> **P/E helps investors assess how much they are paying for earnings and whether that price is justified by future growth and risk.**

## P/B — Price-to-Book ratio

**P/B compares the market value of a company’s equity with its accounting book value.**

$$
\boxed{\text{Book value of equity}=\text{Accounting assets}-\text{Accounting liabilities}}
$$

$$
\boxed{P/B=\frac{\text{Market value of equity}}{\text{Book value of equity}}}
$$

**Market value of equity** — рыночная стоимость всех акций. **Book value of equity** — собственный капитал по бухгалтерскому учёту.

> [!example] Market value vs book value
>
> | Item | Amount |
> |---|---:|
> | Assets | £1,000 |
> | Liabilities | £400 |
> | **Book value of equity** | **£600** |
> | **Market value of equity** | **£900** |
>
> $$P/B=\frac{900}{600}=\boxed{1.5}$$
> Инвесторы платят **£1.50 за каждый £1 бухгалтерской стоимости equity** — £300 сверх book value всего собственного капитала.

| P/B | Meaning |
|---|---|
| **P/B = 1** | Рыночная стоимость equity равна бухгалтерской |
| **P/B > 1** | Рыночная стоимость выше бухгалтерской |
| **P/B < 1** | Рыночная стоимость ниже бухгалтерской |

### How P/B helps an investor

P/B показывает разницу между market value и book value. Затем нужно объяснить её: будущая прибыль, бренд, технологии, клиентская база, риски и качество учётной оценки активов.

**P/B < 1 не означает автоматически выгодную покупку.** Низкая оценка может отражать слабую прибыльность, ожидаемые убытки или сомнения в стоимости активов. Book value не гарантирует сумму, которую получится получить при продаже бизнеса.

> [!example]- If the market values the same equity at £300
> $$P/B=\frac{300}{600}=0.5$$
> Возможны как недооценка бизнеса, так и обоснованная низкая цена из-за рисков или завышенной учётной стоимости активов. Чтобы оценить цену, нужно проверить причины расхождения.

**Сравнивать P/B полезно для похожих компаний с учётом их прибыльности и риска.**

| Ratio | What the price is compared with |
|---|---|
| **P/E → earnings** | Годовая прибыль |
| **P/B → book equity** | Бухгалтерская стоимость собственного капитала |

## Market price vs fundamental value

- **Market price** — цена, по которой актив сейчас торгуется.
- **Fundamental value** — оценка стоимости на основе ожидаемых future cash flows, времени и риска.

Это разные понятия. DCF-оценка зависит от предположений и не является гарантированно правильной рыночной ценой.

## Law of one price and arbitrage

**Law of one price:** identical assets with identical future payoffs and risks should have the same price, assuming no significant trading costs or restrictions.

**Arbitrage:** simultaneously buying an identical asset at a lower price and selling it at a higher price.

> [!example] Same asset, two markets
> Buy at **£100** in market A and simultaneously sell at **£105** in market B.
> $$\text{Gross difference}=105-100=£5$$
> Предполагаем, что обе сделки можно выполнить; комиссии и другие издержки не учитываем.

Покупки на дешёвом рынке и продажи на дорогом помогают сокращать ценовую разницу.

> **Arbitrage tends to enforce the law of one price by reducing price differences between identical assets.**

Law of one price — **принцип**, arbitrage — **механизм**, который помогает ему выполняться. Одинаковая цена на двух рынках не доказывает, что она равна верной fundamental value.

## EMH — Efficient Market Hypothesis

**EMH suggests that market prices reflect available information and adjust quickly when new information arrives.**

Текущая цена уже отражает доступную информацию. Новая неожиданная информация меняет ожидания — цена корректируется.

> [!example]- Why reading a good news story may not give you an advantage
> Акция стоит £100 → неожиданно хорошая новость → инвесторы реагируют → цена становится £110 → ты читаешь новость, но купить по прежним £100 уже нельзя.

**Consistently earning abnormal risk-adjusted returns using information already reflected in prices is difficult.**

EMH не гарантирует, что любая цена всегда идеально правильная, никто никогда не обгонит рынок или рынки не могут резко падать.

---

> [!info]- Sources and original images
> Основа: [[Uni/Modules/IC101 - Finance/Revision/cheat sheet.pages|личный cheat sheet в Pages]]. Текст и таблицы перенесены в Markdown; формулы — в LaTeX. Формулировки уточнены и дополнены по [[IC101 L01 — Study Guide#Проверка личного cheat sheet — 31 октября 2026|проверке от 31 октября 2026]].
>
> Материалы курса: [[IC101 L01 — Slides.pdf]] · [[IC101 S01 — Slides.pdf]].
>
> Дополнительное объяснение valuation ratios: [CFA Institute](https://www.cfainstitute.org/insights/professional-learning/refresher-readings/2026/market-based-valuation-price-enterprise-value-multiples).
>
> Исходные изображения формул из Pages сохранены вместе с основной схемой finance:
> ![[IC101 L01 — DCF Formula.png|600]]
> ![[IC101 L01 — NPV Formula.png|500]]
> ![[IC101 L01 — Bond Pricing Example.png|600]]
> ![[IC101 L01 — PE Formula.png|500]]
> ![[IC101 L01 — PB Formula.png|500]]
