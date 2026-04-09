<div style="background: linear-gradient(135deg, #f39c12 0%, #e67e22 100%); border-radius: 1rem; padding: 2rem 1.8rem 1.6rem; margin-bottom: 2.5rem; color: #fff;">
  <div style="font-size: 0.78rem; font-weight: 700; text-transform: uppercase; letter-spacing: 0.1em; opacity: 0.85; margin-bottom: 0.45rem;">NCTB General Math 9–10 · Chapter 1 — Real Numbers</div>
  <h1 style="font-size: 2rem; font-weight: 900; margin: 0 0 0.35rem; color: #fff; line-height: 1.2;">Exercise 1.1</h1>
  <div style="font-size: 0.93rem; opacity: 0.9; margin: 0;">12 questions · Rational &amp; irrational numbers, recurring decimals, all four operations</div>
</div>

---

**Question 1** 🟢 Easy

Which of the following numbers is irrational?

$$1)\ 0.\overline{3} \qquad 2)\ \sqrt{\dfrac{16}{9}} \qquad 3)\ \sqrt[3]{\dfrac{8}{27}} \qquad 4)\ \dfrac{5}{\sqrt{3}}$$

!!! abstract "📖 Theory — Rational and Irrational Numbers"
    A **rational number** is any number that can be written as \(\dfrac{p}{q}\), where \(p\) and \(q\) are integers and \(q \neq 0\). Every terminating decimal and every repeating decimal is rational.

    An **irrational number** cannot be written in the form \(\dfrac{p}{q}\). Its decimal expansion goes on forever without any repeating pattern. Examples: \(\sqrt{2},\ \sqrt{3},\ \pi\).

!!! tip "📌 Strategy"
    Try to simplify each option to a plain fraction or integer. If you can, it is rational. If you end up with a square root (or cube root) of a non-perfect-square, it is irrational.

**Step 1 — Check option 1:** \(0.\overline{3}\)

A repeating decimal is always rational. We know:

$$0.\overline{3} = 0.3333\ldots = \frac{1}{3}$$

This is a ratio of two integers — **rational**. ✗

**Step 2 — Check option 2:** \(\sqrt{\dfrac{16}{9}}\)

Both 16 and 9 are perfect squares (\(4^2 = 16\) and \(3^2 = 9\)), so the square root simplifies cleanly:

$$\sqrt{\frac{16}{9}} = \frac{\sqrt{16}}{\sqrt{9}} = \frac{4}{3}$$

This is a ratio of two integers — **rational**. ✗

**Step 3 — Check option 3:** \(\sqrt[3]{\dfrac{8}{27}}\)

Both 8 and 27 are perfect cubes (\(2^3 = 8\) and \(3^3 = 27\)), so:

$$\sqrt[3]{\frac{8}{27}} = \frac{\sqrt[3]{8}}{\sqrt[3]{27}} = \frac{2}{3}$$

This is a ratio of two integers — **rational**. ✗

**Step 4 — Check option 4:** \(\dfrac{5}{\sqrt{3}}\)

\(\sqrt{3}\) is irrational — 3 is not a perfect square so it cannot be written as any fraction. Dividing a non-zero integer by an irrational number always gives an irrational result.

We can rationalise the denominator to confirm:

$$\frac{5}{\sqrt{3}} = \frac{5}{\sqrt{3}} \times \frac{\sqrt{3}}{\sqrt{3}} = \frac{5\sqrt{3}}{3}$$

Since \(\sqrt{3}\) is irrational, \(\dfrac{5\sqrt{3}}{3}\) is also irrational. ✓

!!! success "✅ Final Answer"
    Option **4)** — \(\dfrac{5}{\sqrt{3}}\) is irrational.

---

**Question 5** 🔴 Hard

Prove that the following numbers are irrational: &emsp; 1) \(\sqrt{5}\) &emsp; 3) \(\sqrt{10}\)

!!! abstract "📖 Theory — Proof by Contradiction"
    To prove a number is irrational, we use **proof by contradiction**:

    1. **Assume the opposite** — suppose the number *is* rational.
    2. **Follow the logic** — work out what must be true under that assumption.
    3. **Find a contradiction** — show the assumption leads to an impossibility.
    4. **Conclude** — since the assumption is false, the number must be irrational.

    We also use this key fact: **if a prime \(p\) divides \(n^2\), then \(p\) also divides \(n\).**

