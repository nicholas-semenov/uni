---
type: lecture-explanation
module: IC104 - Math
lecture: "[[IC104 L03 — Partial Differentiation and Integration]]"
generated: 2026-10-14
model: claude-opus-5
sources: slides
---

# IC104 L03 — Explanation

> [!info] Пошаговое объяснение (сгенерировано). Лекция: [[IC104 L03 — Partial Differentiation and Integration]]. Ссылки *(Slide N; MM:SS)* ведут к источнику — сверяйся с ними.

## Overview

This is Lecture 3 of IC104 (Introductory Quantitative Techniques for Business and Finance). It has two main halves: first, partial differentiation — how to differentiate a function that has two variables (x and y) by treating one variable as a constant; second, integration — what a definite integral means (the area under a curve), its main properties, the Fundamental Theorem of Calculus, and the standard rules for computing integrals (Slides 1–2). This matters because economic and finance models usually depend on several variables at once (for example a production function, or an option price that depends on time, interest rate, volatility and the price of the underlying asset), and integration is the basic tool for adding up continuously changing quantities (Slides 3, 7).

## 1. What the lecture covers

The lecture plan has two topics. The first is partial differentiation, with the textbook reference Sydsaeter & Hammond Chapter 11.1–11.2. The second is integration, with reference Sydsaeter & Hammond Chapter 9.1–9.5 (Slide 2).

An important practical point: Slides 19–29 are explicitly marked "For interest only – not examinable". This covers the distance/job problem, integration by parts and integration by substitution. Everything up to and including Slide 18 is presented as normal (examinable) material. *(Slide 1; Slide 2; Slide 19; Slide 22; Slide 26)*

**Key points:**

- Part 1: Partial differentiation (textbook Ch. 11.1–11.2).
- Part 2: Integration (textbook Ch. 9.1–9.5).
- Slides 19–29 are labelled 'not examinable'.

> [!note] Interpretation (not stated directly in the sources)
> A sensible study strategy is to master Slides 3–18 first, and read Slides 19–29 only afterwards for understanding. This is my advice, not a statement from the slides.

## 2. Functions of two variables

Until now you have probably worked with functions of one variable, like y = f(x). Slide 3 extends this: a function f of two real variables x and y with domain D is a rule that gives one specific number f(x, y) to each point (x, y) in D. We write z = f(x, y), where the domain D is a subset of the xy-plane. So instead of one input number you now give the function a *pair* of numbers.

The slide gives an economic example that appears in many models: F(x, y) = A·x^a·y^b, where A, a and b are constants. This is called a Cobb–Douglas function. It is used as a production function: x and y are input factors, and F(x, y) is the output, that is, the number of units produced (Slide 3). *(Slide 3)*

**Key points:**

- A function of two variables assigns exactly one value f(x, y) to each point (x, y) in its domain D.
- Notation: z = f(x, y); D is a subset of the xy-plane.
- Cobb–Douglas form: F(x, y) = A·x^a·y^b with constants A, a, b.
- In the Cobb–Douglas production function, x and y are inputs and F(x, y) is output.

**Examples:**

- F(x, y) = A·x^a·y^b — a production function where two inputs (for example capital and labour) produce output.

> [!note] Interpretation (not stated directly in the sources)
> Background (not in the slides): the two inputs in a Cobb–Douglas production function are usually interpreted as capital and labour. Geometrically, z = f(x, y) can be pictured as a surface above the xy-plane, like a hill, which helps explain why we need two different derivatives.

## 3. The idea of a partial derivative

With two variables there is no single "the" derivative, because the function can change when x changes and also when y changes. The trick is to look at one variable at a time. Slide 4 uses z = x³ + 2y². If we suppose y is a constant, then z behaves like a function of x only, and differentiating gives 3x². If instead we keep x fixed, z behaves like a function of y only, and differentiating gives 4y. Notice that when y is treated as a constant, the whole term 2y² is a constant and so disappears; the same happens to x³ when x is held fixed.

This gives the definition on Slide 4: if z = f(x, y), then ∂z/∂x denotes the partial derivative of f(x, y) with respect to x, when y is held constant, and ∂z/∂y denotes the partial derivative with respect to y, when x is held constant. The curly symbol ∂ (instead of d) is the signal that other variables are being held fixed. *(Slide 4)*

**Key points:**

