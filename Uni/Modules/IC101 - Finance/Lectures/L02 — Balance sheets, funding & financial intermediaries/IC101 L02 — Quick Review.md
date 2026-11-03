---
title: "IC101 L02 — Quick Review"
course: IC101
lecture: 2
seminar: 2
topic: "Balance Sheets, Funding & Financial Intermediaries"
type: quick-review
slides_verified: true
seminar_verified: true
transcript_verified: false
tags: [IC101, finance, lecture-2, seminar-2, active-recall]
module: IC101 - Finance
---

# IC101 L02 — Quick Review

Подробности и все решения: [[IC101 L02 — Deep Notes]]. Около 10–15 минут на повторение.

> [!warning] Source status
> Проверены **Lecture 2.pdf**, 28 страниц, и **Seminar 2.pdf**, 12 страниц, найденные локально в Downloads. **Transcript недоступен**: объяснения преподавателя по нему не проверены. Обозначения: **L** = Lecture, **S** = Seminar; числа после них — страницы PDF. **Clarification** = пояснение автора заметок, а не отдельный тезис slides. Полный Source audit: [[IC101 L02 — Deep Notes#Source audit]].

## 1. Balance Sheet: одна карта

$$
\boxed{A=L+E},\qquad E=A-L,\qquad \text{Equity Cushion}=\frac{E}{A}.
$$

- **Assets** — чем располагает компания; **Liabilities** — что она должна; **Equity** — остаточное требование Owners.
- **Equity не является отдельной суммой Cash**. Это разница между Assets и Liabilities.
- **Current**: в учебной схеме — в пределах года; **Non-current** — позже. Assets описывают размещение средств, правая сторона — источники Funding. [L4–6; S4]
- **Clarification:** Liabilities шире, чем Interest-bearing Debt: Accounts Payable тоже являются Liabilities. В упрощённых задачах ниже все Liabilities считаются Debt.

**Пример S4:** $A=100$, $D=70$, $E=30$; Equity Cushion = 30%. Если Assets падают до 70 при прежнем Debt, Equity = 0. **Lenders начинают терять при дальнейшем падении ниже 70**, а не автоматически при Equity = 0.

> [!danger] Bankruptcy: что распределяется?
> В учебной Liquidation Model распределяют доступные средства от Assets. **Equity — остаток после требований**, а не ещё один мешок денег для выплаты. Упрощённая очередь L17: Senior Debt → Junior Debt → Preference Shares → Ordinary Shares. Ordinary Equity — **First Loss**, хотя стоит последней в очереди выплат. Это учебная схема, а не полный порядок по закону.

## 2. ROE: сначала Interest, затем остаток, затем Equity

Для задач L12 и S5–6, S11: Taxes и другие расходы после Operating Profit не моделируются.

$$
I=r_DD,\qquad \Pi_E=OP-I,\qquad
\boxed{ROE=\frac{OP-r_DD}{E}\times100\%}.
$$

**Debt Principal** $D$ — сама сумма займа; **Interest** $I$ — плата за период. Если $D=100$ и $r_D=6\%$, Interest = 6, **не 100 и не 106**. Repayment of Principal — отдельный Cash Flow; не вычитай весь Principal из Operating Profit в задаче на ROE.

| Case | Assets | Equity | Debt | Interest | Operating Profit | Profit to Owners | ROE |
|---|---:|---:|---:|---:|---:|---:|---:|
| Delta, All-equity, Good Year | £200 | £200 | £0 | £0 | £20 | £20 | 10% |
| Delta, 50% Debt, Good Year | £200 | £100 | £100 | £6 | £20 | £14 | 14% |
| Delta, All-equity, Bad Year | £200 | £200 | £0 | £0 | £4 | £4 | 2% |
| Delta, 50% Debt, Bad Year | £200 | £100 | £100 | £6 | £4 | **−£2** | **−2%** |
| Final Exam-style Question | £300 | £200 | £100 | £6 | £30 | £24 | **12%: B** |

[S5–6; S11]

> [!important] Negative ROE
> При положительном Equity отрицательный остаток после Interest даёт отрицательный ROE. Operating Profit = 4 ещё не означает положительный Profit to Owners: $4-6=-2$. Это не означает, что Debt Principal стал отрицательным или что компания автоматически обанкротилась.

**Leverage** усиливает результаты в обе стороны. При одинаковых Assets и Operating Profit оно не создаёт дополнительный Operating Profit: меняются Interest и Equity, на которое делят остаток. [L10–13]

## 3. Debt vs Equity: trade-off

| | Debt | Ordinary Equity |
|---|---|---|
| Что получает поставщик Funding | Contractual Claim | Residual Claim |
| Payments | Interest и Repayment по условиям | Dividends не обязательны в схеме курса |
| Founder Ownership | Нет Dilution от самого займа | New Shares вызывают Dilution |
| Главный риск для Founder | Debt Service, Financial Risk, Refinancing | Меньше Ownership и доля будущего результата |
| Возможный плюс | Сохранение доли; Tax Shield в модели L14 | Нет обязательного Interest или погашения как по Debt |

[L7, L10, L14; S9]

**Clarification к твоему ответу:** Debt может поднять **ROE**, но не гарантирует рост Profit или любого показателя **ROI**. Продажа части Equity уменьшает долю, но **не всегда автоматически лишает Control**; доля будущего Profit меньше, а его абсолютная сумма после роста бизнеса может оказаться больше.

**Business Risk**: Competition, Demand, Operating Costs. **Financial Risk**: дополнительная уязвимость из-за Debt. Recession — Business Shock; Interest, который всё равно нужно обслуживать, усиливает последствия. [L13; S7]

## 4. Interest Rate: когда рост ставок действует?

> [!note] Clarification к L15–18 и S7
> **Variable-rate Debt:** Interest меняется при Reset по условиям договора. **Fixed-rate Debt:** текущий договорный Rate не растёт автоматически вместе с Market Rates в период фиксации. **Refinancing:** когда старый Debt заменяют новым, новый Rate может быть выше даже после Fixed-rate Debt. **Refinancing Risk** — риск не получить новый Funding или получить его на тяжёлых условиях.

```text
Market Rates rise
├─ Variable-rate Debt → Reset → Interest may rise
└─ Fixed-rate Debt → Rate unchanged during fixed period
                      └─ Maturity / Refinancing → new terms may be worse
```

## 5. M&M → Tax Shield → Optimal Capital Structure

**M&M I:** в идеальном мире модели без Taxes и Bankruptcy Costs один только Debt–Equity Mix не меняет Firm Value. Это не обещание одинакового ROE. [L14]

$$
V_L=V_U \quad\text{(M\&M base case)}.
$$

**Tax Shield:** в модели L14 Interest уменьшает Taxable Profit.

$$
\text{Annual Tax Shield}=T_c\times I=T_c r_DD.
$$

Пример L14: $D=£100m$, $r_D=5\%$, $T_c=25\%$ → $I=£5m$ → Annual Tax Shield = **£1.25m**. Это не сумма займа и не весь Interest.

```text
More Debt → Tax Shield → Firm Value up
More Debt → Expected Distress Costs → Firm Value down
                    ↓
Optimal Capital Structure: mix giving highest Firm Value
```

**Clarification:** пик около 40% Debt на рисунке L14 иллюстративен. Универсального «правильного процента Debt» из лекции не следует. Полная формула Present Value of Tax Shield в slides не выводится.

## 6. Primary vs Secondary: сначала Cash Recipient

| Сделка в S8 | Market | Cash Recipient |
|---|---|---|
| Покупка New Shares в обозначенном в slides IPO case | Primary | Issuer |
| Покупка 10 существующих Apple Shares через Trading App | Secondary | Selling Investor |
| New £500m Bond Issue National Grid | Primary | National Grid |
| Продажа своего Gilt другому Investor | Secondary | Ты, как Seller |

В пересказе беседы было 2,000 Shares; в PDF — 10. **Количество классификацию не меняет.** Вопрос — New Issue или Trade of Existing Securities. Исторические утверждения IPO case не проверялись; для ответа достаточно структуры сделки.

**Primary** даёт новый Funding Issuer; **Secondary** даёт Market Liquidity и Price Discovery. При обычной Secondary Trade компания не получает сумму твоей покупки. [L23–24; S8, S10]

## 7. Financial Intermediaries: на чьём Balance Sheet сделка?

```text
Saver: Deposit = Asset
              ↓
Bank: Deposit = Liability | Loan = Asset
                                      ↓
Company: Loan = Liability
```

- **Agency / Broker**: сводит стороны; основная сделка не становится собственной Asset Position; зарабатывает Fee / Commission.
- **Principal / Transforming Intermediary**: сам становится Counterparty; держит Position на собственном Balance Sheet и принимает связанный риск. Bank, Market Maker, Insurer — примеры L20.
- **Principal as intermediary** — роль в сделке; **Debt Principal** — сумма займа. Это разные значения слова.
- **Clarification:** фраза «every asset is someone else’s liability» из L2 относится к связям Financial Claims; здание или оборудование не обязано быть чьей-то Liability. Equity Claim у Investor соответствует Equity Issuer, а не Debt Liability. [L8, L20–22]

## Active Recall

Сначала ответь вслух; затем раскрой Callout.

1. $A=100$, $L=80$: сколько Equity? Где лежит Equity Cash?
2. $OP=4$, $D=100$, $r_D=6\%$, $E=100$: найди Interest, Profit to Owners и ROE.
3. Нужно ли вычитать Debt Principal = 100 при вычислении этого ROE?
4. Почему Debt может поднять ROE, хотя Operating Profit не меняется?
5. Market Rates выросли: почему Fixed-rate Debt не обязательно сразу дорожает?
6. $A=70$, $D=70$: сколько Equity? Начались ли потери Lenders в простой модели?
7. Купил Existing Shares в приложении: кому ушли деньги?
8. Чем M&M Base Case отличается от модели с Tax Shield и Distress Costs?
9. $I=5m$, $T_c=25\%$: сколько Annual Tax Shield?
10. Почему ответ B в последней задаче Seminar 2 — 12%, а не 10%?
11. Broker и Bank: какой тест отличает Agency от Principal?
12. Почему New Equity не означает автоматическую потерю Control?

> [!check]- Answers
> 1. Equity = 20; отдельной Equity Cash нет. 2. Interest = 6; Profit to Owners = −2; ROE = −2%. 3. Нет: Repayment of Principal — отдельный Cash Flow. 4. Interest уменьшает остаток, но Equity Denominator тоже меньше; результат зависит от Operating Return относительно Debt Rate. 5. Действует договорный Rate до конца фиксации; новые условия возникают при Reset / Refinancing. 6. Equity = 0; Lenders ещё покрыты ровно на 70, дальнейшее падение вызывает Shortfall. 7. Selling Investor. 8. Без Frictions Mix не меняет Firm Value; с Tax Shield и Distress Costs появляется Trade-off. 9. £1.25m. 10. $(30-6)/200=12\%$: делим на Equity. 11. Становится ли основная Position собственной Asset / Liability Exposure посредника? 12. Dilution и Control — разные вопросы; важны доля и права.

Следующий шаг: [[IC101 L02 — Deep Notes#Weakness Analysis]] и [[IC101 L02 — Deep Notes#Active Recall — Practice Set]].