!!! tip "📌 Strategy"
    Assume \(\sqrt{5} = \dfrac{p}{q}\) in lowest terms (no common factors). Square both sides. Use the divisibility rule for primes to show both \(p\) and \(q\) share a common factor — contradicting "lowest terms".

**(1) Prove \(\sqrt{5}\) is irrational**

**Step 1 — Assume it is rational**

Suppose \(\sqrt{5}\) is rational. Then we can write:

$$\sqrt{5} = \frac{p}{q}$$

where \(p\) and \(q\) are integers, \(q \neq 0\), and \(\gcd(p,\, q) = 1\) (the fraction is fully reduced — \(p\) and \(q\) share no common factor).

**Step 2 — Square both sides**

$$5 = \frac{p^2}{q^2} \implies p^2 = 5q^2 \quad \cdots (i)$$

**Step 3 — Show that 5 divides \(p\)**

From (i), \(p^2 = 5q^2\), so 5 divides \(p^2\).

Since **5 is prime**, if 5 divides \(p^2\) then 5 must also divide \(p\).

Write \(p = 5m\) for some integer \(m\).

**Step 4 — Show that 5 also divides \(q\)**

Substitute \(p = 5m\) into equation (i):

$$(5m)^2 = 5q^2 \implies 25m^2 = 5q^2 \implies 5m^2 = q^2$$

So 5 divides \(q^2\), and since 5 is prime, 5 also divides \(q\).

**Step 5 — Contradiction**

We now have: 5 divides \(p\) **and** 5 divides \(q\).

This means \(p\) and \(q\) share the common factor 5 — directly contradicting our assumption that \(\gcd(p,\, q) = 1\).

$$\therefore\quad \sqrt{5} \text{ is irrational.} \qquad \blacksquare$$

<hr>

**(3) Prove \(\sqrt{10}\) is irrational**

!!! tip "📌 Strategy"
    Same method — but this time we use the prime **2** (since \(10 = 2 \times 5\)) to derive the contradiction.

**Step 1 — Assume it is rational**

Suppose \(\sqrt{10} = \dfrac{p}{q}\) where \(\gcd(p,\, q) = 1\).

Squaring:

$$p^2 = 10q^2 \quad \cdots (i)$$

**Step 2 — Show that 2 divides \(p\)**

From (i), \(p^2 = 10q^2\). Since \(10 = 2 \times 5\), clearly 2 divides \(p^2\).

Since 2 is prime and 2 divides \(p^2\), we get 2 divides \(p\).

Write \(p = 2m\).

**Step 3 — Show that 2 also divides \(q\)**

Substitute \(p = 2m\) into (i):

$$(2m)^2 = 10q^2 \implies 4m^2 = 10q^2 \implies 2m^2 = 5q^2$$

So 2 divides \(5q^2\). Since \(\gcd(2, 5) = 1\) (2 and 5 share no factors), 2 must divide \(q^2\). Since 2 is prime, 2 divides \(q\).

**Step 4 — Contradiction**

Both \(p\) and \(q\) are divisible by 2, contradicting \(\gcd(p,\, q) = 1\).

$$\therefore\quad \sqrt{10} \text{ is irrational.} \qquad \blacksquare$$

!!! success "✅ Final Answer"
    Both \(\sqrt{5}\) and \(\sqrt{10}\) are irrational — proved by contradiction using the prime divisibility rule.

---

**Question 6** 🟡 Medium

**(1)** Find two irrational numbers between \(0.12\) and \(0.31\).

**(2)** Find a rational and an irrational number between \(\dfrac{1}{\sqrt{2}}\) and \(\sqrt{2}\).

!!! abstract "📖 Theory — Density of Real Numbers"
    Between any two distinct real numbers, there are infinitely many rational numbers and infinitely many irrational numbers. To find an irrational number inside an interval \((a,\, b)\), a useful method is to find \(\sqrt{k}\) where \(k\) is chosen so that \(a < \sqrt{k} < b\) — equivalently, \(a^2 < k < b^2\), with \(k\) not a perfect square.

!!! tip "📌 Strategy"
    **Part (1):** Square the interval boundaries to find the target range for \(k\), then pick two simple non-perfect-square values inside that range.  
    **Part (2):** Compute approximate decimals for the boundaries, then identify a plain integer (rational) and a simple surd (irrational) between them.

**(1) Two irrational numbers between 0.12 and 0.31**

