---
type: lecture-explanation
module: IC104 - Math
lecture: "[[IC104 L02 — Differentiation, Derivatives and Single-Variable Optimisation]]"
generated: 2026-10-12
model: claude-opus-5
sources: slides
---

# IC104 L02 — Explanation

> [!info] Пошаговое объяснение (сгенерировано). Лекция: [[IC104 L02 — Differentiation, Derivatives and Single-Variable Optimisation]]. Ссылки *(Slide N; MM:SS)* ведут к источнику — сверяйся с ними.

## Overview

This lecture introduces differentiation: how to measure the slope (rate of change) of a function, not only for straight lines but also for curves. It builds the derivative step by step from the idea of a tangent line and a limit, gives the standard rules for differentiating (power, sum, product, quotient, chain, exponential, logarithm, implicit), and then uses the first and second derivative to find maximum and minimum points. The last part applies all of this to business problems: minimum average cost, marginal cost, maximum total revenue and profit maximisation (Slides 2, 26, 32-40).

## 1. What the lecture covers

The lecture has three blocks, each following a chapter of the textbook Sydsaeter & Hammond: Differentiation (Chapter 6), Derivatives in Use (Chapter 7) and Single-Variable Optimisation (Chapter 8). "Single-variable" means the functions have only one input variable, usually x or q (quantity).

So the logic of the lecture is: first learn what a derivative *is*, then learn *how to compute* it quickly with rules, then learn *what to use it for* (finding highest and lowest points of economic functions). *(Slide 1; Slide 2)*

**Key points:**

- Three parts: Differentiation, Derivatives in Use, Single-Variable Optimisation
- Based on Sydsaeter & Hammond Chapters 6, 7 and 8
- Everything is about functions of one variable

> [!note] Interpretation (not stated directly in the sources)
> Knowing the three-block structure helps when you revise: the rules part is mostly practice, while the optimisation part is where exam questions about firms and profit usually come from.

## 2. Starting point: the slope of a straight line

The lecture starts with the linear function y = ax + b. For a straight line the slope (also called the gradient) is the ratio of the change in y to the change in x:

slope = (y₁ − y₀) / (x₁ − x₀) = Δy / Δx = change in y / change in x.

The symbol Δ (delta) just means "change in". This ratio tells you how much y changes when x changes by one unit, and the lecture calls this the **rate of change in y**. For a straight line this number is always the same, whatever two points you choose. *(Slide 3)*

**Key points:**

- Slope = Δy/Δx = (y₁ − y₀)/(x₁ − x₀)
- Δ means "change in"
- The slope is the rate of change of y per unit change in x
- For a linear function y = ax + b the slope is constant

**Examples:**

- In y = ax + b with a and b positive, the graph is an upward-sloping straight line (Slide 3).

> [!note] Interpretation (not stated directly in the sources)
> In y = ax + b the slope is simply the coefficient a, and b is the value of y when x = 0. The slides do not say this explicitly here, but it is the standard reading of the linear form.

## 3. The problem with curves: the tangent line

Now take a curve, for example y = x² + 4. The important feature is that the slope of a curve **keeps changing**: as x increases and we move up the curve, the curve gets steeper. So one single number cannot describe the slope of the whole curve.

If we use the old formula (y₁ − y₀)/(x₁ − x₀) with two points P and Q on the curve, we do not get the slope of the curve. We get the slope of the straight line that joins P and Q. To get the slope *at one single point*, we draw a **tangent**: a line that touches the curve at only one point. The slope of the tangent at P is the slope of the function at P, and this tangent is unique — a line with a bigger or smaller slope would cut the curve somewhere else.

The key idea on Slide 6 is the "moving" argument: if we move point Q closer and closer to point P, the line PQ becomes closer and closer to the tangent line AB. *(Slide 4; Slide 5; Slide 6)*

**Key points:**

- The slope of a curve is different at every point
- (y₁−y₀)/(x₁−x₀) gives the slope of the straight line (chord) through P and Q, not of the curve
- A tangent touches the curve at one point only; its slope is the slope of the curve at that point
- Moving Q towards P makes line PQ approach the tangent AB

**Examples:**

- The curve y = x² + 4, with points P and Q on it and tangent line AB at P (Slides 4-6).

## 4. Deriving the slope of y = x² + 4 algebraically

Slide 7 turns that picture into algebra. P and Q are both on the curve, so y₀ = x₀² + 4 and y₁ = x₁² + 4. Because Δx = x₁ − x₀, we can write x₁ = x₀ + Δx and substitute:

