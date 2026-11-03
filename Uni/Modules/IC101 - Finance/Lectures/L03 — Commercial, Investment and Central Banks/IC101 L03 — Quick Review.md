---
title: "IC101 L03 — Quick Review"
module: IC101 - Finance
lecture: 3
type: quick-review
language: ru
tags:
  - IC101
  - lecture-3
  - seminar-3
  - economics
  - quick-review
---

# IC101 L03 — Quick Review

> [!info] Навигация
> Полное объяснение, Seminar 3 и Active Recall: [[IC101 L03 — Deep Notes]].  
> Источники: **Lecture 3, slides 1–30 + transcript**; **Seminar 3, slides 1–12**. Время повторения: **5–10 минут**.

## 1. Main Ideas

1. **Commercial Banks** принимают **Deposits** и предоставляют **Loans**. Для клиента Deposit — **Asset**, для банка — **Liability**.
2. **Bank Transformation**: **short / safe / small Deposits → long / risky / large Loans**. Это обеспечивает Credit, но создаёт **Maturity Mismatch**.
3. **Money Creation**: новый Loan создаёт новый Bank Deposit; покупка/Transfer перемещает Deposit; погашение **Loan Principal** уничтожает соответствующий Deposit Money.
4. **Bank Fragility**: фиксированные **Liabilities**, рискованные **Assets**, небольшой **Equity Cushion**.
5. **Expected Loss** оценивается через **PD × LGD × Loan Amount**; в модели лекции обычный Expected Loss покрывается **Revenue**, дополнительные **Unexpected Losses** сокращают **Equity**.
6. **Bank Run** — массовые Withdrawals. **Illiquidity ≠ Insolvency**.
7. **Safety Net**: **Supervision**, **Capital Requirements**, **Liquidity Buffers**, **Deposit Insurance**, **Lender of Last Resort**.
8. **Central Bank** проводит **Monetary Policy**; **Investment Bank** работает с **Underwriting**, **M&A**, **Sales & Trading**, **Asset & Wealth Management**.

## 2. Key Concepts — различия для экзамена

| Concept | Короткий смысл |
|---|---|
| **Asset** | То, чем банк владеет или что ему должны: Cash & Reserves, Loans, Bonds |
| **Liability** | То, что банк должен: Deposits, Borrowings |
| **Equity** | Остаток Assets после вычета Liabilities; поглощает Losses |
| **Maturity Transformation** | Borrow short, lend long |
| **Risk Transformation** | Diversification большого числа Loans; риск не исчезает полностью |
| **Liquidity Risk** | Недостаточно доступных средств для платежей сегодня |
| **Credit Risk** | Borrower может не выполнить Loan obligations |
| **Illiquid** | Достаточно Assets, но не хватает Cash **сейчас** |
| **Insolvent** | Assets **меньше** Liabilities; Equity < 0 |
| **Moral Hazard** | Ожидаемая помощь может стимулировать больше Risk |
| **Systemic Risk** | Collapse одного банка угрожает другим участникам/системе |

> [!danger] Твоя главная слабая тема — Illiquidity vs Insolvency
> **Не делай вывод «Insolvent», только потому что Cash мало или Cash не назван.**  
> **Test 1:** Сравни **Total Assets и Total Liabilities** → Insolvency?  
> **Test 2:** Сравни немедленные Withdrawals и доступную Liquidity → Illiquidity?

## 3. Important Formulas

$$
\text{Assets}=\text{Liabilities}+\text{Equity}
$$

$$
\text{Equity}=\text{Assets}-\text{Liabilities}
$$

$$
\text{Expected Loss (EL)}=\text{PD}\times\text{LGD}\times\text{Loan Amount}
$$

$$
\text{Unexpected Loss (simplified)}=\text{Actual Loss}-\text{Expected Loss}
$$

**Seminar 3 — готовые контрольные расчёты:**

- £10,000 Loan; PD 5%; LGD 50% → **EL = £250**. Actual Loss £900 → **£650 above Expected Loss** (упрощённая модель).
- Northshore: Loans £200, Deposits £190, Equity £10. Assets lose £6 → **Assets £194; Equity £4; still solvent**.
- Riverbank: Loans £104, Deposits £100, demand £30 today, Cash £2 → **Illiquid**, при условии, что Assets оценены верно и достаточно качественны.
- Peakwater: Assets £96, Deposits £100 → **Equity −£4; Insolvent**.
- Exam MCQ: Loan £5,000, PD 2%, LGD 40% → **EL £40**.

## 4. Economic Mechanisms — WHY / HOW

**Maturity Mismatch**  
Deposits withdrawable today → Loans repay over years → Cash needed now may exceed Liquidity → **Liquidity Risk**.

**Money Creation**  
Loan £200 → Borrower's Deposit +£200 → Money Supply +£200 → payment to seller **does not itself change total deposits** → Principal repayment £200 → corresponding Deposit Money −£200.