- A partial derivative differentiates with respect to one variable while treating the other variable as a constant.
- ∂z/∂x: differentiate in x, hold y constant. ∂z/∂y: differentiate in y, hold x constant.
- Terms that contain only the 'held constant' variable become constants and differentiate to zero.
- The symbol ∂ marks a partial derivative, as opposed to the ordinary d.

**Examples:**

- z = x³ + 2y²: ∂z/∂x = 3x² (y fixed), ∂z/∂y = 4y (x fixed) (Slide 4).

> [!note] Interpretation (not stated directly in the sources)
> Intuition (mine): ∂z/∂x answers 'if I increase input x a little and keep y exactly the same, how fast does the output change?' In economics this is the basis of marginal products.

## 4. Worked examples of partial derivatives

Slide 5 gives two examples. Example 1: f(x, y) = x³y + x²y² + x + y². Holding y constant, ∂f/∂x = 3x²y + 2xy² + 1. Here y and y² act like plain numbers multiplying powers of x, the term x differentiates to 1, and the term y² (no x in it) disappears. Holding x constant, ∂f/∂y = x³ + 2x²y + 2y; this time the lone x term disappears.

Example 2: f(x, y) = xy / (x² + y²). Because this is a quotient, the quotient rule is used while treating y as a constant: ∂f/∂x = [y(x² + y²) − 2x·xy] / (x² + y²)², which simplifies to (y³ − x²y)/(x² + y²)². By the same method (and because the function is symmetric if you swap the roles of x and y), ∂f/∂y = (x³ − y²x)/(x² + y²)² (Slide 5). *(Slide 5)*

**Key points:**

- The usual rules of differentiation (power, product, quotient, chain) still apply — only the 'other' variable is frozen.
- A term containing none of the variable you differentiate by gives zero.
- In Example 2 the quotient rule is applied with y treated as a number.

**Examples:**

- f = x³y + x²y² + x + y² → ∂f/∂x = 3x²y + 2xy² + 1; ∂f/∂y = x³ + 2x²y + 2y.
- f = xy/(x² + y²) → ∂f/∂x = (y³ − x²y)/(x² + y²)²; ∂f/∂y = (x³ − y²x)/(x² + y²)².

> [!note] Interpretation (not stated directly in the sources)
> Checking tip (mine): in the second example you can get ∂f/∂y 'for free' by noticing that swapping x and y leaves the function unchanged, so you just swap x and y in the answer for ∂f/∂x. The slide does not say this, but the two results are consistent with it.

## 5. Higher-order (second-order) partial derivatives

∂f/∂x and ∂f/∂y are called first-order partial derivatives. If these are themselves functions of (x, y), we can differentiate them again, and because there are two choices each time, we get four second-order partial derivatives (Slide 6): ∂/∂x(∂f/∂x) = ∂²f/∂x², ∂/∂x(∂f/∂y) = ∂²f/∂x∂y, ∂/∂y(∂f/∂x) = ∂²f/∂y∂x, and ∂/∂y(∂f/∂y) = ∂²f/∂y².

The slide continues the earlier example f(x, y) = x³y + x²y² + x + y² and reports: ∂²f/∂x² = 6xy + 2y², ∂²f/∂y∂x = ∂²f/∂x∂y = 3x² + 4xy, and ∂²f/∂y² = 2x² + 2. The important observation is that the two 'mixed' partial derivatives are equal here: it does not matter whether you differentiate first in x then in y, or the other way round. *(Slide 6)*

**Key points:**

- First-order partials can be differentiated again, giving four second-order partials.
- Two of them are 'pure' (∂²f/∂x², ∂²f/∂y²) and two are 'mixed' (∂²f/∂x∂y, ∂²f/∂y∂x).
- In the slide's example the two mixed partials are equal: ∂²f/∂y∂x = ∂²f/∂x∂y = 3x² + 4xy.

**Examples:**

- f = x³y + x²y² + x + y²: ∂²f/∂x² = 6xy + 2y²; mixed = 3x² + 4xy; ∂²f/∂y² = 2x² + 2.

> [!note] Interpretation (not stated directly in the sources)
> Background (mine, not on the slides): the equality of the mixed partials is a general result (often called Young's or Schwarz's theorem) that holds when the second-order partials are continuous. The slide only shows it happening in one example and does not state the condition.

## 6. Why partial derivatives matter in finance

Slide 7 motivates the topic with derivatives trading. It says partial derivatives are used extensively in the pricing and hedging of derivatives. A bank's derivative trading desk may hold billions of pounds' worth of derivative positions, and it needs to insure (hedge) itself against changes in the value of those positions caused by changes in time, interest rate, volatility and the price of the underlying assets.