Δy = [(x₀ + Δx)² + 4] − [x₀² + 4] = x₀² + 2x₀Δx + Δx² + 4 − x₀² − 4 = 2x₀Δx + Δx².

Dividing by Δx gives Δy/Δx = (2x₀Δx + Δx²)/Δx = 2x₀ + Δx.

So the slope of the line PQ is 2x₀ + Δx. Now make Δx smaller and smaller (Q moves towards P): the term Δx disappears and we are left with 2x₀. In symbols: lim(Δx→0) Δy/Δx = 2x₀. This limit is exactly the slope of the tangent at P. *(Slide 7)*

**Key points:**

- Substitute x₁ = x₀ + Δx to express everything with Δx
- For y = x² + 4: Δy/Δx = 2x₀ + Δx
- Taking the limit as Δx → 0 removes Δx and leaves 2x₀
- The limit of Δy/Δx is the slope of the tangent

**Examples:**

- y = x² + 4 ⇒ slope at x₀ is 2x₀ (Slide 7).

> [!note] Interpretation (not stated directly in the sources)
> The constant +4 disappears in the subtraction, which is a first hint of a rule that comes later: additive constants do not affect the derivative (Slide 13).

## 5. Definition of the derivative and the tangent line equation

Slide 8 gives the formal definitions. The limit of Δy/Δx is written dy/dx, and it is the slope of the tangent at the point P:

lim(Δx→0) Δy/Δx = dy/dx.

At a specific point x = a we write f′(a) = dy/dx |ₓ₌ₐ, which is the slope of the tangent to the curve y = f(x) at the point (a, f(a)). The **derivative** of f at a is defined with the limit

f′(a) = lim(h→0) [f(a + h) − f(a)] / h,

where h plays the same role as Δx. Finally, the straight line that is tangent to the curve at (a, f(a)) has the equation

y − f(a) = f′(a)(x − a). *(Slide 8)*

**Key points:**

- dy/dx and f′(x) are two notations for the derivative
- f′(a) = lim(h→0) [f(a+h) − f(a)]/h
- f′(a) is the slope of the tangent at the point (a, f(a))
- Tangent line: y − f(a) = f′(a)(x − a)

> [!note] Interpretation (not stated directly in the sources)
> The tangent-line formula is the point-slope form of a straight line: you know one point (a, f(a)) and the slope f′(a). The slides state the formula but do not explain this link.

## 6. Worked example from first principles: f(x) = x³

Slide 9 uses the limit definition for f(x) = x³. First expand f(a + h) = (a + h)³ = a³ + 3a²h + 3ah² + h³. Subtract f(a) = a³: the a³ terms cancel, leaving f(a+h) − f(a) = 3a²h + 3ah² + h³. Divide by h: 3a² + 3ah + h².

As h goes to zero, every term that still contains h disappears, so f′(a) = 3a². This matches the power rule you meet on Slide 13 (x³ ⇒ 3x²), but here it is proved from the definition. *(Slide 9)*

**Key points:**

- Expand f(a+h), subtract f(a), divide by h, then let h → 0
- f(x) = x³ ⇒ f′(a) = 3a²
- Terms containing h vanish in the limit

**Examples:**

- f(x) = x³: [f(a+h) − f(a)]/h = 3a² + 3ah + h² → 3a² (Slide 9).

## 7. What the sign of the derivative tells you

The derivative is useful because its sign shows the direction of the function on an interval I:

- f′(x) ≥ 0 (or > 0) on I ⟺ f is increasing (strictly increasing) on I — the graph slopes upwards.
- f′(x) ≤ 0 (or < 0) on I ⟺ f is decreasing (strictly decreasing) on I — the graph slopes downwards.
- f′(x) = 0 on I ⟺ f is constant on I — the graph is flat.

These statements are given as equivalences ("⟺"), so you can go in both directions: from the sign of the derivative to the shape of the graph, and from the shape back to the sign. *(Slide 10; Slide 11)*

**Key points:**

- Positive derivative = rising graph
- Negative derivative = falling graph
- Zero derivative on a whole interval = flat (constant) function
- "Strictly" increasing/decreasing goes with the strict inequalities > and <

**Examples:**

- Slide 11 shows this with a graph (no numbers given in the text).

> [!note] Interpretation (not stated directly in the sources)
> This is the bridge to the optimisation part: if the function rises before a point and falls after it, that point must be a top (maximum).

## 8. Economic meaning: rates of change and marginal quantities