**Step 1 — Find the target range for \(k\)**

We want \(\sqrt{k}\) to satisfy \(0.12 < \sqrt{k} < 0.31\).

Squaring throughout:

$$0.12^2 < k < 0.31^2 \implies 0.0144 < k < 0.0961$$

We need non-perfect-square rationals \(k\) inside this range.

**Step 2 — Choose two values**

Pick \(k = 0.05\) and \(k = 0.08\) (both lie between 0.0144 and 0.0961):

$$\sqrt{0.05} = \frac{\sqrt{5}}{10} \approx 0.2236 \qquad \sqrt{0.08} = \frac{\sqrt{2}}{5} \approx 0.2828$$

**Step 3 — Verify the interval and irrationality**

$$0.12 < 0.2236 < 0.31\ \checkmark \qquad 0.12 < 0.2828 < 0.31\ \checkmark$$

Both are irrational: \(\sqrt{5}\) and \(\sqrt{2}\) are irrational, and dividing an irrational number by a rational non-zero number keeps it irrational.

<hr>

**(2) A rational and an irrational between \(\dfrac{1}{\sqrt{2}}\) and \(\sqrt{2}\)**

**Step 1 — Find decimal approximations of the boundaries**

$$\frac{1}{\sqrt{2}} = \frac{\sqrt{2}}{2} \approx 0.707 \qquad \sqrt{2} \approx 1.414$$

We need one rational and one irrational number strictly between \(0.707\) and \(1.414\).

**Step 2 — Rational number**

The integer 1 is rational, and:

$$0.707 < 1 < 1.414\ \checkmark$$

**Step 3 — Irrational number**

Consider \(\dfrac{\sqrt{6}}{2}\):

$$\frac{\sqrt{6}}{2} \approx \frac{2.449}{2} \approx 1.225$$

Check: \(0.707 < 1.225 < 1.414\ \checkmark\)

\(\dfrac{\sqrt{6}}{2}\) is irrational because \(\sqrt{6}\) is irrational (6 is not a perfect square), and dividing by 2 does not make it rational.

!!! success "✅ Final Answer"
    **(1)** Two irrational numbers between 0.12 and 0.31: \(\quad\dfrac{\sqrt{5}}{10} \approx 0.2236\quad\) and \(\quad\dfrac{\sqrt{2}}{5} \approx 0.2828\)

    **(2)** Between \(\dfrac{1}{\sqrt{2}}\) and \(\sqrt{2}\): &emsp; Rational: **1** &emsp;·&emsp; Irrational: \(\dfrac{\sqrt{6}}{2}\)

---

**Question 8** 🟢 Easy

Convert the following into repeating decimal fractions: &emsp; 1) \(\dfrac{1}{6}\) &emsp; 2) \(\dfrac{7}{11}\) &emsp; 4) \(3\dfrac{8}{15}\)

!!! abstract "📖 Theory — Converting Fractions to Recurring Decimals"
    To convert a fraction to a decimal, carry out **long division** — divide the numerator by the denominator. Whenever the remainder repeats, the decimal digits from that point onwards will repeat in the same cycle. The repeating block of digits is called the **recurring period**.

!!! tip "📌 Strategy"
    Perform long division step by step. As soon as you see a remainder you have seen before, the decimal has started to repeat — stop and write the overline notation.

**Step 1 — Convert \(\dfrac{1}{6}\)**

Divide 1 by 6:

- \(10 \div 6 = 1\), remainder \(4\)
- \(40 \div 6 = 6\), remainder \(4\) &nbsp;← remainder repeats

The digit 6 repeats forever:

$$\frac{1}{6} = 0.1\overline{6}$$

**Step 2 — Convert \(\dfrac{7}{11}\)**

Divide 7 by 11:

- \(70 \div 11 = 6\), remainder \(4\)
- \(40 \div 11 = 3\), remainder \(7\)
- \(70 \div 11 = 6\), remainder \(4\) &nbsp;← cycle repeats

The block "63" repeats forever:

$$\frac{7}{11} = 0.\overline{63}$$

**Step 3 — Convert \(3\dfrac{8}{15}\)**

The whole number 3 stays as is. Convert the fractional part \(\dfrac{8}{15}\):

- \(80 \div 15 = 5\), remainder \(5\)
- \(50 \div 15 = 3\), remainder \(5\) &nbsp;← remainder repeats