The Black–Scholes formula is used extensively to price simple derivatives. By taking the partial derivatives of the Black–Scholes formula with respect to time, interest rate, volatility and the price of the underlying asset, we obtain exact formulas for the sensitivity of the position in each of these dimensions. Traders then use these sensitivities to decide how much interest-rate exposure, volatility, or how many units of the underlying they need to buy or sell in order to hedge their positions (Slide 7). *(Slide 7)*

**Key points:**

- Each partial derivative of an option price measures sensitivity to one risk factor, holding the others fixed.
- The four factors named on the slide: time, interest rate, volatility, price of the underlying asset.
- Black–Scholes gives closed-form sensitivities, which traders use to size their hedges.

**Examples:**

- Partial derivative of the Black–Scholes price with respect to the underlying asset price → tells the trader how many units of the underlying to buy or sell to hedge.

> [!note] Interpretation (not stated directly in the sources)
> Background (mine): these sensitivities are known in practice as 'the Greeks' (delta, vega, rho, theta). The slide describes them but does not use these names.

## 7. The area problem: where integration comes from

The second half of the lecture starts from a geometric question (Slide 8): how do we find the area of the region S that lies under the graph of f(x) between x = a and x = b, where f(x) is continuous on the interval [a, b]? For a straight line or a rectangle this is easy, but for a curve we need a new idea.

The method is approximation by rectangles. We create a partition Pn of the interval [a, b] — that is, we cut [a, b] into n small pieces — and use rectangles to compute an upper bound U(Pn, f(x)) and a lower bound L(Pn, f(x)) for the area of S. The lower sum uses rectangles that stay below the curve, the upper sum uses rectangles that stick out above it, so the true area is squeezed between them. Then we consider the limits as n → ∞: lim L(Pn, f(x)) and lim U(Pn, f(x)). As the slide puts it, we make each of the rectangles infinitely thin (Slide 8). *(Slide 8)*

**Key points:**

- Goal: the area under a continuous curve f(x) between a and b.
- A partition Pn cuts [a, b] into n subintervals.
- L(Pn, f) is a lower bound (rectangles under the curve); U(Pn, f) is an upper bound.
- We take the limit as n → ∞, i.e. infinitely many infinitely thin rectangles.

> [!note] Interpretation (not stated directly in the sources)
> Mental picture (mine): think of measuring the area of a hill-shaped field by covering it with narrower and narrower strips. Narrower strips leave less error, and in the limit the error vanishes.

## 8. The definite integral and integrability

Slide 9 turns the limit idea into a definition. If lim(n→∞) L(Pn, f(x)) = lim(n→∞) U(Pn, f(x)), then the definite integral of f(x) from a to b is written ∫ from a to b of f(x)dx, and it equals that common limit, called A. In other words, the larger and the smaller rectangles eventually converge to exactly match the area under the curve.

Two points of vocabulary from the slide: A can be interpreted as the area under the curve S; and if we can calculate the area under the curve, we say that f(x) is integrable. So 'integrable' means the squeezing procedure actually works and gives one single number. *(Slide 9)*

**Key points:**

- Definition: ∫ₐᵇ f(x)dx = lim L(Pn, f) = lim U(Pn, f) = A, when the two limits are equal.
- A is interpreted as the area under the curve.
- If the area can be calculated this way, f(x) is called integrable.
- a and b are the limits of integration; dx shows which variable we integrate over.

## 9. Properties of the definite integral (Slides 10–12)

The slides list nine properties. Properties 1–4 (Slide 10): (1) ∫ₐᵇ f(x)dx = −∫_bᵃ f(x)dx — swapping the limits changes the sign; (2) ∫ₐᵃ f(x)dx = 0, because graphically there is no area: the rectangle has width zero; (3) ∫ₐᵇ c dx = c(b − a) for a constant c, which graphically is the area under a straight horizontal line, i.e. a rectangle of height c and width b − a; (4) ∫ₐᵇ [f(x) + g(x)]dx = ∫ₐᵇ f(x)dx + ∫ₐᵇ g(x)dx — you can split a sum of functions.

Properties 5–7 (Slide 11): (5) ∫ₐᵇ c·f(x)dx = c·∫ₐᵇ f(x)dx — multiplying the function by a constant multiplies the value of the integral by that constant; (6) ∫ₐᶜ f(x)dx + ∫_cᵇ f(x)dx = ∫ₐᵇ f(x)dx for a < c < b — we can stick two adjacent areas under the same graph together; (7) if f(x) ≥ 0 on [a, b] then ∫ₐᵇ f(x)dx ≥ 0 — if a function is positive over an interval, its integral is also positive there.