Slide 12 explains how economists read a derivative. The **instantaneous rate of change** of f at a is f′(a). The **relative rate of change** at a is f′(a)/f(a) — the change compared with the level of the function.

Two examples are given. First, if K(t) is the capital stock of an economy at time t, then K′(t) is the rate of investment, usually written I(t), so K′(t) = I(t). Second, if C(x) is the cost of producing x units, then C′(x) is the **marginal cost** at x: the cost of producing one more unit at that point, defined as C′(x) = lim(h→0) [C(x+h) − C(x)]/h. *(Slide 12)*

**Key points:**

- Instantaneous rate of change = f′(a)
- Relative rate of change = f′(a)/f(a)
- K′(t) = I(t): the derivative of capital stock is investment
- C′(x) = marginal cost = cost of one extra unit

**Examples:**

- Capital stock K(t) and investment I(t)
- Cost function C(x) and marginal cost C′(x)

> [!note] Interpretation (not stated directly in the sources)
> The relative rate of change is close to the idea of a growth rate (often expressed in %), which is why it is popular in finance. The slide gives the formula but not this reading.

## 9. Basic rules: power rule and constants

Finding a derivative by the limit definition every time is slow, so we use rules. The process of finding a derivative is called **differentiation** (Slide 13).

Power rule, where a is any constant: f(x) = xᵃ ⇒ f′(x) = a·xᵃ⁻¹. You multiply by the old power and reduce the power by one.

Constants: a constant function f(x) = A has f′(x) = 0. An **additive** constant disappears: y = A + f(x) ⇒ y′ = f′(x). A **multiplicative** constant stays: y = A·f(x) ⇒ y′ = A·f′(x). *(Slide 13)*

**Key points:**

- Differentiation = the process of finding a derivative
- Power rule: xᵃ ⇒ a·xᵃ⁻¹
- Derivative of a constant is 0
- Added constants vanish; multiplying constants are kept

**Examples:**

- y = x² ⇒ y′ = 2x
- y = x⁻² ⇒ y′ = −2x⁻³
- y = x ⇒ y′ = 1·x⁰ = 1
- y = 3x⁴ − 4 ⇒ y′ = 12x³

## 10. Sums and differences, and marginal profit

If F(x) = f(x) ± g(x), then F′(x) = f′(x) ± g′(x). In words: when functions are added (or subtracted), you simply add (or subtract) their derivatives.

The lecture applies this to the profit function π(x) = R(x) − C(x) with R(x) = 3x² and C(x) = 12x. The **marginal profit** is π′(x) = R′(x) − C′(x) = 6x − 12. *(Slide 14)*

**Key points:**

- Derivative of a sum is the sum of the derivatives
- Same rule for differences
- Profit = revenue − cost, so marginal profit = marginal revenue − marginal cost

**Examples:**

- π(x) = 3x² − 12x ⇒ π′(x) = 6x − 12 (Slide 14).

> [!note] Interpretation (not stated directly in the sources)
> Note that π′(x) = 0 when x = 2 in this example; this is the kind of calculation that reappears in the profit-maximisation section (Slide 40). The slide itself does not take this step.

## 11. The product rule

For a product of two functions, F(x) = f(x)·g(x), the derivative is

F′(x) = f′(x)·g(x) + f(x)·g′(x).

The slide describes it in words: keep one function the same and differentiate the other, then differentiate the first and keep the second the same, and add the two results.

The rule extends to more than two factors: for F(x) = f₁(x)·f₂(x)·…·fₙ(x) you differentiate one factor at a time, keep all the others unchanged, and add up all these terms. *(Slide 15)*

**Key points:**

- (f·g)′ = f′g + f g′
- You get one term for each factor you differentiate
- The rule generalises to n factors

**Examples:**

- y = (1 − x²)(2x − 4): f = 1 − x², f′ = −2x, g = 2x − 4, g′ = 2 ⇒ y′ = (−2x)(2x − 4) + 2(1 − x²) = −4x² + 8x + 2 − 2x² = −6x² + 8x + 2 (Slide 15).

## 12. The quotient rule

For a fraction of two functions, F(x) = f(x)/g(x), the derivative is

F′(x) = [f′(x)·g(x) − f(x)·g′(x)] / (g(x))².

Be careful with the order: it is "derivative of the top times the bottom **minus** top times derivative of the bottom", all divided by the bottom squared. Unlike the product rule, the order matters because of the minus sign. *(Slide 16)*

**Key points:**

- (f/g)′ = (f′g − f g′)/g²
- The denominator is squared
- The minus sign means the order of the two terms matters