So \(\dfrac{8}{15} = 0.5\overline{3}\), and therefore:

$$3\frac{8}{15} = 3.5\overline{3}$$

!!! success "✅ Final Answer"
    $$\frac{1}{6} = 0.1\overline{6} \qquad \frac{7}{11} = 0.\overline{63} \qquad 3\frac{8}{15} = 3.5\overline{3}$$

---

**Question 9** 🟡 Medium

Convert into simple fractions: &emsp; 1) \(0.\overline{2}\) &emsp; 2) \(0.\overline{35}\) &emsp; 4) \(3.\overline{78}\)

!!! abstract "📖 Theory — Converting Recurring Decimals to Fractions"
    The key trick: let \(x\) equal the recurring decimal, then multiply by a power of 10 large enough to shift the decimal point so the recurring part lines up exactly with the original. Subtracting removes the infinite tail, leaving a simple equation.

    - If \(n\) digits form the recurring block, multiply by \(10^n\) and subtract.

!!! tip "📌 Strategy"
    **Formula:** A pure recurring decimal with \(n\) recurring digits equals the recurring block divided by \(n\) nines:
    $$0.\overline{d_1 d_2 \cdots d_n} = \frac{d_1 d_2 \cdots d_n}{\underbrace{99\cdots9}_{n}}$$

    For a number with a whole-number part (like \(3.\overline{78}\)), apply the same method to the full number, then the whole number part cancels naturally.

**Step 1 — Convert \(0.\overline{2}\)**

Let \(x = 0.2222\ldots\)

Multiply both sides by 10 (1 recurring digit):

$$10x = 2.2222\ldots$$

Subtract the original equation:

$$10x - x = 2.2222\ldots - 0.2222\ldots$$

$$9x = 2 \implies \boxed{x = \frac{2}{9}}$$

**Step 2 — Convert \(0.\overline{35}\)**

Let \(x = 0.353535\ldots\)

Multiply by 100 (2 recurring digits):

$$100x = 35.353535\ldots$$

Subtract:

$$100x - x = 35.353535\ldots - 0.353535\ldots$$

$$99x = 35 \implies \boxed{x = \frac{35}{99}}$$

**Step 3 — Convert \(3.\overline{78}\)**

Let \(x = 3.787878\ldots\)

Multiply by 100 (2 recurring digits):

$$100x = 378.787878\ldots$$

Subtract:

$$100x - x = 378.787878\ldots - 3.787878\ldots$$

$$99x = 375 \implies x = \frac{375}{99}$$

Simplify by dividing numerator and denominator by \(\gcd(375, 99) = 3\):

$$\boxed{x = \frac{125}{33}}$$

!!! note "📝 Note"
    Always check for common factors after subtracting. Here \(375 = 3 \times 125\) and \(99 = 3 \times 33\), so both divide by 3.

!!! success "✅ Final Answer"
    $$0.\overline{2} = \frac{2}{9} \qquad 0.\overline{35} = \frac{35}{99} \qquad 3.\overline{78} = \frac{125}{33}$$

---

**Question 10** 🟡 Medium

Express as **similar** repeating decimal fractions: &emsp; 1) \(2.\overline{23}\) and \(5.\overline{235}\)

!!! abstract "📖 Theory — Similar Recurring Decimal Fractions"
    Two recurring decimals are **similar** when they have both:

    - the same number of non-recurring digits after the decimal point, and
    - the same length of recurring period.

    To make two recurring decimals similar, find the **LCM** of their period lengths, then extend each recurring block by repeating it until it reaches that common length.

!!! tip "📌 Strategy"
    **Formula:** To extend a recurring block of length \(n\) to length \(L = \text{LCM}\), repeat the block \(L/n\) times.

**Step 1 — Identify the period of each decimal**

\(2.\overline{23}\): the block "23" repeats &ensp;→&ensp; **period = 2**

\(5.\overline{235}\): the block "235" repeats &ensp;→&ensp; **period = 3**

Both have **zero** non-recurring digits (the recurring part starts immediately after the decimal point).

**Step 2 — Find the LCM of the periods**

$$\text{LCM}(2,\ 3) = 6$$

The common period must be **6**.

**Step 3 — Extend each recurring block to length 6**

For \(2.\overline{23}\): repeat "23" three times → "232323"

$$2.\overline{23} \;=\; 2.\overline{232323}$$