**Bank Fragility**  
Loan Assets lose value → Assets ↓ → Deposits owed stay fixed → Equity ↓ → possible **Insolvency**.

**Bank Run**  
Rumour → Withdrawals ↑ → Liquidity shortage → possible **Fire Sale** → Losses ↑ → Equity ↓ → more panic.

**Bank Rate ↑**  
Borrowing Costs ↑ → Consumption / Investment may ↓ → Aggregate Demand ↓ → Inflationary Pressure ↓.

**QE**  
Central Bank buys Bonds → Bond Demand / Prices ↑ → Bond Yields ↓ → financing conditions may ease. **QT** reverses balance-sheet expansion (sales or maturities without reinvestment).

## 5. Essential Graphs / Diagrams

| Slide | Axes / composition | Экономический вывод |
|---|---|---|
| **5–6: Transformation / Lloyds** | Left: Deposits; Right: Loans, both £bn | Short liabilities fund long Assets; mismatch |
| **8: Money Composition** | ~£3 Cash vs ~£97 Bank Deposits per £100 | Bank Deposits dominate broad money in the lecture illustration |
| **9: Money Creation** | Before £1,000 → Loan +£200 → £1,200 → Repayment → £1,000 | Lending creates Deposits; repayments remove them |
| **10 & 13: Fragility / Loss Waterfall** | Assets vs Deposits / Equity; losses allocated to Revenue and Equity | Small equity cushion can vanish quickly |
| **15–16: Bank Runs** | X: year/time; Y: failed-bank Assets / withdrawals | Digital banking makes Runs faster; SVB case |
| **20: Equity Capital** | X: 2007, 2013, 2024; Y: core equity %, approx | Capital cushion increased (~4% → ~11% → ~14%) |
| **22: Monetary Policy** | X: years; Y: Bank Rate %, CPI %, QE Bond Holdings £bn | Rates, Inflation and QE/QT change over time |
| **25: Goldman Sachs** | Business lines vs Revenue ($bn) | Sales & Trading > Investment Banking Fees in slide's 2025 case |

> [!note] Graph interpretation
> Для каждого графика умей назвать **X-axis, Y-axis, direction of change, mechanism, economic meaning**. Historical values above — **из слайдов**, не текущие показатели.

## 6. Three Banks — One System

| | Commercial Bank | Central Bank | Investment Bank |
|---|---|---|---|
| Main role | Deposits & Loans | Monetary Policy & stability | Capital Markets & deals |
| Typical clients | Households / Businesses | Banks / Government | Companies / Investors / Governments |
| Money Creation | Creates Deposits through Lending | Creates Central Bank Money | Not by ordinary retail-deposit Lending |
| Main activities | Payments, Credit | Bank Rate, QE/QT, reserves, emergency liquidity | Underwriting, M&A, Trading, Asset Management |

## 7. Common Mistakes — персонально

> [!warning] Needs Revision
> **1.** «Мало Cash → Insolvent» — неверно. Мало Cash относится к **Illiquidity**; **Insolvency** проверяется через Assets − Liabilities.  
> **2.** **Deposits ≠ Equity**. Deposit клиента — Liability банка.  
> **3.** «При выдаче £300 Loan Money Supply остаётся £1,000 из-за Debt» — неверно. В учебном примере Deposits растут до £1,300; Debt существует одновременно, но это не то же самое, что Money Supply.  
> **4.** Перевод денег продавцу ≠ уничтожение денег. **Principal repayment** уничтожает соответствующие Deposit Money.  
> **5.** Rescue Decision: сначала выясни **Illiquid or Insolvent**, затем **Systemic Risk**, вклад Depositors и **Moral Hazard**.

## 8. Exam Takeaways

- **Expected Loss**: подставляй PD и LGD как десятичные дроби; не забывай **Loan Amount**.
- **Equity Cushion**: при неизменных Liabilities падение Assets на £1 уменьшает Equity на £1.
- **At Equity = 0** cushion полностью исчезает; **Equity < 0** — Insolvency в упрощённой модели.
- **Emergency Loan** может помочь Illiquid Bank, но сам по себе не исправляет Insolvent Bank.
- **Capital ≠ Liquidity**: Capital покрывает Losses; Liquidity Buffers — Withdrawals.
- **Underwriting** = размещение Shares/Bonds и иногда гарантия продажи; **M&A Advisory** = помощь с покупкой/продажей Companies.

> [!caution] Несогласованность источника: FSCS
> В Lecture 3 **Slide 19: £110,000**, а **Slide 29: £120,000**. В записях не фиксируем ни одну как проверенный актуальный лимит. Для реальной суммы требуется отдельная проверка условий FSCS.

**Следующий шаг:** подробная логика, Seminar 3, Graph Walkthrough и вопросы — [[IC101 L03 — Deep Notes]].