**Examples:**

- F(x) = 2x/(1 + x²): f = 2x, g = 1 + x² ⇒ F′ = [2(1 + x²) − 2x·2x]/(1 + x²)² = (−2x² + 2)/(1 + x²)² (Slide 16).

## 13. The chain rule (function of a function)

The chain rule is for a function inside another function (a composite function). If F(x) = f(g(x)) and both functions can be differentiated, then

F′(x) = f′(g(x))·g′(x).

In words: first differentiate the **outer** function, keeping the inner function unchanged, then multiply by the derivative of the **inner** function. With the alternative notation u = g(x) and y = f(u), the same rule is written

dy/dx = (dy/du)·(du/dx).

The practical method shown on Slides 18-20 is always the same: (1) identify the inner function u and the outer function; (2) differentiate the inner function; (3) apply the rule. *(Slide 16; Slide 17; Slide 18; Slide 19; Slide 20)*

**Key points:**

- Chain rule: F′ = f′(g(x))·g′(x)
- Equivalent form: dy/dx = dy/du · du/dx
- Three steps: identify inner/outer, differentiate the inner, multiply
- The chain rule can be combined with other rules (e.g. the quotient rule)

**Examples:**

- y = (2x² + 4x)²: u = 2x² + 4x ⇒ dy/dx = 2u·(4x + 4) = 2(2x² + 4x)(4x + 4) (Slide 16)
- y = (x³ + x²)⁵⁰: u = x³ + x², u′ = 3x² + 2x ⇒ y′ = 50(x³ + x²)⁴⁹(3x² + 2x) (Slide 18)
- y = √(x² + 1) = u^(1/2) with u = x² + 1 ⇒ y′ = ½(x² + 1)^(−1/2)·2x = x/√(x² + 1) (Slide 19)
- y = ((x − 1)/(x + 3))^(1/3): u′ = [1(x+3) − (x−1)1]/(x+3)² = 4/(x+3)² ⇒ y′ = ⅓((x−1)/(x+3))^(−2/3)·4/(x+3)² (Slide 20)

> [!note] Interpretation (not stated directly in the sources)
> Writing a square root as a power ^(1/2) (Slide 19) is a useful habit, because then you can use the power rule for roots as well.

## 14. Higher-order derivatives

The derivative f′(x) is itself a function, so it can be differentiated again. The result (f′)′(x) = f″(x) is the **second derivative**. The slide writes the notations f′ = dy/dx and f″ = d²y/d²x.

There is no reason to stop at two: as long as the previous derivative can be differentiated, you can continue, and the nth-order derivative is written y⁽ⁿ⁾ = f⁽ⁿ⁾(x) or dⁿy/dⁿx. *(Slide 21)*

**Key points:**

- f′ = first derivative, f″ = second derivative (the derivative of the derivative)
- You can continue to nth-order derivatives
- Notations: f″, d²y/d²x, f⁽ⁿ⁾(x)

**Examples:**

- f(x) = 2x⁵ − 3x³ + 2x ⇒ f′ = 10x⁴ − 9x² + 2 and f″ = 40x³ − 18x (Slide 21).

> [!note] Interpretation (not stated directly in the sources)
> The usual textbook notation for the second derivative is d²y/dx², not d²y/d²x; the slides consistently write the version with d²q or d²x in the denominator. This looks like a typing/formatting issue rather than a different concept.

## 15. Convex and concave functions

The second derivative describes how the *slope* changes, which gives the curvature of the graph:

- f″(x) > 0 on an interval I ⟺ f′ is increasing on I
- f″(x) < 0 on I ⟺ f′ is decreasing on I

From this the slide defines: f is **convex** on I ⟺ f″(x) ≥ 0 for all x in I, and f is **concave** on I ⟺ f″(x) ≤ 0 for all x in I. *(Slide 22)*

**Key points:**

- Second derivative tells you whether the slope is rising or falling
- Convex: f″ ≥ 0 (slope increasing)
- Concave: f″ ≤ 0 (slope decreasing)

> [!note] Interpretation (not stated directly in the sources)
> A common picture: a convex function has a 'cup' or U shape, a concave function an upside-down U shape. The slide gives only the inequalities, not this image.

## 16. Derivatives of exponential and logarithmic functions

Slide 23 lists the special rules you must memorise:

- y = eˣ ⇒ y′ = eˣ. The derivative of this exponential function is the function itself; the slide stresses that **only** this function has that property.
- y = aˣ: rewrite it as aˣ = (e^{ln a})ˣ = e^{(ln a)x}, which gives y′ = aˣ·ln a.
- y = ln x ⇒ y′ = 1/x.
- y = ln h(x) ⇒ y′ = h′(x)/h(x) (this is the chain rule applied to the logarithm). *(Slide 23)*

**Key points:**

- (eˣ)′ = eˣ
- (aˣ)′ = aˣ ln a, obtained by rewriting aˣ as e^{(ln a)x}
- (ln x)′ = 1/x
- (ln h(x))′ = h′(x)/h(x)

**Examples:**

- y = xᵖe^{ax} ⇒ y′ = p x^{p−1}e^{ax} + xᵖ a e^{ax} = x^{p−1}e^{ax}(p + ax) — product rule plus chain rule
- y = x·2^{3x} ⇒ y′ = 1·2^{3x} + x·3·2^{3x}ln2 = 2^{3x}(1 + 3x ln 2)
- y = ln(4 − x²) ⇒ y′ = −2x/(4 − x²) = 2x/(x² − 4)

> [!note] Interpretation (not stated directly in the sources)
> In the second example the slide text is rendered as "y = x23x"; from the worked derivative it must mean y = x·2^{3x}. I read the formula from the solution, which is the safest interpretation.

## 17. Implicit differentiation

Sometimes y is not given as an explicit formula y = f(x), but hidden inside an equation of the form g(x, y) = c. The method is:

1. Differentiate both sides of g(x, y(x)) = c with respect to x, treating y as a function of x (so every time you differentiate y you must use the chain rule and write y′).
2. Solve the resulting equation for y′.

In the example y³ + 3x²y = 13: differentiating gives 3y²y′ + 6xy + 3x²y′ = 0 (the first term by the chain rule, the second part by the product rule), and solving gives y′ = −6xy/(3x² + 3y²) = −2xy/(x² + y²). *(Slide 24)*

**Key points:**

- Used when the relation between x and y is given as an equation, not as y = f(x)
- Treat y as y(x) and apply the chain rule: (y³)′ = 3y²y′
- The right-hand side is a constant, so its derivative is 0
- Then solve algebraically for y′

**Examples:**

- y³ + 3x²y = 13 ⇒ y′ = −2xy/(x² + y²) (Slide 24).

## 18. Economic application of implicit differentiation: price and interest rate

Slide 25 asks a comparative-statics question: with a supply function S = A·P^(−α)·r^(−β), how does the equilibrium price react to an increase in the interest rate r? The slide says the supply of the commodity is a decreasing function of its price P and of the interest rate r, and that we need dP/dr.

Differentiating the supply relation implicitly and setting the result equal to zero gives

A(−αP^(−α−1))(dP/dr)·r^(−β) + A P^(−α)(−β r^(−β−1)) = 0.

Solving for dP/dr and simplifying leads to dP/dr = −P·β/(α·r) < 0. So the conclusion stated on the slide is that the (equilibrium) price falls when the interest rate rises. *(Slide 25)*

**Key points:**

- Comparative statics: use a derivative to see how one variable reacts to a change in another
- The derivative wanted is dP/dr
- Result: dP/dr = −Pβ/(αr), which is negative
- A negative derivative means P decreases when r increases

**Examples:**

- S = AP^(−α)r^(−β) ⇒ dP/dr = −Pβ/(αr) < 0 (Slide 25).

> [!note] Interpretation (not stated directly in the sources)
> The step where the derivative of the supply expression is set equal to zero only makes sense if the quantity supplied S is held constant (for example, at a fixed equilibrium quantity). The slide does not state this assumption, so I flag it below rather than treat it as given.

## 19. Finding maximum and minimum points: the main idea

The second half of the lecture uses derivatives to find the best point of a function — for example the point of maximum profitability, which is very often needed in finance and economics.

The key fact is: **at a maximum or a minimum point the slope of the function is zero**. So the procedure is: differentiate the function, set the derivative equal to zero, and solve for x (or q). That gives candidate points. Then you must check *which* kind of point it is — a maximum, a minimum, or a point of inflection — by looking at the second derivative.

Slide 27 gives a simple illustration: y = x² − 4x + 6 has slope y′ = 2x − 4, so the slope is negative for small x and positive for large x; a function can be decreasing for some values of x and increasing for others. *(Slide 26; Slide 27)*

**Key points:**

- At a maximum or minimum, the slope is zero
- Method: differentiate ⇒ set derivative = 0 ⇒ solve
- Use the second derivative to identify the type of point
- A point of inflection can also have a zero derivative