For \(5.\overline{235}\): repeat "235" twice → "235235"

$$5.\overline{235} \;=\; 5.\overline{235235}$$

Both now have period 6 and zero non-recurring digits — they are **similar**.

!!! success "✅ Final Answer"
    $$2.\overline{23} = 2.\overline{232323} \qquad 5.\overline{235} = 5.\overline{235235}$$

---

**Question 11** 🟡 Medium

Add: &emsp; 1) \(0.\overline{45} + 0.\overline{134}\)

!!! tip "📌 Strategy"
    Convert each recurring decimal to a fraction using the recurring-digits rule, then add using a common denominator.

**Step 1 — Convert \(0.\overline{45}\) to a fraction**

Two recurring digits → divide by 99:

$$0.\overline{45} = \frac{45}{99}$$

Simplify: \(\gcd(45, 99) = 9\), so:

$$\frac{45}{99} = \frac{5}{11}$$

**Step 2 — Convert \(0.\overline{134}\) to a fraction**

Three recurring digits → divide by 999:

$$0.\overline{134} = \frac{134}{999}$$

\(\gcd(134, 999) = 1\), so this is already in simplest form.

**Step 3 — Find the LCM of the denominators**

$$999 = 3^3 \times 37 \qquad 11 \text{ is prime and does not divide } 999$$

$$\text{LCM}(11,\ 999) = 11 \times 999 = 10989$$

**Step 4 — Add the fractions**

$$\frac{5}{11} + \frac{134}{999} = \frac{5 \times 999}{10989} + \frac{134 \times 11}{10989} = \frac{4995 + 1474}{10989} = \frac{6469}{10989}$$

\(\gcd(6469,\ 10989) = 1\), so the fraction is fully simplified.

!!! success "✅ Final Answer"
    $$0.\overline{45} + 0.\overline{134} = \frac{6469}{10989}$$

---

**Question 12** 🟡 Medium

Subtract: &emsp; 1) \(3.\overline{4} - 2.\overline{13}\) &emsp;&emsp;&emsp; 3) \(8.\overline{49} - 5.\overline{356}\)

!!! tip "📌 Strategy"
    For each decimal, let \(x\) equal the full number and apply the recurring-decimal method to convert it to a fraction. Then subtract using a common denominator.

**(1) \(3.\overline{4} - 2.\overline{13}\)**

**Step 1 — Convert \(3.\overline{4}\)**

Let \(x = 3.4444\ldots\) &ensp;→&ensp; \(10x = 34.4444\ldots\) &ensp;→&ensp; \(9x = 31\)

$$3.\overline{4} = \frac{31}{9}$$

**Step 2 — Convert \(2.\overline{13}\)**

Let \(x = 2.131313\ldots\) &ensp;→&ensp; \(100x = 213.131313\ldots\) &ensp;→&ensp; \(99x = 211\)

$$2.\overline{13} = \frac{211}{99}$$

**Step 3 — Subtract**

$$\frac{31}{9} - \frac{211}{99} = \frac{341}{99} - \frac{211}{99} = \frac{130}{99}$$

Converting back: \(\dfrac{130}{99} = 1\dfrac{31}{99} = 1.\overline{31}\)

*Check:* \(3.4444\ldots - 2.1313\ldots = 1.3131\ldots\ \checkmark\)

<hr>

**(3) \(8.\overline{49} - 5.\overline{356}\)**

**Step 1 — Convert \(8.\overline{49}\)**

Let \(x = 8.494949\ldots\) &ensp;→&ensp; \(100x = 849.494949\ldots\) &ensp;→&ensp; \(99x = 841\)

$$8.\overline{49} = \frac{841}{99}$$

**Step 2 — Convert \(5.\overline{356}\)**

Let \(x = 5.356356\ldots\) &ensp;→&ensp; \(1000x = 5356.356356\ldots\) &ensp;→&ensp; \(999x = 5351\)

$$5.\overline{356} = \frac{5351}{999}$$

**Step 3 — Find the LCM of 99 and 999**

$$99 = 3^2 \times 11 \qquad 999 = 3^3 \times 37$$

$$\text{LCM}(99,\ 999) = 3^3 \times 11 \times 37 = 10989$$

**Step 4 — Subtract**

$$\frac{841}{99} - \frac{5351}{999} = \frac{841 \times 111}{10989} - \frac{5351 \times 11}{10989} = \frac{93351 - 58861}{10989} = \frac{34490}{10989}$$

