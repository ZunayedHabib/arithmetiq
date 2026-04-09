---
title: Exercise 1.1 — Real Numbers
---

<style>
/* ── Reset & container ───────────────────────────── */
#aqe { font-family: inherit; }

/* ── Page header ─────────────────────────────────── */
.aqe-header {
  background: linear-gradient(135deg, #f39c12 0%, #e67e22 100%);
  border-radius: 1rem;
  padding: 2rem 1.8rem 1.6rem;
  color: #fff;
  margin-bottom: 1.5rem;
}
.aqe-header-sub {
  font-size: 0.78rem; font-weight: 700; text-transform: uppercase;
  letter-spacing: 0.1em; opacity: 0.85; margin-bottom: 0.45rem;
}
.aqe-header h1 {
  font-size: 2rem; font-weight: 900; margin: 0 0 0.35rem;
  color: #fff; line-height: 1.2; border: none; padding: 0;
}
.aqe-header-desc { font-size: 0.93rem; opacity: 0.9; margin: 0; }

/* ── Navigation bar ──────────────────────────────── */
.aqe-nav {
  display: flex; align-items: center; justify-content: space-between;
  background: #f5f7fa; border-radius: 0.75rem;
  padding: 0.7rem 1rem; margin: 1rem 0;
  border: 1px solid #e0e0e0;
}
[data-md-color-scheme="slate"] .aqe-nav {
  background: #1e2533; border-color: #3a4a5c;
}
.aqe-btn {
  background: linear-gradient(135deg, #f39c12, #e67e22);
  color: #fff; border: none; border-radius: 0.5rem;
  padding: 0.5rem 1.15rem; font-size: 0.88rem; font-weight: 700;
  cursor: pointer; transition: opacity 0.15s; letter-spacing: 0.01em;
}
.aqe-btn:hover { opacity: 0.88; }
.aqe-counter {
  font-size: 0.88rem; font-weight: 600; color: #555;
}
[data-md-color-scheme="slate"] .aqe-counter { color: #a0aec0; }

/* ── Question visibility ─────────────────────────── */
.aqe-q { display: none; }
.aqe-q.aqe-active { display: block; }

/* ── Question header ─────────────────────────────── */
.aqe-q-head {
  display: flex; align-items: center; gap: 0.8rem;
  font-size: 1.2rem; font-weight: 800;
  padding-bottom: 0.6rem; margin-bottom: 1.1rem;
  border-bottom: 2.5px solid #f39c12;
  color: #1a202c;
}
[data-md-color-scheme="slate"] .aqe-q-head { color: #e2e8f0; }

.aqe-badge {
  font-size: 0.72rem; font-weight: 700; text-transform: uppercase;
  letter-spacing: 0.06em; padding: 0.22em 0.8em;
  border-radius: 999px; color: #fff; white-space: nowrap;
}
.aqe-easy   { background: #27ae60; }
.aqe-medium { background: #e67e22; }
.aqe-hard   { background: #e74c3c; }

/* ── Question text ───────────────────────────────── */
.aqe-qtext {
  font-size: 1rem; line-height: 1.75; margin-bottom: 1rem;
  color: #2d3748;
}
[data-md-color-scheme="slate"] .aqe-qtext { color: #e2e8f0; }

/* ── Theory box ──────────────────────────────────── */
.aqe-theory { border-radius: 0.6rem; overflow: hidden; margin: 1rem 0; }
.aqe-theory-h {
  background: #1a3a5c; color: #fff;
  font-weight: 700; font-size: 0.85rem;
  padding: 0.5rem 1rem; letter-spacing: 0.03em;
}
.aqe-theory-b {
  background: #e8f4fd; padding: 0.9rem 1.15rem;
  font-size: 0.93rem; line-height: 1.8; color: #1a202c;
}
[data-md-color-scheme="slate"] .aqe-theory-b { background: #0d1f35; color: #e2e8f0; }

/* ── Strategy box ────────────────────────────────── */
.aqe-strat { border-radius: 0.6rem; overflow: hidden; margin: 1rem 0; }
.aqe-strat-h {
  background: #0d6654; color: #fff;
  font-weight: 700; font-size: 0.85rem;
  padding: 0.5rem 1rem; letter-spacing: 0.03em;
}
.aqe-strat-b {
  background: #e0f5f0; padding: 0.9rem 1.15rem;
  font-size: 0.93rem; line-height: 1.8; color: #1a202c;
}
[data-md-color-scheme="slate"] .aqe-strat-b { background: #0a2820; color: #e2e8f0; }

/* ── Step box ────────────────────────────────────── */
.aqe-step {
  background: #fff; border: 1px solid #e2e8f0;
  border-radius: 0.6rem; margin: 0.85rem 0;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05); overflow: hidden;
}
[data-md-color-scheme="slate"] .aqe-step {
  background: #1e2533; border-color: #3a4a5c;
  box-shadow: 0 2px 8px rgba(0,0,0,0.2);
}
.aqe-step-h {
  background: #f7f8fa; border-bottom: 1px solid #e2e8f0;
  padding: 0.55rem 1rem; font-weight: 700; font-size: 0.88rem;
  color: #2d3748;
}
[data-md-color-scheme="slate"] .aqe-step-h {
  background: #283244; border-color: #3a4a5c; color: #e2e8f0;
}
.aqe-step-b {
  padding: 0.9rem 1.15rem; font-size: 0.93rem;
  line-height: 1.85; color: #2d3748;
}
[data-md-color-scheme="slate"] .aqe-step-b { color: #e2e8f0; }

/* ── Part separator ──────────────────────────────── */
.aqe-sep {
  border: none; border-top: 1.5px dashed #d0d5dd;
  margin: 1.3rem 0 1rem;
}
[data-md-color-scheme="slate"] .aqe-sep { border-color: #3a4a5c; }
.aqe-part {
  font-weight: 700; font-size: 1rem; color: #2d3748; margin: 0.6rem 0 0.5rem;
}
[data-md-color-scheme="slate"] .aqe-part { color: #e2e8f0; }

/* ── Note box ────────────────────────────────────── */
.aqe-note { border-radius: 0.6rem; overflow: hidden; margin: 1rem 0; }
.aqe-note-h {
  background: #9a7d0a; color: #fff;
  font-weight: 700; font-size: 0.85rem;
  padding: 0.5rem 1rem;
}
.aqe-note-b {
  background: #fef9e7; padding: 0.9rem 1.15rem;
  font-size: 0.93rem; line-height: 1.8; color: #1a202c;
}
[data-md-color-scheme="slate"] .aqe-note-b { background: #2c2400; color: #e2e8f0; }

/* ── Final answer box ────────────────────────────── */
.aqe-ans { border-radius: 0.6rem; overflow: hidden; margin: 1.2rem 0 0.5rem; }
.aqe-ans-h {
  background: #1a5c1a; color: #fff;
  font-weight: 700; font-size: 0.85rem;
  padding: 0.5rem 1rem;
}
.aqe-ans-b {
  background: #e8f8e8; padding: 0.9rem 1.15rem;
  font-size: 0.93rem; line-height: 1.9; color: #1a202c;
}
[data-md-color-scheme="slate"] .aqe-ans-b { background: #0a2010; color: #e2e8f0; }

/* ── Answer table ────────────────────────────────── */
.aqe-tbl {
  border-collapse: collapse; width: 100%;
  font-size: 0.92rem; margin-top: 0.4rem;
}
.aqe-tbl th {
  background: rgba(0,0,0,0.07); padding: 0.45rem 0.8rem;
  text-align: left; font-weight: 700; border: 1px solid #c8e6c9;
}
[data-md-color-scheme="slate"] .aqe-tbl th {
  background: rgba(255,255,255,0.08); border-color: #1a4a1a;
}
.aqe-tbl td {
  padding: 0.45rem 0.8rem; border: 1px solid #c8e6c9;
  vertical-align: middle;
}
[data-md-color-scheme="slate"] .aqe-tbl td { border-color: #1a4a1a; }
.aqe-rat  { color: #1a5c1a; font-weight: 700; }
.aqe-irr  { color: #c0392b; font-weight: 700; }
[data-md-color-scheme="slate"] .aqe-rat  { color: #6fdc6f; }
[data-md-color-scheme="slate"] .aqe-irr  { color: #ff8080; }

/* ── Inline helpers ──────────────────────────────── */
.aqe-ok  { color: #27ae60; font-weight: 700; }
.aqe-no  { color: #e74c3c; font-weight: 700; }
.aqe-kb  { font-weight: 700; }
</style>

<div id="aqe">

<!-- ══════════════════════════════════════════════
     PAGE HEADER
══════════════════════════════════════════════ -->
<div class="aqe-header">
  <div class="aqe-header-sub">NCTB General Math 9–10 · Chapter 1 — Real Numbers</div>
  <h1>Exercise 1.1</h1>
  <div class="aqe-header-desc">12 questions · Rational &amp; irrational numbers, recurring decimals, all four operations</div>
</div>

<!-- ══════════════════════════════════════════════
     TOP NAVIGATION
══════════════════════════════════════════════ -->
<div class="aqe-nav">
  <button class="aqe-btn aqe-btn-prev">← Previous</button>
  <span class="aqe-counter">Question 1 of 12</span>
  <button class="aqe-btn aqe-btn-next">Next →</button>
</div>

<!-- ══════════════════════════════════════════════
     QUESTION 1 — Which is irrational? (MCQ)
══════════════════════════════════════════════ -->
<div class="aqe-q aqe-active arithmatex" id="aqe-q-0">

  <div class="aqe-q-head">
    Question 1 <span class="aqe-badge aqe-easy">🟢 Easy</span>
  </div>

  <div class="aqe-qtext">
    Which of the following is an irrational number?
    $$1)\ 0.\overline{3} \qquad 2)\ \sqrt{\dfrac{16}{9}} \qquad 3)\ \sqrt[3]{\dfrac{8}{27}} \qquad 4)\ \dfrac{5}{\sqrt{3}}$$
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Try to simplify each option completely. If it reduces to a fraction \(\frac{p}{q}\) of two integers, it is <strong>rational</strong>. If it still contains a square root of a non-perfect-square number, it is <strong>irrational</strong>.<br><br>
      <strong>Key idea:</strong> A rational number is any number that can be written as \(\frac{p}{q}\) where \(p\) and \(q\) are integers and \(q \neq 0\). Every repeating decimal and every terminating decimal is rational.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Check option 1: \(0.\overline{3}\)</div>
    <div class="aqe-step-b">
      A repeating decimal is always rational. We know from basic fractions:<br><br>
      $$0.\overline{3} = 0.3333\ldots = \frac{1}{3}$$
      This is a ratio of two integers — <span class="aqe-no">Rational ✗</span>
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Check option 2: \(\sqrt{\dfrac{16}{9}}\)</div>
    <div class="aqe-step-b">
      Both 16 and 9 are perfect squares (\(4^2 = 16\) and \(3^2 = 9\)), so the square root simplifies completely:
      $$\sqrt{\frac{16}{9}} = \frac{\sqrt{16}}{\sqrt{9}} = \frac{4}{3}$$
      This is a ratio of two integers — <span class="aqe-no">Rational ✗</span>
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Check option 3: \(\sqrt[3]{\dfrac{8}{27}}\)</div>
    <div class="aqe-step-b">
      Both 8 and 27 are perfect cubes (\(2^3 = 8\) and \(3^3 = 27\)):
      $$\sqrt[3]{\frac{8}{27}} = \frac{\sqrt[3]{8}}{\sqrt[3]{27}} = \frac{2}{3}$$
      This is a ratio of two integers — <span class="aqe-no">Rational ✗</span>
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 4 — Check option 4: \(\dfrac{5}{\sqrt{3}}\)</div>
    <div class="aqe-step-b">
      \(\sqrt{3}\) is irrational — 3 is not a perfect square, so it cannot be written as a fraction. Dividing a non-zero integer by an irrational number always gives an irrational result.<br><br>
      We can rationalise the denominator to confirm:
      $$\frac{5}{\sqrt{3}} = \frac{5}{\sqrt{3}} \times \frac{\sqrt{3}}{\sqrt{3}} = \frac{5\sqrt{3}}{3}$$
      Since \(\sqrt{3}\) is irrational, \(\dfrac{5\sqrt{3}}{3}\) is also irrational — <span class="aqe-ok">Irrational ✓</span>
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      Option <strong>4)</strong> — \(\dfrac{5}{\sqrt{3}}\) is the irrational number.
    </div>
  </div>

</div><!-- end Q1 -->

<!-- ══════════════════════════════════════════════
     QUESTION 2 — Prove √5 and √10 irrational
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-1">

  <div class="aqe-q-head">
    Question 2 <span class="aqe-badge aqe-hard">🔴 Hard</span>
  </div>

  <div class="aqe-qtext">
    Prove that the following numbers are irrational: &emsp; <strong>1)</strong> \(\sqrt{5}\) &emsp; <strong>3)</strong> \(\sqrt{10}\)
  </div>

  <div class="aqe-theory">
    <div class="aqe-theory-h">📖 Theory — Proof by Contradiction</div>
    <div class="aqe-theory-b">
      To prove a number is irrational, we use a method called <strong>proof by contradiction</strong>:<br><br>
      &nbsp;&nbsp;1. <strong>Assume the opposite</strong> — suppose the number <em>is</em> rational.<br>
      &nbsp;&nbsp;2. <strong>Follow the logic</strong> — work out what must be true under that assumption.<br>
      &nbsp;&nbsp;3. <strong>Find a contradiction</strong> — show the assumption leads to something impossible.<br>
      &nbsp;&nbsp;4. <strong>Conclude</strong> — since the assumption is false, the number must be irrational.<br><br>
      We also use this critical fact about primes:<br>
      <strong>If a prime \(p\) divides \(n^2\), then \(p\) must also divide \(n\).</strong>
    </div>
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Assume \(\sqrt{5} = \frac{p}{q}\) in <strong>lowest terms</strong> (meaning \(p\) and \(q\) share no common factor, i.e.\ \(\gcd(p,q) = 1\)). Square both sides. Use the prime divisibility rule to show both \(p\) and \(q\) must be divisible by 5 — a direct contradiction of "lowest terms".
    </div>
  </div>

  <p class="aqe-part">(1) Prove that \(\sqrt{5}\) is irrational</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Assume \(\sqrt{5}\) is rational</div>
    <div class="aqe-step-b">
      Suppose \(\sqrt{5}\) is rational. Then we can write it as a fraction:
      $$\sqrt{5} = \frac{p}{q}$$
      where \(p\) and \(q\) are integers, \(q \neq 0\), and \(\gcd(p,\, q) = 1\) (the fraction is fully reduced).
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Square both sides</div>
    <div class="aqe-step-b">
      Squaring both sides of \(\sqrt{5} = \dfrac{p}{q}\):
      $$5 = \frac{p^2}{q^2} \implies p^2 = 5q^2 \quad \cdots (i)$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Show that 5 divides \(p\)</div>
    <div class="aqe-step-b">
      From equation (i), \(p^2 = 5q^2\), so <strong>5 divides \(p^2\)</strong>.<br><br>
      Since 5 is a prime number, if 5 divides \(p^2\) then 5 must also divide \(p\).<br><br>
      So we can write \(p = 5m\) for some integer \(m\).
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 4 — Show that 5 also divides \(q\) — contradiction</div>
    <div class="aqe-step-b">
      Substitute \(p = 5m\) into equation (i):
      $$(5m)^2 = 5q^2 \implies 25m^2 = 5q^2 \implies 5m^2 = q^2$$
      So 5 divides \(q^2\), and since 5 is prime, 5 must also divide \(q\).<br><br>
      We now have: 5 divides <em>both</em> \(p\) and \(q\).<br>
      But this contradicts our assumption that \(\gcd(p,\, q) = 1\).<br><br>
      $$\therefore\quad \sqrt{5} \text{ is irrational.} \qquad \blacksquare$$
    </div>
  </div>

  <hr class="aqe-sep">
  <p class="aqe-part">(3) Prove that \(\sqrt{10}\) is irrational</p>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Same method — but this time we use the prime <strong>2</strong> (since \(10 = 2 \times 5\)) to derive the contradiction.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Assume \(\sqrt{10}\) is rational</div>
    <div class="aqe-step-b">
      Suppose \(\sqrt{10} = \dfrac{p}{q}\) where \(\gcd(p,\, q) = 1\). Squaring:
      $$p^2 = 10q^2 \quad \cdots (i)$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Show that 2 divides \(p\)</div>
    <div class="aqe-step-b">
      From (i), \(p^2 = 10q^2\). Since \(10 = 2 \times 5\), clearly 2 divides \(p^2\).<br><br>
      Since 2 is prime and 2 divides \(p^2\), we get 2 divides \(p\).<br><br>
      Write \(p = 2m\).
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Show that 2 also divides \(q\) — contradiction</div>
    <div class="aqe-step-b">
      Substitute \(p = 2m\) into (i):
      $$(2m)^2 = 10q^2 \implies 4m^2 = 10q^2 \implies 2m^2 = 5q^2$$
      So 2 divides \(5q^2\). Since \(\gcd(2, 5) = 1\), 2 does not divide 5, so 2 must divide \(q^2\). Since 2 is prime, 2 divides \(q\).<br><br>
      Both \(p\) and \(q\) are divisible by 2 — this contradicts \(\gcd(p,\, q) = 1\).
      $$\therefore\quad \sqrt{10} \text{ is irrational.} \qquad \blacksquare$$
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      Both \(\sqrt{5}\) and \(\sqrt{10}\) are irrational — proved by contradiction using the prime divisibility rule.
    </div>
  </div>

</div><!-- end Q2 -->

<!-- ══════════════════════════════════════════════
     QUESTION 3 — Find numbers between given values
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-2">

  <div class="aqe-q-head">
    Question 3 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    <strong>(1)</strong> Find two irrational numbers between \(0.12\) and \(0.31\).<br><br>
    <strong>(2)</strong> Find a rational and an irrational number between \(\dfrac{1}{\sqrt{2}}\) and \(\sqrt{2}\).
  </div>

  <div class="aqe-theory">
    <div class="aqe-theory-h">📖 Theory — Numbers Between Two Values</div>
    <div class="aqe-theory-b">
      Between any two distinct real numbers, there are <strong>infinitely many</strong> rational numbers and <strong>infinitely many</strong> irrational numbers. This is called the <em>density</em> of the real numbers.<br><br>
      A practical way to find an irrational between \(a\) and \(b\): choose any non-perfect-square \(k\) with \(a^2 &lt; k &lt; b^2\). Then \(\sqrt{k}\) is irrational and lies in \((a,\, b)\).
    </div>
  </div>

  <p class="aqe-part">(1) Two irrational numbers between 0.12 and 0.31</p>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      We want \(\sqrt{k}\) with \(0.12 &lt; \sqrt{k} &lt; 0.31\). Squaring the inequality gives us the range for \(k\): square the boundaries and pick non-perfect-square values of \(k\) in between.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Find the target range for \(k\)</div>
    <div class="aqe-step-b">
      We want \(\sqrt{k}\) such that \(0.12 &lt; \sqrt{k} &lt; 0.31\). Squaring all three parts:
      $$0.12^2 \;<\; k \;<\; 0.31^2 \implies 0.0144 \;<\; k \;<\; 0.0961$$
      Choose any non-perfect-square value of \(k\) inside this range.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Choose two suitable values and verify</div>
    <div class="aqe-step-b">
      Choose \(k = 0.05\) and \(k = 0.08\) (both lie inside \(0.0144\) to \(0.0961\)):
      $$\sqrt{0.05} = \frac{\sqrt{5}}{10} \approx 0.2236 \qquad \sqrt{0.08} = \frac{\sqrt{2}}{5} \approx 0.2828$$
      Verify both lie in the interval:
      $$0.12 \;<\; 0.2236 \;<\; 0.31 \;\checkmark \qquad 0.12 \;<\; 0.2828 \;<\; 0.31 \;\checkmark$$
      Both are irrational because \(\sqrt{5}\) and \(\sqrt{2}\) are irrational, and dividing by a non-zero rational keeps them irrational.
    </div>
  </div>

  <hr class="aqe-sep">
  <p class="aqe-part">(2) A rational and an irrational number between \(\dfrac{1}{\sqrt{2}}\) and \(\sqrt{2}\)</p>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      First find the decimal values of the boundaries. Then identify a simple integer or fraction (rational) and a simple surd (irrational) that both fall strictly between them.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Find decimal values of the boundaries</div>
    <div class="aqe-step-b">
      $$\frac{1}{\sqrt{2}} = \frac{\sqrt{2}}{2} \approx 0.707 \qquad \text{and} \qquad \sqrt{2} \approx 1.414$$
      We need one rational and one irrational number strictly between \(0.707\) and \(1.414\).
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Find a rational number</div>
    <div class="aqe-step-b">
      The integer \(1\) is rational, and:
      $$0.707 \;<\; 1 \;<\; 1.414 \;\checkmark$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Find an irrational number</div>
    <div class="aqe-step-b">
      Consider \(\dfrac{\sqrt{6}}{2}\):
      $$\frac{\sqrt{6}}{2} \approx \frac{2.449}{2} \approx 1.225$$
      $$0.707 \;<\; 1.225 \;<\; 1.414 \;\checkmark$$
      \(\dfrac{\sqrt{6}}{2}\) is irrational because \(\sqrt{6}\) is irrational (6 is not a perfect square), and dividing by 2 does not make it rational.
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      <strong>(1)</strong> Two irrational numbers between 0.12 and 0.31: &nbsp;\(\dfrac{\sqrt{5}}{10} \approx 0.2236\) &nbsp;and&nbsp; \(\dfrac{\sqrt{2}}{5} \approx 0.2828\)<br><br>
      <strong>(2)</strong> Between \(\dfrac{1}{\sqrt{2}}\) and \(\sqrt{2}\): &nbsp; Rational: \(\mathbf{1}\) &nbsp;·&nbsp; Irrational: \(\dfrac{\sqrt{6}}{2}\)
    </div>
  </div>

</div><!-- end Q3 -->

<!-- ══════════════════════════════════════════════
     QUESTION 4 — Fractions to recurring decimals
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-3">

  <div class="aqe-q-head">
    Question 4 <span class="aqe-badge aqe-easy">🟢 Easy</span>
  </div>

  <div class="aqe-qtext">
    Convert the following into repeating decimal fractions:
    &emsp; <strong>1)</strong> \(\dfrac{1}{6}\) &emsp; <strong>2)</strong> \(\dfrac{7}{11}\) &emsp; <strong>4)</strong> \(3\dfrac{8}{15}\)
  </div>

  <div class="aqe-theory">
    <div class="aqe-theory-h">📖 Theory — Fractions as Recurring Decimals</div>
    <div class="aqe-theory-b">
      Every fraction \(\frac{p}{q}\) (where \(q\) has prime factors other than 2 and 5) produces a <strong>recurring decimal</strong> — a decimal where a block of digits repeats forever. The repeating block is called the <strong>recurring period</strong>.<br><br>
      To find it: perform long division. Whenever a remainder repeats, the decimal digits from that point cycle forever. We write the repeating block with an overline: \(0.\overline{63}\) means \(0.636363\ldots\)
    </div>
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Perform long division step by step. Record each remainder. As soon as a remainder appears for the second time, the decimal has started to repeat — stop and write the overline notation.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert \(\dfrac{1}{6}\)</div>
    <div class="aqe-step-b">
      Divide 1 by 6 using long division:<br><br>
      &nbsp;&nbsp;&nbsp; \(10 \div 6 = 1\) remainder \(4\)<br>
      &nbsp;&nbsp;&nbsp; \(40 \div 6 = 6\) remainder \(4\) &nbsp;← remainder repeats<br><br>
      The digit 6 repeats forever. The 1 before it is non-recurring:
      $$\frac{1}{6} = 0.1\overline{6}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Convert \(\dfrac{7}{11}\)</div>
    <div class="aqe-step-b">
      Divide 7 by 11:<br><br>
      &nbsp;&nbsp;&nbsp; \(70 \div 11 = 6\) remainder \(4\)<br>
      &nbsp;&nbsp;&nbsp; \(40 \div 11 = 3\) remainder \(7\)<br>
      &nbsp;&nbsp;&nbsp; \(70 \div 11 = 6\) remainder \(4\) &nbsp;← cycle repeats<br><br>
      The block "63" repeats from the very start:
      $$\frac{7}{11} = 0.\overline{63}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Convert \(3\dfrac{8}{15}\)</div>
    <div class="aqe-step-b">
      The whole number 3 stays as is. Convert the fractional part \(\dfrac{8}{15}\):<br><br>
      &nbsp;&nbsp;&nbsp; \(80 \div 15 = 5\) remainder \(5\)<br>
      &nbsp;&nbsp;&nbsp; \(50 \div 15 = 3\) remainder \(5\) &nbsp;← remainder repeats<br><br>
      So \(\dfrac{8}{15} = 0.5\overline{3}\), and therefore:
      $$3\frac{8}{15} = 3.5\overline{3}$$
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$\frac{1}{6} = 0.1\overline{6} \qquad \frac{7}{11} = 0.\overline{63} \qquad 3\frac{8}{15} = 3.5\overline{3}$$
    </div>
  </div>

</div><!-- end Q4 -->

<!-- ══════════════════════════════════════════════
     QUESTION 5 — Recurring decimals to fractions
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-4">

  <div class="aqe-q-head">
    Question 5 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Convert the following into simple fractions:
    &emsp; <strong>1)</strong> \(0.\overline{2}\) &emsp; <strong>2)</strong> \(0.\overline{35}\) &emsp; <strong>4)</strong> \(3.\overline{78}\)
  </div>

  <div class="aqe-theory">
    <div class="aqe-theory-h">📖 Theory — The Algebraic Cancellation Method</div>
    <div class="aqe-theory-b">
      The key insight: let \(x\) equal the recurring decimal. Multiply both sides by \(10^n\) where \(n\) is the number of digits in the repeating block. This shifts the decimal so the recurring part lines up exactly with the original. Subtracting eliminates the infinite tail — leaving a simple equation to solve.
    </div>
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      <strong>Formula — shortcut for pure recurring decimals:</strong><br>
      $$0.\overline{d_1 d_2 \cdots d_n} = \frac{\text{the recurring block}}{\underbrace{99\cdots9}_{n \text{ nines}}}$$
      For a decimal with a whole number part (like \(3.\overline{78}\)), apply the algebraic method to the full number — the whole number part cancels naturally in the subtraction.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert \(0.\overline{2} = 0.2222\ldots\)</div>
    <div class="aqe-step-b">
      Let \(x = 0.2222\ldots\)<br><br>
      Multiply by 10 (the recurring block has 1 digit):
      $$10x = 2.2222\ldots$$
      Subtract the original equation \(x = 0.2222\ldots\):
      $$10x - x = 2.2222\ldots - 0.2222\ldots$$
      $$9x = 2 \implies x = \frac{2}{9}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Convert \(0.\overline{35} = 0.353535\ldots\)</div>
    <div class="aqe-step-b">
      Let \(x = 0.353535\ldots\)<br><br>
      Multiply by 100 (the recurring block has 2 digits):
      $$100x = 35.353535\ldots$$
      Subtract: \(100x - x = 35.353535\ldots - 0.353535\ldots\)
      $$99x = 35 \implies x = \frac{35}{99}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Convert \(3.\overline{78} = 3.787878\ldots\)</div>
    <div class="aqe-step-b">
      Let \(x = 3.787878\ldots\)<br><br>
      Multiply by 100 (recurring block has 2 digits):
      $$100x = 378.787878\ldots$$
      Subtract: \(100x - x = 378.787878\ldots - 3.787878\ldots\)
      $$99x = 375 \implies x = \frac{375}{99}$$
      Simplify: \(\gcd(375, 99) = 3\), so:
      $$x = \frac{125}{33}$$
    </div>
  </div>

  <div class="aqe-note">
    <div class="aqe-note-h">📝 Note</div>
    <div class="aqe-note-b">
      Always check for common factors after the subtraction step. Here \(375 = 3 \times 125\) and \(99 = 3 \times 33\) — both divisible by 3. Dividing gives the fully simplified fraction \(\frac{125}{33}\).
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$0.\overline{2} = \frac{2}{9} \qquad 0.\overline{35} = \frac{35}{99} \qquad 3.\overline{78} = \frac{125}{33}$$
    </div>
  </div>

</div><!-- end Q5 -->

<!-- ══════════════════════════════════════════════
     QUESTION 6 — Similar recurring decimals
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-5">

  <div class="aqe-q-head">
    Question 6 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Express as <strong>similar</strong> repeating decimal fractions: &emsp; <strong>1)</strong> \(2.\overline{23}\) and \(5.\overline{235}\)
  </div>

  <div class="aqe-theory">
    <div class="aqe-theory-h">📖 Theory — Similar Recurring Decimal Fractions</div>
    <div class="aqe-theory-b">
      Two recurring decimals are called <strong>similar</strong> when they have:<br>
      &nbsp;&nbsp;• the same number of non-recurring digits after the decimal point, and<br>
      &nbsp;&nbsp;• the same length of recurring period.<br><br>
      Similar decimals are easier to add and subtract because the recurring blocks line up. To make two decimals similar, we extend each recurring block by repeating it until both reach a common period length.
    </div>
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      <strong>Step:</strong> Find the LCM of the two period lengths. Repeat each recurring block \(\frac{\text{LCM}}{\text{period}}\) times to extend it to the common length.<br><br>
      For example, a period-2 block repeated 3 times gives period 6.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Identify the period of each decimal</div>
    <div class="aqe-step-b">
      \(2.\overline{23}\): the block "23" repeats &nbsp;→&nbsp; <strong>period = 2</strong><br><br>
      \(5.\overline{235}\): the block "235" repeats &nbsp;→&nbsp; <strong>period = 3</strong><br><br>
      Both have <strong>zero</strong> non-recurring digits (the recurring part starts immediately after the decimal point). Good — no alignment needed there.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Find the LCM of the two periods</div>
    <div class="aqe-step-b">
      $$\text{LCM}(2,\; 3) = 6$$
      Both decimals must be rewritten with a recurring period of length <strong>6</strong>.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Extend each recurring block to length 6</div>
    <div class="aqe-step-b">
      For \(2.\overline{23}\): period 2 → repeat "23" three times → "232323"
      $$2.\overline{23} = 2.\overline{232323}$$
      For \(5.\overline{235}\): period 3 → repeat "235" twice → "235235"
      $$5.\overline{235} = 5.\overline{235235}$$
      Both now have period 6 and zero non-recurring digits — they are <strong>similar</strong>.
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$2.\overline{23} = 2.\overline{232323} \qquad 5.\overline{235} = 5.\overline{235235}$$
    </div>
  </div>

</div><!-- end Q6 -->

<!-- ══════════════════════════════════════════════
     QUESTION 7 — Add recurring decimals
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-6">

  <div class="aqe-q-head">
    Question 7 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Add: &emsp; \(0.\overline{45} + 0.\overline{134}\)
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Convert each recurring decimal to a fraction using the shortcut: recurring block ÷ matching number of 9s. Then add the fractions using a common denominator.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert \(0.\overline{45}\) to a fraction</div>
    <div class="aqe-step-b">
      Two recurring digits → divide by 99:
      $$0.\overline{45} = \frac{45}{99}$$
      Simplify: \(\gcd(45, 99) = 9\), so:
      $$\frac{45}{99} = \frac{5}{11}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Convert \(0.\overline{134}\) to a fraction</div>
    <div class="aqe-step-b">
      Three recurring digits → divide by 999:
      $$0.\overline{134} = \frac{134}{999}$$
      \(\gcd(134, 999) = 1\), so this is already fully simplified.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Find the LCM of the denominators</div>
    <div class="aqe-step-b">
      We need a common denominator for \(\frac{5}{11}\) and \(\frac{134}{999}\).<br><br>
      \(999 = 3^3 \times 37\). Since 11 is prime and does not divide 999:
      $$\text{LCM}(11,\; 999) = 11 \times 999 = 10989$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 4 — Add the fractions</div>
    <div class="aqe-step-b">
      $$\frac{5}{11} + \frac{134}{999} = \frac{5 \times 999}{10989} + \frac{134 \times 11}{10989} = \frac{4995 + 1474}{10989} = \frac{6469}{10989}$$
      \(\gcd(6469, 10989) = 1\), so this fraction is fully simplified.
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$0.\overline{45} + 0.\overline{134} = \frac{6469}{10989}$$
    </div>
  </div>

</div><!-- end Q7 -->

<!-- ══════════════════════════════════════════════
     QUESTION 8 — Subtract recurring decimals
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-7">

  <div class="aqe-q-head">
    Question 8 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Subtract: &emsp; <strong>1)</strong> \(3.\overline{4} - 2.\overline{13}\) &emsp;&emsp; <strong>3)</strong> \(8.\overline{49} - 5.\overline{356}\)
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      For each number, let \(x\) equal the full decimal (including the whole number part) and apply the algebraic method to convert it to a fraction. Then subtract using a common denominator.
    </div>
  </div>

  <p class="aqe-part">(1) &nbsp;\(3.\overline{4} - 2.\overline{13}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert \(3.\overline{4}\) and \(2.\overline{13}\) to fractions</div>
    <div class="aqe-step-b">
      For \(3.\overline{4} = 3.4444\ldots\): let \(x = 3.4444\ldots\), then \(10x = 34.4444\ldots\), subtract: \(9x = 31\)
      $$3.\overline{4} = \frac{31}{9}$$
      For \(2.\overline{13} = 2.1313\ldots\): let \(x = 2.1313\ldots\), then \(100x = 213.1313\ldots\), subtract: \(99x = 211\)
      $$2.\overline{13} = \frac{211}{99}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Subtract</div>
    <div class="aqe-step-b">
      Convert \(\dfrac{31}{9}\) to ninety-ninths: \(\dfrac{31}{9} = \dfrac{341}{99}\)
      $$\frac{341}{99} - \frac{211}{99} = \frac{130}{99}$$
      Converting back: \(\dfrac{130}{99} = 1.\overline{31}\)<br><br>
      <em>Check:</em> \(3.4444\ldots - 2.1313\ldots = 1.3131\ldots\; \checkmark\)
    </div>
  </div>

  <hr class="aqe-sep">
  <p class="aqe-part">(3) &nbsp;\(8.\overline{49} - 5.\overline{356}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert both decimals to fractions</div>
    <div class="aqe-step-b">
      For \(8.\overline{49} = 8.4949\ldots\): let \(x = 8.4949\ldots\), then \(100x = 849.4949\ldots\), subtract: \(99x = 841\)
      $$8.\overline{49} = \frac{841}{99}$$
      For \(5.\overline{356} = 5.356356\ldots\): let \(x = 5.356356\ldots\), then \(1000x = 5356.356356\ldots\), subtract: \(999x = 5351\)
      $$5.\overline{356} = \frac{5351}{999}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Find the LCM of 99 and 999</div>
    <div class="aqe-step-b">
      $$99 = 3^2 \times 11 \qquad 999 = 3^3 \times 37$$
      $$\text{LCM}(99,\; 999) = 3^3 \times 11 \times 37 = 10989$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Subtract</div>
    <div class="aqe-step-b">
      $$\frac{841}{99} - \frac{5351}{999} = \frac{841 \times 111}{10989} - \frac{5351 \times 11}{10989} = \frac{93351 - 58861}{10989} = \frac{34490}{10989}$$
      \(\gcd(34490, 10989) = 1\), so this is fully simplified.
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$3.\overline{4} - 2.\overline{13} = \frac{130}{99} = 1.\overline{31}$$
      $$8.\overline{49} - 5.\overline{356} = \frac{34490}{10989}$$
    </div>
  </div>

</div><!-- end Q8 -->

<!-- ══════════════════════════════════════════════
     QUESTION 9 — Multiply recurring decimals
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-8">

  <div class="aqe-q-head">
    Question 9 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Multiply: &emsp; <strong>1)</strong> \(0.\overline{3} \times 0.\overline{6}\) &emsp;&emsp; <strong>3)</strong> \(0.\overline{62} \times 0.\overline{3}\)
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Convert each recurring decimal to a fraction using the shortcut (recurring block ÷ matching 9s). Multiply the fractions. Simplify fully, and check whether the result is a recognisable recurring decimal.
    </div>
  </div>

  <p class="aqe-part">(1) &nbsp;\(0.\overline{3} \times 0.\overline{6}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert to fractions and multiply</div>
    <div class="aqe-step-b">
      $$0.\overline{3} = \frac{3}{9} = \frac{1}{3} \qquad 0.\overline{6} = \frac{6}{9} = \frac{2}{3}$$
      $$\frac{1}{3} \times \frac{2}{3} = \frac{2}{9} = 0.\overline{2}$$
    </div>
  </div>

  <hr class="aqe-sep">
  <p class="aqe-part">(3) &nbsp;\(0.\overline{62} \times 0.\overline{3}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert to fractions and multiply</div>
    <div class="aqe-step-b">
      Two recurring digits → divide by 99:
      $$0.\overline{62} = \frac{62}{99} \qquad 0.\overline{3} = \frac{1}{3}$$
      $$\frac{62}{99} \times \frac{1}{3} = \frac{62}{297}$$
      Check for common factors: \(62 = 2 \times 31\) and \(297 = 3^3 \times 11\) share none, so this is fully simplified.
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$0.\overline{3} \times 0.\overline{6} = \frac{2}{9} = 0.\overline{2}$$
      $$0.\overline{62} \times 0.\overline{3} = \frac{62}{297}$$
    </div>
  </div>

</div><!-- end Q9 -->

<!-- ══════════════════════════════════════════════
     QUESTION 10 — Divide recurring decimals
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-9">

  <div class="aqe-q-head">
    Question 10 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Divide: &emsp; <strong>1)</strong> \(0.\overline{3} \div 0.\overline{6}\) &emsp;&emsp; <strong>3)</strong> \(2.\overline{37} \div 0.\overline{45}\)
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Convert to fractions. Then <strong>divide by multiplying by the reciprocal</strong>: \(\frac{a}{b} \div \frac{c}{d} = \frac{a}{b} \times \frac{d}{c}\). Look for common factors between numerator and denominator and cancel them before multiplying.
    </div>
  </div>

  <p class="aqe-part">(1) &nbsp;\(0.\overline{3} \div 0.\overline{6}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert to fractions and divide</div>
    <div class="aqe-step-b">
      $$0.\overline{3} = \frac{1}{3} \qquad 0.\overline{6} = \frac{2}{3}$$
      $$\frac{1}{3} \div \frac{2}{3} = \frac{1}{3} \times \frac{3}{2} = \frac{1}{2} = 0.5$$
    </div>
  </div>

  <hr class="aqe-sep">
  <p class="aqe-part">(3) &nbsp;\(2.\overline{37} \div 0.\overline{45}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Convert \(2.\overline{37}\) to a fraction</div>
    <div class="aqe-step-b">
      Let \(x = 2.3737\ldots\), then \(100x = 237.3737\ldots\), subtract: \(99x = 235\)
      $$2.\overline{37} = \frac{235}{99}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Convert \(0.\overline{45}\) to a fraction</div>
    <div class="aqe-step-b">
      $$0.\overline{45} = \frac{45}{99} = \frac{5}{11}$$
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Divide and simplify</div>
    <div class="aqe-step-b">
      $$\frac{235}{99} \div \frac{5}{11} = \frac{235}{99} \times \frac{11}{5} = \frac{235 \times 11}{99 \times 5}$$
      Factor to cancel: \(235 = 5 \times 47\) and \(99 = 9 \times 11\):
      $$= \frac{\cancel{5} \times 47 \times \cancel{11}}{9 \times \cancel{11} \times \cancel{5}} = \frac{47}{9} = 5.\overline{2}$$
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      $$0.\overline{3} \div 0.\overline{6} = \frac{1}{2} = 0.5$$
      $$2.\overline{37} \div 0.\overline{45} = \frac{47}{9} = 5.\overline{2}$$
    </div>
  </div>

</div><!-- end Q10 -->

<!-- ══════════════════════════════════════════════
     QUESTION 11 — Values and 4 d.p. approximations
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-10">

  <div class="aqe-q-head">
    Question 11 <span class="aqe-badge aqe-medium">🟡 Medium</span>
  </div>

  <div class="aqe-qtext">
    Write down the exact value and approximate value to <strong>4 decimal places</strong>: &emsp; <strong>2)</strong> \(0.\overline{25}\) &emsp; <strong>3)</strong> \(1.\overline{34}\)
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Convert the recurring decimal to a fraction — that is its <strong>exact value</strong>. Then write out the decimal expansion and apply the rounding rule:<br><br>
      Look at the <strong>5th decimal digit</strong>. If it is 5 or more, round the 4th digit <em>up</em>. If it is less than 5, leave the 4th digit unchanged (round down).
    </div>
  </div>

  <p class="aqe-part">(2) &nbsp;\(0.\overline{25}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Find the exact value</div>
    <div class="aqe-step-b">
      Two recurring digits → divide by 99:
      $$0.\overline{25} = \frac{25}{99}$$
      Decimal expansion: \(0.25252525\ldots\)
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Approximate to 4 decimal places</div>
    <div class="aqe-step-b">
      The first five decimal places: \(0.2525\mathbf{2}\ldots\)<br><br>
      The 5th digit is <strong>2</strong> (less than 5) → round down (keep the 4th digit as is):
      $$0.\overline{25} \approx 0.2525$$
    </div>
  </div>

  <hr class="aqe-sep">
  <p class="aqe-part">(3) &nbsp;\(1.\overline{34}\)</p>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Find the exact value</div>
    <div class="aqe-step-b">
      $$1.\overline{34} = 1 + \frac{34}{99} = \frac{99 + 34}{99} = \frac{133}{99}$$
      Decimal expansion: \(1.34343434\ldots\)
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Approximate to 4 decimal places</div>
    <div class="aqe-step-b">
      The first five decimal places: \(1.3434\mathbf{3}\ldots\)<br><br>
      The 5th digit is <strong>3</strong> (less than 5) → round down:
      $$1.\overline{34} \approx 1.3434$$
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      <table class="aqe-tbl">
        <tr><th>Number</th><th>Exact value</th><th>Approx (4 d.p.)</th></tr>
        <tr><td>\(0.\overline{25}\)</td><td>\(\dfrac{25}{99}\)</td><td>\(0.2525\)</td></tr>
        <tr><td>\(1.\overline{34}\)</td><td>\(\dfrac{133}{99}\)</td><td>\(1.3434\)</td></tr>
      </table>
    </div>
  </div>

</div><!-- end Q11 -->

<!-- ══════════════════════════════════════════════
     QUESTION 12 — Classify rational / irrational
══════════════════════════════════════════════ -->
<div class="aqe-q arithmatex" id="aqe-q-11">

  <div class="aqe-q-head">
    Question 12 <span class="aqe-badge aqe-easy">🟢 Easy</span>
  </div>

  <div class="aqe-qtext">
    State whether each of the following is rational or irrational:
    $$\mathbf{2)}\; \sqrt{9} \qquad \mathbf{3)}\; \sqrt{11} \qquad \mathbf{5)}\; \frac{\sqrt{8}}{\sqrt{7}} \qquad \mathbf{6)}\; \frac{\sqrt{27}}{\sqrt{48}}$$
  </div>

  <div class="aqe-strat">
    <div class="aqe-strat-h">📌 Strategy</div>
    <div class="aqe-strat-b">
      Simplify each expression as far as possible. If the result is a plain integer or a fraction of two integers, it is <strong>rational</strong>. If it still contains a square root of a number that is <em>not</em> a perfect square, it is <strong>irrational</strong>.<br><br>
      <strong>Important:</strong> never assume a ratio of two surds is irrational — always simplify first.
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 1 — Classify \(\sqrt{9}\)</div>
    <div class="aqe-step-b">
      $$\sqrt{9} = 3$$
      A whole number is rational. &nbsp;→&nbsp; <span class="aqe-rat">Rational</span>
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 2 — Classify \(\sqrt{11}\)</div>
    <div class="aqe-step-b">
      Is 11 a perfect square? We know \(3^2 = 9\) and \(4^2 = 16\) — there is no integer whose square equals 11. Its decimal expansion is non-terminating and non-repeating.<br><br>
      &nbsp;→&nbsp; <span class="aqe-irr">Irrational</span>
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 3 — Classify \(\dfrac{\sqrt{8}}{\sqrt{7}}\)</div>
    <div class="aqe-step-b">
      $$\frac{\sqrt{8}}{\sqrt{7}} = \sqrt{\frac{8}{7}} = \frac{2\sqrt{2}}{\sqrt{7}} = \frac{2\sqrt{2} \cdot \sqrt{7}}{7} = \frac{2\sqrt{14}}{7}$$
      Since 14 is not a perfect square, \(\sqrt{14}\) is irrational, and so is \(\dfrac{2\sqrt{14}}{7}\).<br><br>
      &nbsp;→&nbsp; <span class="aqe-irr">Irrational</span>
    </div>
  </div>

  <div class="aqe-step">
    <div class="aqe-step-h">Step 4 — Classify \(\dfrac{\sqrt{27}}{\sqrt{48}}\)</div>
    <div class="aqe-step-b">
      $$\frac{\sqrt{27}}{\sqrt{48}} = \sqrt{\frac{27}{48}}$$
      Simplify the fraction inside: \(\dfrac{27}{48} = \dfrac{9}{16}\) (divide both by 3).
      $$\sqrt{\frac{9}{16}} = \frac{\sqrt{9}}{\sqrt{16}} = \frac{3}{4}$$
      Since both 9 and 16 are perfect squares, the result is a fraction of integers.<br><br>
      &nbsp;→&nbsp; <span class="aqe-rat">Rational</span>
    </div>
  </div>

  <div class="aqe-note">
    <div class="aqe-note-h">📝 Note</div>
    <div class="aqe-note-b">
      \(\dfrac{\sqrt{27}}{\sqrt{48}}\) looks like it should be irrational — but after simplifying \(\frac{27}{48} = \frac{9}{16}\), both numerator and denominator are perfect squares, so the surds cancel out completely and give a rational answer \(\frac{3}{4}\). Always simplify before concluding.
    </div>
  </div>

  <div class="aqe-ans">
    <div class="aqe-ans-h">✅ Final Answer</div>
    <div class="aqe-ans-b">
      <table class="aqe-tbl">
        <tr><th>Expression</th><th>Simplified form</th><th>Type</th></tr>
        <tr><td>\(\sqrt{9}\)</td><td>\(3\)</td><td class="aqe-rat">Rational</td></tr>
        <tr><td>\(\sqrt{11}\)</td><td>\(\sqrt{11}\)</td><td class="aqe-irr">Irrational</td></tr>
        <tr><td>\(\dfrac{\sqrt{8}}{\sqrt{7}}\)</td><td>\(\dfrac{2\sqrt{14}}{7}\)</td><td class="aqe-irr">Irrational</td></tr>
        <tr><td>\(\dfrac{\sqrt{27}}{\sqrt{48}}\)</td><td>\(\dfrac{3}{4}\)</td><td class="aqe-rat">Rational</td></tr>
      </table>
    </div>
  </div>

</div><!-- end Q12 -->

<!-- ══════════════════════════════════════════════
     BOTTOM NAVIGATION
══════════════════════════════════════════════ -->
<div class="aqe-nav" style="margin-top:1.5rem;">
  <button class="aqe-btn aqe-btn-prev">← Previous</button>
  <span class="aqe-counter">Question 1 of 12</span>
  <button class="aqe-btn aqe-btn-next">Next →</button>
</div>

</div><!-- end #aqe -->

<script>
(function () {
  var container = document.getElementById('aqe');
  if (!container) return;

  var items   = container.querySelectorAll('.aqe-q');
  var total   = items.length;
  var current = 0;
  var typeset = {};
  typeset[0]  = true; /* Q1 is visible on load — MathJax handles it */

  /* ── Show question N ── */
  function show(n) {
    items[current].classList.remove('aqe-active');
    current = n;
    items[current].classList.add('aqe-active');

    /* Typeset math in this question if not yet done */
    if (!typeset[current] && window.MathJax && MathJax.typesetPromise) {
      MathJax.typesetPromise([items[current]]).catch(function () {});
      typeset[current] = true;
    }

    updateNav();
    container.scrollIntoView({ behavior: 'smooth', block: 'start' });
  }

  /* ── Update button visibility and counter ── */
  function updateNav() {
    container.querySelectorAll('.aqe-btn-prev').forEach(function (b) {
      b.style.visibility = (current === 0) ? 'hidden' : 'visible';
    });
    container.querySelectorAll('.aqe-btn-next').forEach(function (b) {
      b.style.visibility = (current === total - 1) ? 'hidden' : 'visible';
    });
    container.querySelectorAll('.aqe-counter').forEach(function (c) {
      c.textContent = 'Question ' + (current + 1) + ' of ' + total;
    });
  }

  /* ── Wire up buttons ── */
  container.querySelectorAll('.aqe-btn-prev').forEach(function (b) {
    b.addEventListener('click', function () {
      if (current > 0) show(current - 1);
    });
  });
  container.querySelectorAll('.aqe-btn-next').forEach(function (b) {
    b.addEventListener('click', function () {
      if (current < total - 1) show(current + 1);
    });
  });

  updateNav();
})();
</script>