Properties 8–9 (Slide 12): (8) if f(x) ≥ g(x) on [a, b] then ∫ₐᵇ f(x)dx ≥ ∫ₐᵇ g(x)dx — if one function is greater than another over an interval, its integral is also greater; (9) if m ≤ f(x) ≤ M on [a, b], then m(b − a) ≤ ∫ₐᵇ f(x) ≤ M(b − a). *(Slide 10; Slide 11; Slide 12)*

**Key points:**

- Swapping the limits flips the sign; equal limits give zero.
- The integral of a constant c over [a, b] is c(b − a).
- Integration is linear: sums split up, and constants can be pulled outside.
- Adjacent intervals can be joined: ∫ₐᶜ + ∫_cᵇ = ∫ₐᵇ.
- Order is preserved: f ≥ 0 gives a non-negative integral; f ≥ g gives a larger integral.
- Property 9 bounds the integral between m(b − a) and M(b − a).

**Examples:**

- Property 3: the area under the constant function c between a and b is just the rectangle c·(b − a).

> [!note] Interpretation (not stated directly in the sources)
> My reading of property 9: since f never goes below m and never above M, its area must lie between the areas of the two rectangles with heights m and M on the same base (b − a). The slide states the inequality without giving this graphical explanation.

## 10. Example: the half circle

Slide 13 shows that integrals can sometimes be found by recognising a shape. It starts from the equation of a circle, (x − x₀)² + (y − y₀)² = r², and takes the particular circle (x − 2)² + (y − 0)² = 2², i.e. centre (2, 0) and radius 2. Expanding gives (x² − 4x + 4) + y² = 4, so y² = 4x − x², and therefore y = ±√(4x − x²) = ±√(4 − (x − 2)²).

Taking the positive square root gives the upper half of the circle. The circle crosses the x-axis at x = 0 and x = 4, so the slide concludes that ∫ from 0 to 4 of √(4 − (x − 2)²) is the area of a half circle = ½·π·2² = 2π. The point is that we knew the answer from geometry before knowing any integration rules. *(Slide 13)*

**Key points:**

- Circle equation: (x − x₀)² + (y − y₀)² = r², centre (x₀, y₀), radius r.
- The chosen circle has centre (2, 0) and radius 2; the positive root y = +√(4 − (x − 2)²) is the top half.
- ∫₀⁴ √(4 − (x − 2)²) dx = ½πr² = 2π.

**Examples:**

- ∫₀⁴ √(4 − (x − 2)²) dx = 2π (area of a semicircle of radius 2).

## 11. The Fundamental Theorem of Calculus

Slide 14 gives the key result that connects differentiation and integration. Let f(x) be an integrable function. The antiderivative of f(x) is a function F(x) satisfying F(x) = ∫f(x)dx, which is equivalent to F′(x) = f(x). So an antiderivative is a function whose derivative gives you back f. The slide stresses that the antiderivative is not unique, because [F(x) + c]′ = f(x): adding any constant does not change the derivative.

We can use the Fundamental Theorem of Calculus to evaluate definite integrals, whenever a closed form of the antiderivative exists: ∫ₐᵇ f(x)dx = F(x)|ₐᵇ = F(b) − F(a). In words from the slide: if we want the area under the graph of f(x) between a and b, we integrate it to produce F(x), and then calculate F(b) − F(a).

Finally the slide defines the indefinite integral: ∫f(x)dx = F(x) + C when F′(x) = f(x), where C is a constant. So a definite integral is a number (an area), while an indefinite integral is a family of functions differing by a constant. *(Slide 14)*

**Key points:**

- F is an antiderivative of f when F′(x) = f(x).
- Antiderivatives are not unique: F(x) + c works for any constant c.
- ∫ₐᵇ f(x)dx = F(b) − F(a) — this replaces the rectangle limits with simple arithmetic.
- Indefinite integral: ∫f(x)dx = F(x) + C (a function plus a constant).
- Definite integral = a number; indefinite integral = a function family.

> [!note] Interpretation (not stated directly in the sources)
> A practical note (mine): the constant C cancels out in F(b) − F(a), which is why you can ignore it when evaluating a definite integral but must write it for an indefinite one. The slides imply this but do not say it directly.

## 12. Example: checking the theorem against a triangle