\(\gcd(34490,\ 10989) = 1\), so the fraction is fully simplified.

!!! success "✅ Final Answer"
    $$3.\overline{4} - 2.\overline{13} = \frac{130}{99} = 1.\overline{31}$$
    $$8.\overline{49} - 5.\overline{356} = \frac{34490}{10989}$$

---

**Question 13** 🟡 Medium

Multiply: &emsp; 1) \(0.\overline{3} \times 0.\overline{6}\) &emsp;&emsp;&emsp; 3) \(0.\overline{62} \times 0.\overline{3}\)

!!! tip "📌 Strategy"
    Convert each recurring decimal to a fraction, multiply the fractions, then simplify. Check whether the result converts back to a recognisable recurring decimal.

**(1) \(0.\overline{3} \times 0.\overline{6}\)**

**Step 1 — Convert to fractions**

$$0.\overline{3} = \frac{3}{9} = \frac{1}{3} \qquad 0.\overline{6} = \frac{6}{9} = \frac{2}{3}$$

**Step 2 — Multiply**

$$\frac{1}{3} \times \frac{2}{3} = \frac{2}{9} = 0.\overline{2}$$

<hr>

**(3) \(0.\overline{62} \times 0.\overline{3}\)**

**Step 1 — Convert to fractions**

$$0.\overline{62} = \frac{62}{99} \qquad 0.\overline{3} = \frac{1}{3}$$

**Step 2 — Multiply**

$$\frac{62}{99} \times \frac{1}{3} = \frac{62}{297}$$

\(\gcd(62,\ 297) = 1\) &ensp;(since \(62 = 2 \times 31\) and \(297 = 3^3 \times 11\) share no common prime factors), so the fraction is fully simplified.

!!! success "✅ Final Answer"
    $$0.\overline{3} \times 0.\overline{6} = \frac{2}{9} = 0.\overline{2}$$
    $$0.\overline{62} \times 0.\overline{3} = \frac{62}{297}$$

---

**Question 14** 🟡 Medium

Divide: &emsp; 1) \(0.\overline{3} \div 0.\overline{6}\) &emsp;&emsp;&emsp; 3) \(2.\overline{37} \div 0.\overline{45}\)

!!! tip "📌 Strategy"
    Convert to fractions, then **divide by multiplying by the reciprocal**. Simplify fully — look for common factors between numerator and denominator.

**(1) \(0.\overline{3} \div 0.\overline{6}\)**

**Step 1 — Convert to fractions**

$$0.\overline{3} = \frac{1}{3} \qquad 0.\overline{6} = \frac{2}{3}$$

**Step 2 — Divide**

$$\frac{1}{3} \div \frac{2}{3} = \frac{1}{3} \times \frac{3}{2} = \frac{1}{2} = 0.5$$

<hr>

**(3) \(2.\overline{37} \div 0.\overline{45}\)**

**Step 1 — Convert \(2.\overline{37}\)**

Let \(x = 2.373737\ldots\) &ensp;→&ensp; \(100x = 237.373737\ldots\) &ensp;→&ensp; \(99x = 235\)

$$2.\overline{37} = \frac{235}{99}$$

**Step 2 — Convert \(0.\overline{45}\)**

$$0.\overline{45} = \frac{45}{99} = \frac{5}{11}$$

**Step 3 — Divide**

$$\frac{235}{99} \div \frac{5}{11} = \frac{235}{99} \times \frac{11}{5} = \frac{235 \times 11}{99 \times 5}$$

Factor to cancel: \(235 = 5 \times 47\) and \(99 = 9 \times 11\), so:

$$= \frac{\cancel{5} \times 47 \times \cancel{11}}{9 \times \cancel{11} \times \cancel{5}} = \frac{47}{9} = 5.\overline{2}$$

!!! success "✅ Final Answer"
    $$0.\overline{3} \div 0.\overline{6} = \frac{1}{2} = 0.5$$
    $$2.\overline{37} \div 0.\overline{45} = \frac{47}{9} = 5.\overline{2}$$

---

**Question 15** 🟡 Medium

Write down the value and its approximation to 4 decimal places: &emsp; 2) \(0.\overline{25}\) &emsp; 3) \(1.\overline{34}\)