**Examples:**

- y = x² − 4x + 6 with y′ = 2x − 4 (Slide 27).

> [!note] Interpretation (not stated directly in the sources)
> For y = x² − 4x + 6, setting 2x − 4 = 0 gives x = 2 as the stationary point; the slide shows the derivative but does not solve it.

## 20. Definition of extreme points and the first-order condition

Formally (Slide 28): a point c in the domain D is a **maximum point** for f if f(c) ≥ f(x) for all x in D; a point d is a **minimum point** if f(d) ≤ f(x) for all x in D. So an extreme point is defined by comparing the function value there with all other values. For example x = 0 is a maximum point for f(x) = −x² and a minimum point for f(x) = x².

Slide 29 states the **necessary first-order condition**: the first derivative of a continuous function y = f(x) shows where the function increases, where it decreases, and where it reaches a **stationary point** (neither increasing nor decreasing). The condition f′(c) = 0 is *necessary* for c to be a maximum or minimum point. The slide also points out that a stationary point can instead be a **point of inflection** (labelled x₂ in the right-hand graph). *(Slide 28; Slide 29)*

**Key points:**

- Maximum point: f(c) ≥ f(x) for all x in the domain
- Minimum point: f(d) ≤ f(x) for all x in the domain
- Stationary point: f′ = 0, the function is neither rising nor falling
- f′(c) = 0 is necessary, but not sufficient, for an extreme point

**Examples:**

- x = 0 is a maximum for f(x) = −x² and a minimum for f(x) = x² (Slide 28).

> [!note] Interpretation (not stated directly in the sources)
> "Necessary but not sufficient" is exactly why the second-derivative check on the next slides exists: every max/min has zero slope, but not every point with zero slope is a max or min.

## 21. Second-order conditions: maximum for concave, minimum for convex

Slides 30 and 31 give the test that separates maxima from minima.

Maximum: if f′(x) ≥ 0 for x ≤ c and f′(x) ≤ 0 for x ≥ c, then x = c is a maximum point. The function rises up to c and then falls, so the graph of the first derivative is downward-sloping. Equivalently, if at c the first-order condition dy/dx = 0 holds and the second-order condition says the second derivative is negative, the point is a maximum.

Minimum: if f′(x) ≤ 0 for x ≤ c and f′(x) ≥ 0 for x ≥ c, then x = c is a minimum point. The function falls and then rises, so the graph of the first derivative is upward-sloping. Equivalently, dy/dx = 0 together with a positive second derivative means the point is a minimum. *(Slide 22; Slide 30; Slide 31)*

**Key points:**

- FOC (first-order condition): dy/dx = 0 locates the candidate point
- SOC (second-order condition): second derivative < 0 ⇒ maximum
- SOC: second derivative > 0 ⇒ minimum
- Maximum: slope goes from + to −; minimum: slope goes from − to +
- Links to Slide 22: maximum for concave functions, minimum for convex functions

> [!note] Interpretation (not stated directly in the sources)
> The slides write the second-order condition as d²y/dx < 0 and d²y/dx > 0; from the context (and Slide 22) this must mean the second derivative d²y/dx², as used correctly in the later numerical examples.

## 22. Application 1: cost function and minimum average cost

Slide 32 sets up a firm's total cost function TC = f(q) = 5q² + 2q + 500, where q is the number of production units. Here 500 is the **fixed cost** (it does not depend on q) and 5q² + 2q is the **variable cost**. **Average cost** is AC = TC/q.

To find the output with the lowest average cost (Slide 33), first write AC in a form that is easy to differentiate: AC = TC/q = 5q + 2 + 500q⁻¹. Then apply the first-order condition:

dAC/dq = 5 − 500q⁻² = 0 ⇒ 5q² = 500 ⇒ q = ±10.

The solution q = −10 is ignored because a negative output makes no economic sense. Finally check the second-order condition: d²AC/dq² = 1000/q³, and at q = 10 this is 1000/1000 = 1 > 0, which is positive, so q = 10 is indeed a **minimum**. *(Slide 32; Slide 33)*

**Key points:**

- TC = 5q² + 2q + 500; fixed cost 500, variable cost 5q² + 2q
- AC = TC/q = 5q + 2 + 500/q
- FOC: 5 − 500q⁻² = 0 gives q = ±10
- Reject q = −10 on economic grounds
- SOC: d²AC/dq² = 1000/q³ > 0 at q = 10 ⇒ minimum

**Examples:**