Slide 15 tests the theorem on a case we can check by elementary geometry. Suppose F(x) = ½x². Then f(x) = F′(x) = x, so F is an antiderivative of f. The Fundamental Theorem says the area under the curve f(x) = x from 0 to b is ∫₀ᵇ f(x)dx = F(b) − F(0) = ½b² − ½·0² = ½b².

The region under the line y = x between 0 and b is a right-angled triangle with base b and height b. Using the formula A = ½·base·height we also get ½b². So ∫₀ᵇ x dx = ½b², and the calculus answer agrees with the geometry (Slide 15). *(Slide 15)*

**Key points:**

- F(x) = ½x² is an antiderivative of f(x) = x.
- ∫₀ᵇ x dx = F(b) − F(0) = ½b².
- The same result comes from the triangle area formula ½·base·height, confirming the theorem.

**Examples:**

- ∫₀ᵇ x dx = ½b² = area of a triangle with base b and height b.

## 13. Standard integration rules to memorise

Slide 16 says that evaluating definite integrals is, in essence, the task of finding antiderivatives, and warns that this is not as straightforward as differentiation. Then it gives the basic rules. The Anti-Power Rule: ∫ₐᵇ xⁿ dx = [1/(n+1) · x^(n+1)] evaluated from a to b — so you raise the power by one and divide by the new power (the reverse of the power rule for derivatives). The integral of a constant: ∫ₐᵇ c dx = cx|ₐᵇ.

Slide 17 adds three more, with the instruction 'remember all these': ∫ₐᵇ (1/x)dx = ln x|ₐᵇ; ∫ₐᵇ e^(nx) dx = [(1/n)e^(nx)]|ₐᵇ; and ∫ₐᵇ nˣ dx = [(1/ln n)·nˣ]|ₐᵇ, valid for n > 0 and n ≠ 1. *(Slide 16; Slide 17)*

**Key points:**

- Finding an antiderivative is the core difficulty of integration, and it is harder than differentiating.
- Anti-power rule: ∫xⁿdx = x^(n+1)/(n+1).
- ∫c dx = cx.
- ∫(1/x)dx = ln x.
- ∫e^(nx)dx = (1/n)e^(nx).
- ∫nˣdx = nˣ/ln n, for n > 0, n ≠ 1.

> [!note] Interpretation (not stated directly in the sources)
> Two cautions from standard calculus, not stated on the slides: the anti-power rule fails for n = −1 (that is exactly the case covered by the ln rule), and the ln rule is usually written ln|x|, so it is only safe as written when the interval [a, b] lies in the positive numbers.

## 14. Worked examples of definite integrals

Slide 18 applies the rules. First, ∫₂⁵ (3x² + 2x + 1)dx is split using the sum property into ∫₂⁵3x²dx + ∫₂⁵2xdx + ∫₂⁵1dx. Each piece is integrated with the anti-power rule: 3x² gives x³, 2x gives x², and 1 gives x. Evaluating at the limits: [5³ − 2³] + [5² − 2²] + [5 − 2] = (125 − 8) + (25 − 4) + 3 = 141.

Second, ∫₂⁵ e^(2x)dx = [½e^(2x)] from 2 to 5 = ½e¹⁰ − ½e⁴, which the slide factorises as ½e⁴(e⁶ − 1). Third, ∫₁⁴ (1/x)dx = ln x|₁⁴ = ln 4 − ln 1. (Since ln 1 = 0, this is just ln 4.) *(Slide 18)*

**Key points:**

- Break a polynomial into separate integrals using the sum and constant-multiple properties.
- Integrate each power term, then substitute the upper and lower limits and subtract.
- ∫₂⁵(3x² + 2x + 1)dx = 141.
- ∫₂⁵e^(2x)dx = ½e¹⁰ − ½e⁴ = ½e⁴(e⁶ − 1).
- ∫₁⁴(1/x)dx = ln 4 − ln 1.

**Examples:**

- ∫₂⁵(3x² + 2x + 1)dx = [x³ + x² + x]₂⁵ = 141.
- ∫₂⁵e^(2x)dx = ½e⁴(e⁶ − 1).
- ∫₁⁴(1/x)dx = ln 4 − ln 1 = ln 4.

> [!note] Interpretation (not stated directly in the sources)
> The simplification ln 1 = 0 (so the answer is simply ln 4) is standard background; the slide leaves the answer as ln 4 − ln 1.

## 15. Application: the job problem (not examinable)