!!! tip "📌 Strategy"
    Convert the recurring decimal to a fraction — that is its exact value. Then write out enough decimal places to apply the rounding rule: look at the **5th** decimal digit; if it is 5 or more, round up the 4th digit; if less than 5, leave it unchanged.

**Step 1 — Exact value of \(0.\overline{25}\)**

$$0.\overline{25} = \frac{25}{99}$$

Decimal expansion: \(0.25252525\ldots\)

**Step 2 — Approximate \(0.\overline{25}\) to 4 decimal places**

The first 5 decimal digits are: \(0.2525\mathbf{2}\ldots\)

The 5th digit is **2** (less than 5) → round down (keep the 4th digit as is):

$$0.\overline{25} \approx 0.2525$$

**Step 3 — Exact value of \(1.\overline{34}\)**

$$1.\overline{34} = 1 + \frac{34}{99} = \frac{99 + 34}{99} = \frac{133}{99}$$

Decimal expansion: \(1.34343434\ldots\)

**Step 4 — Approximate \(1.\overline{34}\) to 4 decimal places**

The first 5 decimal digits are: \(1.3434\mathbf{3}\ldots\)

The 5th digit is **3** (less than 5) → round down:

$$1.\overline{34} \approx 1.3434$$

!!! success "✅ Final Answer"
    | Number | Exact value | Approx (4 d.p.) |
    |--------|-------------|-----------------|
    | \(0.\overline{25}\) | \(\dfrac{25}{99}\) | \(0.2525\) |
    | \(1.\overline{34}\) | \(\dfrac{133}{99}\) | \(1.3434\) |

---

**Question 16** 🟢 Easy

State which of the following are rational and which are irrational:

$$2)\ \sqrt{9} \qquad 3)\ \sqrt{11} \qquad 5)\ \frac{\sqrt{8}}{\sqrt{7}} \qquad 6)\ \frac{\sqrt{27}}{\sqrt{48}}$$

!!! tip "📌 Strategy"
    Simplify each expression as far as possible. If the result is a fraction of integers, it is rational. If it still contains a square root of a non-perfect-square number, it is irrational.

**Step 1 — Classify \(\sqrt{9}\)**

$$\sqrt{9} = 3$$

A whole number is rational. → **Rational**

**Step 2 — Classify \(\sqrt{11}\)**

Is 11 a perfect square? \(3^2 = 9\) and \(4^2 = 16\), so 11 lies between them — it is **not** a perfect square. Its decimal expansion is non-terminating and non-repeating.

→ **Irrational**

**Step 3 — Classify \(\dfrac{\sqrt{8}}{\sqrt{7}}\)**

$$\frac{\sqrt{8}}{\sqrt{7}} = \sqrt{\frac{8}{7}} = \frac{2\sqrt{2}}{\sqrt{7}} = \frac{2\sqrt{2} \cdot \sqrt{7}}{7} = \frac{2\sqrt{14}}{7}$$

Since 14 is not a perfect square, \(\sqrt{14}\) is irrational, so \(\dfrac{2\sqrt{14}}{7}\) is also irrational.

→ **Irrational**

**Step 4 — Classify \(\dfrac{\sqrt{27}}{\sqrt{48}}\)**

$$\frac{\sqrt{27}}{\sqrt{48}} = \sqrt{\frac{27}{48}}$$

Simplify the fraction inside: \(\dfrac{27}{48} = \dfrac{9}{16}\) (divide both by 3).

$$\sqrt{\frac{9}{16}} = \frac{\sqrt{9}}{\sqrt{16}} = \frac{3}{4}$$

Since both 9 and 16 are perfect squares, the result is a fraction of integers.

→ **Rational**

!!! note "📝 Note"
    Never assume a ratio of two surds is always irrational — always simplify first. Here \(\sqrt{27}/\sqrt{48}\) looks irrational but the surds cancel to give the rational \(\frac{3}{4}\).

!!! success "✅ Final Answer"
    | Expression | Simplified form | Type |
    |-----------|-----------------|------|
    | \(\sqrt{9}\) | \(3\) | Rational |
    | \(\sqrt{11}\) | \(\sqrt{11}\) | Irrational |
    | \(\dfrac{\sqrt{8}}{\sqrt{7}}\) | \(\dfrac{2\sqrt{14}}{7}\) | Irrational |
    | \(\dfrac{\sqrt{27}}{\sqrt{48}}\) | \(\dfrac{3}{4}\) | Rational |