- Minimum average cost at q = 10 (Slides 32-33).

> [!note] Interpretation (not stated directly in the sources)
> Rewriting 500/q as 500q⁻¹ is the trick that lets you use the power rule instead of the quotient rule — a small but very practical step.

## 23. Application 2: marginal cost and its relation to average cost

Slide 34 defines marginal cost intuitively: if production increases by a small amount Δq, the extra cost per unit is ΔTC/Δq, and in the limit MC = lim(Δq→0) ΔTC/Δq = dTC/dq. So marginal cost is simply the derivative of total cost.

For TC = 5q² + 2q + 500 we get MC = 10q + 2. The slide explains that the marginal cost curve measures the **slope** of the total cost curve; it is upward-sloping because the slope of total cost increases as q increases. Also, the fixed cost does not affect MC (because the derivative of the constant 500 is zero).

Slide 36 connects the two curves. The minimum of AC is at q = 10, where AC = 102. For q > 10 the MC curve lies above the AC curve (MC > AC); for q < 10 it lies below (MC < AC). And exactly where MC = AC, average cost is at its minimum — the slide checks this algebraically: 10q + 2 = 5q + 2 + 500q⁻¹ ⇒ 10q² + 2q = 5q² + 2q + 500 ⇒ 5q² = 500 ⇒ q = ±10, the same answer as before. *(Slide 34; Slide 35; Slide 36)*

**Key points:**

- MC = dTC/dq, the limit of ΔTC/Δq
- For TC = 5q² + 2q + 500: MC = 10q + 2
- MC is the slope of the TC curve; fixed costs do not affect MC
- MC < AC left of q = 10, MC > AC right of q = 10
- AC is at its minimum exactly where MC = AC

**Examples:**

- At q = 10: AC = 5(10) + 2 + 500/10 = 102 and MC = 10(10) + 2 = 102, so MC = AC (Slides 35-36).

> [!note] Interpretation (not stated directly in the sources)
> The slides give AC = 102 at q = 10 without the arithmetic; I added the calculation 50 + 2 + 50 = 102 to show where the number comes from.

## 24. Application 3: demand, total revenue and marginal revenue

Slide 37 starts from a market demand function q = −4p + 260. Solving for p gives p = −q/4 + 65. Total revenue is price times quantity:

TR = p·q = (−q/4 + 65)q = −q²/4 + 65q.

Marginal revenue is defined in the same way as marginal cost, as a derivative: MR = dTR/dq = −q/2 + 65.

Slide 38 then maximises total revenue. FOC: dTR/dq = −2q/4 + 65 = 0 ⇒ q = 130. SOC: d²TR/dq² = −1/2 < 0, which is negative, so q = 130 really is a maximum. *(Slide 37; Slide 38)*

**Key points:**

- Invert the demand function to get p as a function of q
- TR = p·q
- MR = dTR/dq
- FOC gives q = 130; SOC = −1/2 < 0 confirms a maximum

**Examples:**

- q = −4p + 260 ⇒ p = −q/4 + 65 ⇒ TR = −q²/4 + 65q ⇒ MR = −q/2 + 65, maximum TR at q = 130 (Slides 37-38).

> [!note] Interpretation (not stated directly in the sources)
> In the TR line the slide shows "(−q/4 + 260)q" but then writes the result as −q²/4 + 65q, which matches p = −q/4 + 65. So the "260" there appears to be a typing error for 65; the rest of the calculation is consistent with 65.

## 25. Application 4: profit maximisation

The final example puts revenue and cost together. The given functions are TC = q² + 2q + 500, p = −2q + 200, so TR = p·q = −2q² + 200q (Slide 39).

Profit is total revenue minus total cost:

Π = TR − TC = −2q² + 200q − (q² + 2q + 500) = −3q² + 198q − 500.

FOC: dΠ/dq = −6q + 198 = 0 ⇒ q = 33. SOC: d²Π/dq² = −6 < 0, negative, so q = 33 is a maximum. The profit-maximising output is therefore 33 units. *(Slide 39; Slide 40)*

**Key points:**

- Π = TR − TC
- Π = −3q² + 198q − 500 for the given functions
- FOC: −6q + 198 = 0 ⇒ q = 33
- SOC: −6 < 0 ⇒ q = 33 is a maximum

**Examples:**

- TC = q² + 2q + 500, p = −2q + 200 ⇒ profit maximum at q = 33 (Slides 39-40).