Slides 19–21 are marked 'For interest only – not examinable'. They start from the distance formula, distance = rate × time (for example 100 miles = 50 mph × 2 hours), and say this gives intuition for many problems: ask yourself what you are really doing.

The Job Problem: if Lenny can do a job in 6 hours and Carl can do the same job in 4 hours, how long does the job take if they work together? Lenny does 1/6 of the job per hour, Carl 1/4 per hour, so together 1/6 + 1/4 = 5/12 per hour. Here the 'job' plays the role of distance, so time = distance/rate = 1 ÷ (5/12) = 12/5 = 2 hours 24 minutes (Slides 19–20). This answer assumes both men work at a constant rate.

Slide 20 then drops that assumption: suppose Lenny works at rate L(x) = (12 − x)/54 and Carl at C(x) = (8 − x)/24, i.e. they get slower over time. These rates are chosen so that ∫₀⁶L(x)dx = 1 and ∫₀⁴C(x)dx = 1 — each still finishes his own job alone in 6 and 4 hours. The problem becomes: find T such that ∫₀ᵗ[L(x) + C(x)]dx = 1. Slide 21 multiplies through by 216 to clear the fractions, obtaining ∫₀ᵗ[(48 − 4x) + (72 − 9x)]dx = 216, i.e. ∫₀ᵗ[120 − 13x]dx = 216. Integrating and substituting the limits leads to the quadratic 13T² − 240T + 432 = 0, which the slide says is solved with the quadratic formula giving approximately 2 hours. *(Slide 19; Slide 20; Slide 21)*

**Key points:**

- Rates add: working together, you add the per-hour fractions of the job.
- With constant rates, together they finish in 12/5 hours = 2 h 24 min.
- If the rate changes over time, the work done is an integral of the rate function.
- The condition ∫₀⁶L dx = 1 means 'Lenny completes exactly one job in 6 hours'.
- Solving ∫₀ᵗ[L + C]dx = 1 gives 13T² − 240T + 432 = 0, with answer about 2 hours.
- This whole topic is marked not examinable.

**Examples:**

- Constant rates: 1/6 + 1/4 = 5/12 per hour → T = 12/5 h.
- Variable rates: L(x) = (12 − x)/54, C(x) = (8 − x)/24 → T ≈ 2 hours.

> [!note] Interpretation (not stated directly in the sources)
> My own check: ∫₀ᵗ(120 − 13x)dx = 120T − 13T²/2, and setting this equal to 216 and multiplying by 2 does give 13T² − 240T + 432 = 0, whose smaller root is about 2.02 hours. This supports the slide's 'approx. 2h', and it also explains the stray '2' characters that appear in the slide text — they are the denominators of fractions that the file did not display properly. The general lesson (mine): an integral is the natural tool when a rate is not constant.

## 16. Integration by parts (not examinable)

Slide 22 presents integration by parts as 'the product rule backwards'. Let f(x) and g(x) be continuous, integrable functions with F′(x) = f(x) and G′(x) = g(x). The product rule says d[F(x)G(x)]/dx = f(x)G(x) + F(x)g(x). Integrating both sides gives F(x)G(x) = ∫f(x)G(x)dx + ∫F(x)g(x)dx, and rearranging gives the formula: ∫F(x)g(x)dx = F(x)G(x) − ∫f(x)G(x)dx. The key idea stated on the slide is to choose F(x) and g(x) so that the remaining integral ∫f(x)G(x)dx is easy to compute.

Slide 23 gives two indefinite examples. Example 1: ∫xe^x dx with F(x) = x, G(x) = e^x, f(x) = 1, g(x) = e^x, giving xe^x − ∫1·e^x dx = xe^x − e^x + C. Example 2: ∫ln(1 + x)dx with F(x) = ln(1 + x), G(x) = 1 + x, f(x) = 1/(1 + x), g(x) = 1, giving ln(1 + x)(1 + x) − ∫(1 + x)·1/(1 + x)dx = (1 + x)ln(1 + x) − x + C.

Slide 24 adapts the formula to definite integrals: ∫ₐᵇ f(x)G(x)dx = F(b)G(b) − F(a)G(a) − ∫ₐᵇ F(x)g(x)dx. Slide 25 works through ∫₁³ x²ln(x)dx with F(x) = ln x, G(x) = ⅓x³, f(x) = 1/x, g(x) = x², obtaining 9ln(3) − 26/9. *(Slide 22; Slide 23; Slide 24; Slide 25)*

**Key points:**

- Integration by parts comes from reversing the product rule.
- Formula: ∫F(x)g(x)dx = F(x)G(x) − ∫f(x)G(x)dx.
- Choose the parts so that the new integral is simpler than the original.
- Definite version: ∫ₐᵇ f(x)G(x)dx = F(b)G(b) − F(a)G(a) − ∫ₐᵇ F(x)g(x)dx.
- Marked not examinable.

**Examples:**

- ∫xe^x dx = xe^x − e^x + C.
- ∫ln(1 + x)dx = (1 + x)ln(1 + x) − x + C.
- ∫₁³x²ln(x)dx = 9ln 3 − 26/9.

> [!note] Interpretation (not stated directly in the sources)
> Note (mine): in Example 2 the choice G(x) = 1 + x rather than G(x) = x is a deliberate trick — any antiderivative of g = 1 is allowed, and this one cancels neatly with f(x) = 1/(1 + x). In Slide 25 the definite formula is used with the roles arranged so that the log is differentiated and x² is integrated; this is the standard choice because ln x becomes the simpler 1/x.

## 17. Integration by substitution (not examinable)

Slide 26 introduces the second technique with a neat contrast: integration by parts is the product rule backwards, while integration by substitution is the chain rule backwards. Let F(x) = ∫f(x)dx and x = g(u). The chain rule gives dF[g(u)]/du = F′(g(u))g′(u) = f(g(u))g′(u). Integrating both sides with respect to u gives F(g(u)) = ∫f(g(u))g′(u)du. So the rule is: if f(x) is integrable and g(x) is invertible and continuously differentiable, the substitution x = g(u) changes the integration variable from x to u as ∫f(x)dx = ∫f(g(u))g′(u)du.

Slide 27 gives two examples. Example 1: ∫e^(√x)/√x. Let u = √x, so x = u² and dx = 2u du; the integral becomes ∫(e^u/u)·2u du = 2∫e^u du = 2e^u + C = 2e^(√x) + C (for x > 0). Example 2: ∫(e^x + e^(−x))/(e^x − e^(−x))dx. Let u = e^x − e^(−x), so du = (e^x + e^(−x))dx; the integral becomes ∫(1/u)du = ln u + C = ln(e^x − e^(−x)) + C.

Slide 28 handles definite integrals: the limits must also be converted, giving ∫(x=a to x=b) f(x)dx = ∫(u = g⁻¹(a) to u = g⁻¹(b)) f(g(u))g′(u)du; the slide verifies with the Fundamental Theorem that this still equals F(b) − F(a). Slide 29 is a worked example: ∫₋₁⁰ x²(x³ − 1)⁴dx with u = x³ − 1 and du = 3x²dx. The x-limits −1 and 0 become u-limits −2 and −1, and the answer is ⅓·⅕[u⁵] from −2 to −1 = 31/15. *(Slide 26; Slide 27; Slide 28; Slide 29)*

**Key points:**

- Substitution reverses the chain rule.
- Rule: ∫f(x)dx = ∫f(g(u))g′(u)du with x = g(u), where g is invertible and continuously differentiable.
- For definite integrals you must also change the limits from x-values to the corresponding u-values.
- Choose the substitution so that the messy inner part becomes the new variable u.
- Marked not examinable.

**Examples:**

- ∫e^(√x)/√x dx with u = √x → 2e^(√x) + C.
- ∫(e^x + e^(−x))/(e^x − e^(−x))dx with u = e^x − e^(−x) → ln(e^x − e^(−x)) + C.
- ∫₋₁⁰ x²(x³ − 1)⁴dx with u = x³ − 1 → 31/15.

> [!note] Interpretation (not stated directly in the sources)
> Pattern to look for (mine): substitution works when the integrand already contains the derivative of the inner function as a factor — in Example 2 the numerator is exactly du/dx, and on Slide 29 the factor x² is (up to the constant ⅓) the derivative of x³ − 1. I also note that ⅓ of ⅕[(−1)⁵ − (−2)⁵] = (1/15)(−1 + 32) = 31/15, which matches the slide.

## How the ideas connect