> [!note] Interpretation (not stated directly in the sources)
> Note that the TC here (q² + 2q + 500) is not the same as the one used in the average-cost example (5q² + 2q + 500); it is a new, separate example. Also, by the sum/difference rule, dΠ/dq = 0 is the same as MR = MC, although the slides do not say this in the profit section.

## How the ideas connect

- The slope formula Δy/Δx for a straight line (Slide 3) becomes the derivative when we take the limit Δx → 0 for a curve (Slides 7-8).
- The limit definition of the derivative (Slide 8) is used to prove particular results such as f(x) = x³ ⇒ f′ = 3a² (Slide 9), which the power rule (Slide 13) then gives instantly.
- The sign of the first derivative (increasing/decreasing, Slide 10) is the basis of the first-order condition for maxima and minima (Slides 29-31).
- The second derivative (Slide 21) and convexity/concavity (Slide 22) give the second-order condition that distinguishes maxima from minima (Slides 30-31).
- Marginal cost and marginal revenue (Slides 12, 34, 37) are just derivatives of total cost and total revenue, so the economic 'marginal' language and the mathematical 'derivative' language mean the same thing.
- The chain rule (Slides 16-20) is what makes implicit differentiation possible, because y is treated as a function of x (Slide 24).
- Implicit differentiation is applied to economics in the supply/interest-rate example (Slide 25), where the sign of dP/dr answers an economic question.
- The same three-step optimisation recipe (differentiate, set to zero, check the second derivative) is used for minimum average cost (Slide 33), maximum total revenue (Slide 38) and maximum profit (Slide 40).
- Minimum average cost occurs where MC = AC (Slide 36), which links the optimisation condition to the comparison of two cost curves.

## ⚠️ Unclear or conflicting in the sources

- No lecture recording or transcript was provided in the sources, only slides, so no timestamps can be given and nothing can be added from the lecturer's spoken explanation.
- Slide 37: TR is written as (−q/4 + 260)q although p was found to be −q/4 + 65; the result −q²/4 + 65q and the later answer q = 130 are consistent with 65, so '260' looks like a typo, but the slide is contradictory as printed.
- Notation for second (and nth) derivatives is written as d²y/d²x and dⁿy/dⁿx (Slides 21, 33, 38, 40), and as d²y/dx on Slides 30-31. The standard notation is d²y/dx²; the intended meaning is clear from the worked examples but the slides are inconsistent.
- Slide 25: the supply function is described as a decreasing function of its own price P, which is unusual for a supply function (supply normally increases with price). It is also not stated why the differentiated expression is set equal to zero (presumably the quantity is held constant at equilibrium), and the slide speaks of the 'equilibrium price' although no demand function is given.
- Slide 23: the second example is printed as 'y = x23x'; the intended function can only be reconstructed from the answer (apparently y = x·2^{3x}).
- The slide numbers printed at the bottom of the later slides (29, 30, …, 43) do not match the order of the slides as supplied (Slides 26-40 in this file), which suggests some slides are missing from the source. The graphs referred to on Slides 4-6, 11, 27, 29-32, 35-37 and 39 are not described in the text, so their visual content cannot be explained here.
- Slide 10 states the relations with '⟺' (if and only if) using non-strict inequalities; the exact logical status of the strict versions in brackets is not fully spelled out.
- Slide 29 mentions a 'point of inflection' at x₂ in a graph, but the slides give no definition or test for a point of inflection.

## Recap

1. The derivative f′(a) = lim(h→0)[f(a+h) − f(a)]/h is the slope of the tangent to the curve at the point (a, f(a)), i.e. the rate of change of the function at that point.
2. The slope of a straight line is constant (Δy/Δx), but the slope of a curve changes at every point, which is why the limit idea is needed.
3. The sign of the first derivative tells you whether the function is increasing (f′ > 0), decreasing (f′ < 0) or constant (f′ = 0).
4. The main differentiation rules are the power rule, constants, sums/differences, product, quotient and chain rules, plus the special rules for eˣ, aˣ and ln x.
5. The chain rule (differentiate the outer function, then multiply by the derivative of the inner function) also allows implicit differentiation of equations like y³ + 3x²y = 13.
6. In economics the derivative is a marginal quantity: K′(t) = investment, C′(x) = marginal cost, dTR/dq = marginal revenue.
7. To optimise: set the first derivative equal to zero (first-order condition), then use the second derivative — negative means a maximum, positive means a minimum.
8. Applied examples: average cost is minimised at q = 10 where MC = AC, total revenue is maximised at q = 130, and profit (Π = TR − TC = −3q² + 198q − 500) is maximised at q = 33.