- Functions of two variables (Slide 3) are the reason partial derivatives are needed at all (Slide 4): with two inputs there are two independent directions of change.
- First-order partial derivatives (Slide 4–5) are the input for second-order partial derivatives (Slide 6), which are simply the same procedure applied twice.
- The finance motivation on Slide 7 is a direct use of the definition on Slide 4: 'hold everything else constant' is exactly what a hedging sensitivity measures.
- The rectangle approximation (Slide 8) defines the definite integral (Slide 9); the properties on Slides 10–12 are then just statements about areas.
- The half-circle (Slide 13) and triangle (Slide 15) examples link integrals back to familiar geometry and act as checks on the Fundamental Theorem.
- The Fundamental Theorem (Slide 14) is the bridge between the two halves of the lecture: integration is undone by differentiation, so knowing derivative rules gives you integration rules (Slides 16–17).
- Integration by parts (Slide 22) and by substitution (Slide 26) are the product rule and the chain rule read backwards, so differentiation techniques map one-to-one onto integration techniques.
- The job problem (Slides 19–21) connects the integral to the idea of a rate: when a rate is constant you multiply, when it varies you integrate.

## ⚠️ Unclear or conflicting in the sources

- The task mentions combining slides and a recording, but no transcript or timestamps were provided in the source — only the slide text. So nothing here comes from the lecturer's spoken words, and any emphasis or extra explanation given in the lecture is missing.
- Slide 4 writes the one-variable derivatives as dz/dx = 3x² and dz/dy = 4y before introducing the ∂ symbol. Strictly these should be partial derivatives (∂z/∂x, ∂z/∂y); the mixed notation may be a slide simplification or a typographical issue.
- Slide 6 states that the two mixed second-order partials are equal in the example, but does not say under what conditions this is true in general, and does not name the theorem.
- Slide 10, property (4): the slide explains ∫[f + g] = ∫f + ∫g as 'adding together two adjacent areas under the same curve'. That description actually fits property (6) on Slide 11; property (4) is about adding two different functions over the same interval. This looks like an error or a mixed-up caption.
- Slide 12, property (9) is given with no explanation and the integral is written '∫ₐᵇ f(x)' without dx.
- Several integrals in the source are missing the 'dx' (for example on Slide 13 and in Slide 27, Example 1) — presumably formatting loss rather than a mathematical point.
- Slide 17 writes ∫(1/x)dx = ln x without the absolute value (ln|x|) and without stating that the interval must avoid x = 0; Slide 16's anti-power rule also does not exclude the case n = −1.
- Slide 21 contains stray '2' characters and is hard to read; the step from ∫₀ᵗ(120 − 13x)dx = 216 to 13T² − 240T + 432 = 0 requires the term 13T²/2, which is not clearly visible in the text. The final root is only given as 'approx. 2h' with no exact value.
- Slide 29 contains an extra '=' sign inside the integral ('∫₋₁⁰ = x²(x³ − 1)⁴dx'), which appears to be a typo.
- Slide 8 refers to upper and lower sums U(Pn, f) and L(Pn, f) but does not define precisely how the rectangle heights are chosen; the slides also describe diagrams that are not reproduced in the text.
- The Cobb–Douglas function on Slide 3 is introduced but no partial derivative of it is actually computed, so its link to the later examples is left implicit.
- The slides say Slides 19–29 are 'not examinable', but it is not stated whether these techniques will be needed in later lectures of the module.

## Recap

1. A function of two variables, z = f(x, y), gives one output for each point (x, y); the Cobb–Douglas function F(x, y) = A·x^a·y^b is a standard economic example (Slide 3).
2. A partial derivative differentiates with respect to one variable while holding the other constant: ∂z/∂x holds y fixed and ∂z/∂y holds x fixed (Slide 4).
3. Differentiating the first-order partials again gives four second-order partials, and in the slide's example the two mixed ones are equal (Slide 6).
4. Partial derivatives of the Black–Scholes formula with respect to time, interest rate, volatility and the underlying price give the sensitivities traders use to hedge (Slide 7).
5. The definite integral ∫ₐᵇ f(x)dx is defined as the common limit of lower and upper rectangle sums and is interpreted as the area under the curve (Slides 8–9).
6. Integrals are linear and additive over adjacent intervals, preserve inequalities, and are zero when the limits are equal (Slides 10–12).
7. The Fundamental Theorem of Calculus says that if F′(x) = f(x), then ∫ₐᵇ f(x)dx = F(b) − F(a), which turns area-finding into finding an antiderivative (Slide 14).
8. You must memorise the basic antiderivatives: ∫xⁿdx = x^(n+1)/(n+1), ∫c dx = cx, ∫(1/x)dx = ln x, ∫e^(nx)dx = (1/n)e^(nx), ∫nˣdx = nˣ/ln n (Slides 16–17).
9. Integration by parts (product rule backwards) and integration by substitution (chain rule backwards) are presented as interesting but explicitly not examinable (Slides 22, 26).
