---
hide:
  - toc
---

<style>
.ex-page { max-width: 860px; margin: 0 auto; }
.q-nav { display: flex; justify-content: space-between; align-items: center; padding: 0.5rem 0; margin-bottom: 0.8rem; }
.q-nav-btn { background: linear-gradient(135deg, #f39c12, #e67e22); color: #fff; border: none; border-radius: 8px; padding: 0.5rem 1.2rem; font-size: 0.92rem; font-weight: 600; cursor: pointer; transition: opacity 0.15s; }
.q-nav-btn:hover { opacity: 0.85; }
.q-counter { color: #777; font-size: 0.88rem; font-weight: 500; }
.q-nav-spacer { min-width: 110px; }
.q-header { background: linear-gradient(135deg, #f39c12, #e67e22); color: #fff; padding: 0.9rem 1.4rem; border-radius: 12px 12px 0 0; font-size: 1.08rem; font-weight: 700; }
.q-body { background: #fff; border: 1px solid #dde3ea; border-top: none; border-radius: 0 0 12px 12px; padding: 1.4rem 1.6rem; box-shadow: 0 3px 10px rgba(0,0,0,.06); margin-bottom: 1rem; color: #1a1a1a; }
.badge { display: inline-block; padding: 0.2rem 0.65rem; border-radius: 20px; font-size: 0.8rem; font-weight: 700; margin-left: 0.5rem; vertical-align: middle; }
.badge-easy   { background: #e8f5e9; color: #2e7d32; }
.badge-medium { background: #fff8e1; color: #e65100; }
.badge-hard   { background: #fce4ec; color: #b71c1c; }
.q-text { font-size: 1.05rem; line-height: 1.75; color: #1a1a1a; margin: 0 0 0.8rem; }
.q-options { margin: 0.2rem 0 1rem 0; padding-left: 1.4rem; }
.q-options li { margin: 0.45rem 0; font-size: 1rem; }
.part-label { font-weight: 700; font-size: 1rem; color: #e67e22; margin: 1rem 0 0.3rem; }
.part-hr { border: none; border-top: 2px dashed #e2e8f0; margin: 1.2rem 0; }
.theory-box { border-radius: 10px; overflow: hidden; margin: 1rem 0; }
.theory-header { background: #1a3a5c; color: #fff; padding: 0.5rem 1rem; font-size: 0.82rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; }
.theory-body { background: #e8f4fd; border: 1px solid #b3d7f0; border-top: none; padding: 0.95rem 1.2rem; font-size: 0.97rem; line-height: 1.8; color: #1a3a5c; }
.formula-box { border-radius: 10px; overflow: hidden; margin: 0.8rem 0; }
.formula-header { background: #4a235a; color: #fff; padding: 0.5rem 1rem; font-size: 0.82rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; }
.formula-body { background: #f5eef8; border: 1px solid #d2b4de; border-top: none; padding: 0.9rem 1.2rem; font-size: 0.97rem; line-height: 1.9; color: #4a235a; }
.strategy-box { border-radius: 10px; overflow: hidden; margin: 1rem 0; }
.strategy-header { background: #0d7d6b; color: #fff; padding: 0.5rem 1rem; font-size: 0.82rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; }
.strategy-body { background: #e6f7f4; border: 1px solid #a7d9d0; border-top: none; padding: 0.95rem 1.2rem; font-size: 0.97rem; line-height: 1.8; color: #0a4d3e; }
.step-box { background: #fafafa; border: 1px solid #dde3ea; border-left: 4px solid #e67e22; border-radius: 8px; padding: 0.9rem 1.2rem; margin: 0.8rem 0; }
.step-label { font-weight: 700; font-size: 0.88rem; color: #e67e22; letter-spacing: 0.04em; margin-bottom: 0.5rem; }
.step-body { font-size: 0.97rem; line-height: 1.9; color: #2d2d2d; }
.note-box { border-radius: 10px; overflow: hidden; margin: 0.8rem 0; }
.note-header { background: #f39c12; color: #fff; padding: 0.45rem 1rem; font-size: 0.82rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; }
.note-body { background: #fef9ec; border: 1px solid #f5d87a; border-top: none; padding: 0.85rem 1.2rem; font-size: 0.95rem; line-height: 1.75; color: #7d4e00; }
.final-box { border-radius: 10px; overflow: hidden; margin: 1.2rem 0 0.4rem; }
.final-header { background: linear-gradient(135deg, #27ae60, #2ecc71); color: #fff; padding: 0.5rem 1rem; font-size: 0.82rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; }
.final-body { background: #eafaf1; border: 1px solid #a8dfbb; border-top: none; padding: 1rem 1.2rem; font-size: 1rem; line-height: 1.85; color: #1a5935; }
</style>

# Exercise 1.1 — Real Numbers

<div class="ex-page">

<!-- ══════════════════════════════════════════════════════════
     QUESTION 1  —  Which number is irrational?  (Easy)
════════════════════════════════════════════════════════════ -->
<div id="q1" class="question-block">
<div class="q-nav">
  <div class="q-nav-spacer"></div>
  <span class="q-counter">Question 1 of 13</span>
  <button class="q-nav-btn" onclick="showQ(2)">Next ▶</button>
</div>
<div class="q-header">Question 1 <span class="badge badge-easy">🟢 Easy</span></div>
<div class="q-body">

<p class="q-text">Which of the following numbers is irrational?</p>
<ol class="q-options">
  <li class="arithmatex">\( 0.\dot{3} \)</li>
  <li class="arithmatex">\( \sqrt{\dfrac{16}{9}} \)</li>
  <li class="arithmatex">\( \sqrt[3]{\dfrac{8}{27}} \)</li>
  <li class="arithmatex">\( \dfrac{5}{\sqrt{3}} \)</li>
</ol>

<div class="theory-box">
<div class="theory-header">Theory — Rational and Irrational Numbers</div>
<div class="theory-body arithmatex">
A <strong>rational number</strong> can be written as \( \dfrac{p}{q} \), where \( p \) and \( q \) are integers and \( q \neq 0 \). This includes all integers, all terminating decimals, and all recurring decimals (since they repeat a fixed pattern).<br><br>
An <strong>irrational number</strong> cannot be written as \( \dfrac{p}{q} \). Its decimal expansion goes on forever with no repeating pattern. Examples: \( \sqrt{2},\ \sqrt{3},\ \pi \).<br><br>
<strong>Key tests:</strong><br>
• If \( \sqrt{n} \) simplifies to a whole number or a fraction → rational.<br>
• If \( \sqrt{n} \) cannot simplify (because \( n \) is not a perfect square) → irrational.<br>
• A non-zero rational ÷ an irrational = irrational.
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Simplify each option completely. If it reduces to a fraction or integer, it is rational. If an irreducible square (or cube) root remains, it is irrational.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 1 — Simplify option 1: \( 0.\dot{3} \)</div>
<div class="step-body arithmatex">
\( 0.\dot{3} \) means \( 0.3333\ldots \) — a recurring decimal. Every recurring decimal equals a fraction:
\[ 0.\dot{3} = \frac{1}{3} \]
This is a ratio of two integers. It is <strong>rational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Simplify option 2: \( \sqrt{\dfrac{16}{9}} \)</div>
<div class="step-body arithmatex">
Take the square root of the numerator and denominator separately:
\[ \sqrt{\frac{16}{9}} = \frac{\sqrt{16}}{\sqrt{9}} = \frac{4}{3} \]
Both 16 and 9 are perfect squares, so the result is a simple fraction. It is <strong>rational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Simplify option 3: \( \sqrt[3]{\dfrac{8}{27}} \)</div>
<div class="step-body arithmatex">
Take the cube root of numerator and denominator separately:
\[ \sqrt[3]{\frac{8}{27}} = \frac{\sqrt[3]{8}}{\sqrt[3]{27}} = \frac{2}{3} \]
Since \( 2^3 = 8 \) and \( 3^3 = 27 \), both are perfect cubes. Result is a fraction. It is <strong>rational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Simplify option 4: \( \dfrac{5}{\sqrt{3}} \)</div>
<div class="step-body arithmatex">
The denominator contains \( \sqrt{3} \). Since 3 is not a perfect square, \( \sqrt{3} \) is irrational — it cannot be expressed as a fraction.<br><br>
Dividing the rational number 5 by the irrational \( \sqrt{3} \) always gives an irrational result.<br><br>
Therefore \( \dfrac{5}{\sqrt{3}} \) is <strong>irrational</strong>.
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
The answer is option <strong>4</strong>. The number \( \dfrac{5}{\sqrt{3}} \) is irrational.<br>
Options 1–3 are all rational: \( 0.\dot{3} = \dfrac{1}{3} \), \( \sqrt{\dfrac{16}{9}} = \dfrac{4}{3} \), \( \sqrt[3]{\dfrac{8}{27}} = \dfrac{2}{3} \).
</div>
</div>

<div class="q-nav">
  <div class="q-nav-spacer"></div>
  <span class="q-counter">Question 1 of 13</span>
  <button class="q-nav-btn" onclick="showQ(2)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 2  —  Classify rational / irrational  (Easy)
════════════════════════════════════════════════════════════ -->
<div id="q2" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(1)">◀ Previous</button>
  <span class="q-counter">Question 2 of 13</span>
  <button class="q-nav-btn" onclick="showQ(3)">Next ▶</button>
</div>
<div class="q-header">Question 2 <span class="badge badge-easy">🟢 Easy</span></div>
<div class="q-body">

<p class="q-text arithmatex">State whether each of the following is rational or irrational, giving a reason.</p>
<ol class="q-options">
  <li class="arithmatex">\( 0.\dot{4} \)</li>
  <li class="arithmatex">\( \sqrt{9} \)</li>
  <li class="arithmatex">\( \sqrt{11} \)</li>
  <li class="arithmatex">\( \dfrac{\sqrt{27}}{\sqrt{48}} \)</li>
  <li class="arithmatex">\( 5.\dot{6}3\dot{9} \)</li>
</ol>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
For each number, ask: can it be written as \( \dfrac{p}{q} \)?<br>
• Recurring decimals → always rational (they convert to fractions).<br>
• \( \sqrt{n} \) → rational if \( n \) is a perfect square, irrational otherwise.<br>
• A ratio of surds: simplify first — the surds may cancel.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 1 — Classify \( 0.\dot{4} \)</div>
<div class="step-body arithmatex">
\( 0.\dot{4} = 0.4444\ldots \) is a recurring decimal. All recurring decimals are rational:
\[ 0.\dot{4} = \frac{4}{9} \]
It is <strong>rational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Classify \( \sqrt{9} \)</div>
<div class="step-body arithmatex">
Since \( 3^2 = 9 \), the number 9 is a perfect square:
\[ \sqrt{9} = 3 \]
The result is a whole number, which is rational. It is <strong>rational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Classify \( \sqrt{11} \)</div>
<div class="step-body arithmatex">
The perfect squares either side of 11 are \( 3^2 = 9 \) and \( 4^2 = 16 \). Since 11 lies strictly between them, it is not a perfect square.<br><br>
Therefore \( \sqrt{11} \) cannot be simplified to a fraction. It is <strong>irrational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Classify \( \dfrac{\sqrt{27}}{\sqrt{48}} \)</div>
<div class="step-body arithmatex">
Combine the square roots into one:
\[ \frac{\sqrt{27}}{\sqrt{48}} = \sqrt{\frac{27}{48}} \]
Simplify the fraction (GCD of 27 and 48 is 3):
\[ \sqrt{\frac{27}{48}} = \sqrt{\frac{9}{16}} = \frac{\sqrt{9}}{\sqrt{16}} = \frac{3}{4} \]
The irrational parts cancelled. The result is a simple fraction. It is <strong>rational</strong>.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 5 — Classify \( 5.\dot{6}3\dot{9} \)</div>
<div class="step-body arithmatex">
The notation \( 5.\dot{6}3\dot{9} \) means the digits 6, 3, 9 repeat: \( 5.639639639\ldots \)<br><br>
This is a recurring decimal, so it can be written as a fraction. It is <strong>rational</strong>.
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
<strong>Rational:</strong> \( 0.\dot{4} \), \( \sqrt{9} \), \( \dfrac{\sqrt{27}}{\sqrt{48}} \), \( 5.\dot{6}3\dot{9} \)<br>
<strong>Irrational:</strong> \( \sqrt{11} \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(1)">◀ Previous</button>
  <span class="q-counter">Question 2 of 13</span>
  <button class="q-nav-btn" onclick="showQ(3)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 3  —  Convert fractions to recurring decimals  (Easy)
════════════════════════════════════════════════════════════ -->
<div id="q3" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(2)">◀ Previous</button>
  <span class="q-counter">Question 3 of 13</span>
  <button class="q-nav-btn" onclick="showQ(4)">Next ▶</button>
</div>
<div class="q-header">Question 3 <span class="badge badge-easy">🟢 Easy</span></div>
<div class="q-body">

<p class="q-text">Convert the following into recurring decimal fractions:</p>
<ol class="q-options">
  <li class="arithmatex">\( \dfrac{1}{6} \)</li>
  <li class="arithmatex">\( \dfrac{7}{11} \)</li>
  <li class="arithmatex">\( 3\dfrac{8}{15} \)</li>
</ol>

<div class="theory-box">
<div class="theory-header">Theory — Recurring Decimals</div>
<div class="theory-body arithmatex">
When you divide one integer by another using long division, the remainder eventually repeats — because there are only finitely many possible remainders. Once a remainder repeats, the decimal digits from that point on repeat forever. This is called a <strong>recurring (repeating) decimal</strong>.<br><br>
Notation: a dot above a digit means that digit repeats. Dots above the <em>first</em> and <em>last</em> digits of a group mean that whole group repeats. For example:<br>
\( 0.\dot{3} = 0.3333\ldots \) and \( 0.\dot{6}\dot{3} = 0.636363\ldots \)
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Perform long division. Divide the numerator by the denominator, continuing past the decimal point. Watch the remainders — when a remainder repeats, you have found the recurring block. For a mixed number, convert the fractional part only, then attach the whole number.
</div>
</div>

<div class="part-label">(a) \( \dfrac{1}{6} \)</div>

<div class="step-box">
<div class="step-label">Step 1 — Divide 1 by 6 step by step</div>
<div class="step-body arithmatex">
\( 1 \div 6 \): since \( 1 < 6 \), place a decimal point and work with 10, then 40, and so on.<br><br>
• \( 10 \div 6 = 1 \) remainder \( 4 \) → write digit <strong>1</strong> after the decimal point<br>
• Append a zero to the remainder: \( 40 \div 6 = 6 \) remainder \( 4 \) → write digit <strong>6</strong><br>
• Append a zero to the remainder: \( 40 \div 6 = 6 \) remainder \( 4 \) → write digit <strong>6</strong> again<br><br>
The remainder 4 never changes, so the digit 6 repeats forever.
\[ \frac{1}{6} = 0.1\dot{6} = 0.1666\ldots \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) \( \dfrac{7}{11} \)</div>

<div class="step-box">
<div class="step-label">Step 2 — Divide 7 by 11 step by step</div>
<div class="step-body arithmatex">
\( 7 \div 11 \): since \( 7 < 11 \), place a decimal point and work with 70, then 40, then 70 again.<br><br>
• \( 70 \div 11 = 6 \) remainder \( 4 \) → write digit <strong>6</strong><br>
• Append a zero to the remainder: \( 40 \div 11 = 3 \) remainder \( 7 \) → write digit <strong>3</strong><br>
• Append a zero to the remainder: \( 70 \div 11 = 6 \) remainder \( 4 \) → back to the start<br><br>
The remainder cycle \( 4 \to 7 \to 4 \to \cdots \) repeats, so the two-digit block "63" recurs forever.
\[ \frac{7}{11} = 0.\dot{6}\dot{3} = 0.6363\ldots \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(c) \( 3\dfrac{8}{15} \)</div>

<div class="step-box">
<div class="step-label">Step 3 — Separate the whole number and convert the fraction</div>
<div class="step-body arithmatex">
Write \( 3\dfrac{8}{15} = 3 + \dfrac{8}{15} \).<br><br>
Now divide 8 by 15 step by step:<br><br>
• \( 80 \div 15 = 5 \) remainder \( 5 \) → write digit <strong>5</strong><br>
• Append a zero to the remainder: \( 50 \div 15 = 3 \) remainder \( 5 \) → write digit <strong>3</strong><br>
• Append a zero to the remainder: \( 50 \div 15 = 3 \) remainder \( 5 \) → back to the same remainder<br><br>
The remainder 5 repeats indefinitely, so only the digit 3 recurs.
\[ \frac{8}{15} = 0.5\dot{3} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Attach the whole number</div>
<div class="step-body arithmatex">
\[ 3\frac{8}{15} = 3 + 0.5\dot{3} = 3.5\dot{3} \]
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) \( \dfrac{1}{6} = 0.1\dot{6} \)<br>
(b) \( \dfrac{7}{11} = 0.\dot{6}\dot{3} \)<br>
(c) \( 3\dfrac{8}{15} = 3.5\dot{3} \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(2)">◀ Previous</button>
  <span class="q-counter">Question 3 of 13</span>
  <button class="q-nav-btn" onclick="showQ(4)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 4  —  Values and approximations  (Easy)
════════════════════════════════════════════════════════════ -->
<div id="q4" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(3)">◀ Previous</button>
  <span class="q-counter">Question 4 of 13</span>
  <button class="q-nav-btn" onclick="showQ(5)">Next ▶</button>
</div>
<div class="q-header">Question 4 <span class="badge badge-easy">🟢 Easy</span></div>
<div class="q-body">

<p class="q-text">Write down the value and the approximate value correct to 4 decimal places:</p>
<ol class="q-options">
  <li class="arithmatex">\( 12 \)</li>
  <li class="arithmatex">\( 0.\dot{2}\dot{5} \)</li>
  <li class="arithmatex">\( 1.\dot{3}\dot{4} \)</li>
  <li class="arithmatex">\( 5.1\dot{3}0\dot{2} \)</li>
</ol>

<div class="theory-box">
<div class="theory-header">Theory — Approximating to Decimal Places</div>
<div class="theory-body arithmatex">
To approximate a number to 4 decimal places:<br>
1. Write out the decimal until you have at least 5 digits after the point.<br>
2. Look at the <strong>5th decimal digit</strong>:<br>
&nbsp;&nbsp;&nbsp;• If it is <strong>5 or more</strong> → round the 4th digit <em>up</em> by 1.<br>
&nbsp;&nbsp;&nbsp;• If it is <strong>less than 5</strong> → leave the 4th digit unchanged (round down).<br>
3. Drop all digits from the 5th place onward.
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
First write the full decimal expansion by identifying the repeating block. Then read the first four decimal places, check the fifth, and round accordingly.
</div>
</div>

<div class="part-label">(a) \( 12 \)</div>

<div class="step-box">
<div class="step-label">Step 1 — Write the exact value and approximate</div>
<div class="step-body arithmatex">
12 is a whole number. Its decimal expansion is \( 12.000000\ldots \) — all zeros, no recurring part.<br><br>
<strong>Exact value:</strong> \( 12 \)<br>
<strong>Approximate value (4 d.p.):</strong> \( 12.0000 \)
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) \( 0.\dot{2}\dot{5} \)</div>

<div class="step-box">
<div class="step-label">Step 2 — Write the expansion and approximate</div>
<div class="step-body arithmatex">
\( 0.\dot{2}\dot{5} \) means the block "25" repeats:
\[ 0.\dot{2}\dot{5} = 0.25252525\ldots \]
The decimal digits are: 2, 5, 2, 5, 2, 5, …<br><br>
4 decimal places: <strong>0.2525</strong><br>
5th digit: 2 → less than 5, so round down (keep 4th digit as 5).<br><br>
<strong>Approximate value (4 d.p.):</strong> \( 0.2525 \)
</div>
</div>

<hr class="part-hr">
<div class="part-label">(c) \( 1.\dot{3}\dot{4} \)</div>

<div class="step-box">
<div class="step-label">Step 3 — Write the expansion and approximate</div>
<div class="step-body arithmatex">
\( 1.\dot{3}\dot{4} \) means the block "34" repeats:
\[ 1.\dot{3}\dot{4} = 1.34343434\ldots \]
Decimal digits after the point: 3, 4, 3, 4, 3, 4, …<br><br>
4 decimal places: <strong>1.3434</strong><br>
5th digit: 3 → less than 5, so round down.<br><br>
<strong>Approximate value (4 d.p.):</strong> \( 1.3434 \)
</div>
</div>

<hr class="part-hr">
<div class="part-label">(d) \( 5.1\dot{3}0\dot{2} \)</div>

<div class="step-box">
<div class="step-label">Step 4 — Write the expansion and approximate</div>
<div class="step-body arithmatex">
\( 5.1\dot{3}0\dot{2} \) means the block "302" repeats after the initial 1:
\[ 5.1\dot{3}0\dot{2} = 5.1302302302\ldots \]
Decimal digits after the point: 1, 3, 0, 2, 3, 0, 2, …<br><br>
4 decimal places: <strong>5.1302</strong><br>
5th digit: 3 → less than 5, so round down.<br><br>
<strong>Approximate value (4 d.p.):</strong> \( 5.1302 \)
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) \( 12 \) — exact: \( 12 \), approx: \( 12.0000 \)<br>
(b) \( 0.\dot{2}\dot{5} = 0.2525\overline{25}\ldots \) — approx: \( 0.2525 \)<br>
(c) \( 1.\dot{3}\dot{4} = 1.3434\overline{34}\ldots \) — approx: \( 1.3434 \)<br>
(d) \( 5.1\dot{3}0\dot{2} = 5.1302\overline{302}\ldots \) — approx: \( 5.1302 \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(3)">◀ Previous</button>
  <span class="q-counter">Question 4 of 13</span>
  <button class="q-nav-btn" onclick="showQ(5)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 5  —  Convert recurring decimals to fractions  (Medium)
════════════════════════════════════════════════════════════ -->
<div id="q5" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(4)">◀ Previous</button>
  <span class="q-counter">Question 5 of 13</span>
  <button class="q-nav-btn" onclick="showQ(6)">Next ▶</button>
</div>
<div class="q-header">Question 5 <span class="badge badge-medium">🟡 Medium</span></div>
<div class="q-body">

<p class="q-text">Convert the following recurring decimals into simple fractions:</p>
<ol class="q-options">
  <li class="arithmatex">\( 0.\dot{2} \)</li>
  <li class="arithmatex">\( 0.3\dot{5} \)</li>
  <li class="arithmatex">\( 3.7\dot{8} \)</li>
</ol>

<div class="theory-box">
<div class="theory-header">Theory — The Algebraic Method</div>
<div class="theory-body arithmatex">
The trick is to use multiplication to shift the decimal so that two versions of the same number can be subtracted, making the recurring part disappear.<br><br>
<strong>Key rule:</strong> If there are \( d \) non-recurring decimal digits and \( n \) recurring digits, multiply by \( 10^{d+n} \) and by \( 10^d \), then subtract. This cancels the recurring tail.
</div>
</div>

<div class="formula-box">
<div class="formula-header">Formula — Recurring Decimal to Fraction</div>
<div class="formula-body arithmatex">
For a recurring decimal with \( d \) non-recurring digits after the point and \( n \) recurring digits:
\[ \text{Fraction} = \frac{\text{(all digits up to end of one period)} - \text{(non-recurring digits only)}}{\underbrace{99\ldots9}_{n}\underbrace{00\ldots0}_{d}} \]
The denominator has \( n \) nines followed by \( d \) zeros.
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Let \( x \) equal the recurring decimal. Multiply by the right powers of 10 to shift the decimal, then subtract to eliminate the repeating part. Solve for \( x \) and simplify the fraction.
</div>
</div>

<div class="part-label">(a) \( 0.\dot{2} \)</div>

<div class="step-box">
<div class="step-label">Step 1 — Set up the equation</div>
<div class="step-body arithmatex">
Let \( x = 0.\dot{2} = 0.2222\ldots \)<br><br>
There are 0 non-recurring digits and 1 recurring digit, so multiply by \( 10^1 = 10 \):
\[ 10x = 2.2222\ldots \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Subtract to remove the recurring part</div>
<div class="step-body arithmatex">
\[ 10x - x = 2.2222\ldots - 0.2222\ldots \]
\[ 9x = 2 \]
\[ x = \frac{2}{9} \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) \( 0.3\dot{5} \)</div>

<div class="step-box">
<div class="step-label">Step 3 — Set up the equation</div>
<div class="step-body arithmatex">
Let \( x = 0.3\dot{5} = 0.35555\ldots \)<br><br>
There is 1 non-recurring digit (3) and 1 recurring digit (5). Multiply by \( 10^1 = 10 \) and by \( 10^{1+1} = 100 \):
\[ 10x = 3.5555\ldots \]
\[ 100x = 35.5555\ldots \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Subtract to remove the recurring part</div>
<div class="step-body arithmatex">
\[ 100x - 10x = 35.5555\ldots - 3.5555\ldots \]
\[ 90x = 32 \]
\[ x = \frac{32}{90} = \frac{16}{45} \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(c) \( 3.7\dot{8} \)</div>

<div class="step-box">
<div class="step-label">Step 5 — Set up the equation</div>
<div class="step-body arithmatex">
Let \( x = 3.7\dot{8} = 3.7888\ldots \)<br><br>
There is 1 non-recurring digit after the decimal point (7) and 1 recurring digit (8). Multiply by \( 10 \) and by \( 100 \):
\[ 10x = 37.888\ldots \]
\[ 100x = 378.888\ldots \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 6 — Subtract and solve</div>
<div class="step-body arithmatex">
\[ 100x - 10x = 378.888\ldots - 37.888\ldots \]
\[ 90x = 341 \]
\[ x = \frac{341}{90} \]
This fraction is already in its simplest form (GCD of 341 and 90 is 1).
</div>
</div>

<div class="note-box">
<div class="note-header">Note</div>
<div class="note-body arithmatex">
To check: \( \dfrac{341}{90} = 3.7888\ldots \) ✓ (divide 341 ÷ 90 to verify).
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) \( 0.\dot{2} = \dfrac{2}{9} \)<br>
(b) \( 0.3\dot{5} = \dfrac{16}{45} \)<br>
(c) \( 3.7\dot{8} = \dfrac{341}{90} \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(4)">◀ Previous</button>
  <span class="q-counter">Question 5 of 13</span>
  <button class="q-nav-btn" onclick="showQ(6)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 6  —  Similar recurring decimals  (Medium)
════════════════════════════════════════════════════════════ -->
<div id="q6" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(5)">◀ Previous</button>
  <span class="q-counter">Question 6 of 13</span>
  <button class="q-nav-btn" onclick="showQ(7)">Next ▶</button>
</div>
<div class="q-header">Question 6 <span class="badge badge-medium">🟡 Medium</span></div>
<div class="q-body">

<p class="q-text arithmatex">Express the following as similar recurring decimal fractions:</p>
<p class="arithmatex" style="margin-left:1.4rem;">\( 2.\dot{2}\dot{3} \) and \( 5.\dot{2}3\dot{5} \)</p>

<div class="theory-box">
<div class="theory-header">Theory — Similar Recurring Decimals</div>
<div class="theory-body arithmatex">
Two recurring decimals are called <strong>similar</strong> when their repeating blocks have the same number of digits (the same <em>period length</em>).<br><br>
This matters for addition and subtraction: you can only add or subtract recurring decimals digit-by-digit when their periods are the same length.<br><br>
<strong>How to make them similar:</strong><br>
If one decimal has period length \( p \) and another has period length \( q \), extend both periods to the LCM of \( p \) and \( q \) by writing the repeating block multiple times.
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
1. Find the period length of each decimal.<br>
2. Find the LCM of those two period lengths.<br>
3. Rewrite each decimal with the period repeated enough times so that the total period length equals the LCM.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 1 — Identify the period of each decimal</div>
<div class="step-body arithmatex">
\( 2.\dot{2}\dot{3} = 2.232323\ldots \) → repeating block is "23" → <strong>period length = 2</strong><br><br>
\( 5.\dot{2}3\dot{5} = 5.235235235\ldots \) → repeating block is "235" → <strong>period length = 3</strong>
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Find the LCM of the two period lengths</div>
<div class="step-body arithmatex">
LCM(2, 3) = 6<br><br>
We need to rewrite both decimals so that their repeating block is 6 digits long.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Extend each decimal to period length 6</div>
<div class="step-body arithmatex">
<strong>For \( 2.\dot{2}\dot{3} \)</strong> (period 2, need period 6 = 3 repetitions):<br>
Write the block "23" three times: 23|23|23<br>
\[ 2.\dot{2}\dot{3} = 2.\dot{2}3232\dot{3} \]
<br>
<strong>For \( 5.\dot{2}3\dot{5} \)</strong> (period 3, need period 6 = 2 repetitions):<br>
Write the block "235" twice: 235|235<br>
\[ 5.\dot{2}3\dot{5} = 5.\dot{2}3523\dot{5} \]
<br>
Both now have period length 6, so they are <strong>similar</strong>.
</div>
</div>

<div class="note-box">
<div class="note-header">Note</div>
<div class="note-body arithmatex">
Repeating the block does not change the value of the decimal — it just rewrites it with a longer period. For example, \( 0.\dot{3} = 0.\dot{3}\dot{3} = 0.333\ldots \) regardless of how you group it.
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
\( 2.\dot{2}\dot{3} = 2.\dot{2}3232\dot{3} \)<br>
\( 5.\dot{2}3\dot{5} = 5.\dot{2}3523\dot{5} \)<br><br>
Both now have period length 6 and are <strong>similar recurring decimals</strong>.
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(5)">◀ Previous</button>
  <span class="q-counter">Question 6 of 13</span>
  <button class="q-nav-btn" onclick="showQ(7)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 7  —  Add recurring decimals  (Medium)
════════════════════════════════════════════════════════════ -->
<div id="q7" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(6)">◀ Previous</button>
  <span class="q-counter">Question 7 of 13</span>
  <button class="q-nav-btn" onclick="showQ(8)">Next ▶</button>
</div>
<div class="q-header">Question 7 <span class="badge badge-medium">🟡 Medium</span></div>
<div class="q-body">

<p class="q-text arithmatex">Add: \( 0.4\dot{5} + 0.1\dot{3}\dot{4} \)</p>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Convert each recurring decimal to a fraction using the algebraic method, add the fractions, then convert the result back to a decimal. This is more reliable than trying to add recurring decimals directly.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 1 — Convert \( 0.4\dot{5} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 0.4\dot{5} = 0.45555\ldots \)<br>
1 non-recurring digit (4), 1 recurring digit (5) → multiply by 10 and 100:
\[ 10x = 4.5555\ldots \]
\[ 100x = 45.5555\ldots \]
Subtract:
\[ 90x = 41 \implies x = \frac{41}{90} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Convert \( 0.1\dot{3}\dot{4} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 0.1\dot{3}\dot{4} = 0.13434\ldots \)<br>
1 non-recurring digit (1), 2 recurring digits (34) → multiply by 10 and 1000:
\[ 10x = 1.3434\ldots \]
\[ 1000x = 134.3434\ldots \]
Subtract:
\[ 990x = 133 \implies x = \frac{133}{990} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Add the two fractions</div>
<div class="step-body arithmatex">
\[ \frac{41}{90} + \frac{133}{990} \]
The LCM of 90 and 990 is 990. Convert the first fraction:
\[ \frac{41}{90} = \frac{41 \times 11}{990} = \frac{451}{990} \]
Now add:
\[ \frac{451}{990} + \frac{133}{990} = \frac{584}{990} \]
Simplify (GCD of 584 and 990 is 2):
\[ \frac{584}{990} = \frac{292}{495} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Convert the result back to a decimal</div>
<div class="step-body arithmatex">
Divide 292 by 495 using long division:<br><br>
\( 2920 \div 495 = 5 \) remainder 445<br>
\( 4450 \div 495 = 8 \) remainder 490<br>
\( 4900 \div 495 = 9 \) remainder 445<br>
\( 4450 \div 495 = 8 \) remainder 490 — the pair (8, 9) repeats.
\[ \frac{292}{495} = 0.5\dot{8}\dot{9} \]
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
\[ 0.4\dot{5} + 0.1\dot{3}\dot{4} = \frac{292}{495} = 0.5\dot{8}\dot{9} \]
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(6)">◀ Previous</button>
  <span class="q-counter">Question 7 of 13</span>
  <button class="q-nav-btn" onclick="showQ(8)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 8  —  Subtract recurring decimals  (Medium)
════════════════════════════════════════════════════════════ -->
<div id="q8" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(7)">◀ Previous</button>
  <span class="q-counter">Question 8 of 13</span>
  <button class="q-nav-btn" onclick="showQ(9)">Next ▶</button>
</div>
<div class="q-header">Question 8 <span class="badge badge-medium">🟡 Medium</span></div>
<div class="q-body">

<p class="q-text">Subtract:</p>
<ol class="q-options">
  <li class="arithmatex">\( 3.\dot{4} - 2.1\dot{3} \)</li>
  <li class="arithmatex">\( 8.49 - 5.35\dot{6} \)</li>
</ol>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Convert each recurring decimal to a fraction, perform the subtraction as a fraction calculation, then convert the answer back to a decimal. This avoids any confusion with misaligned repeating blocks.
</div>
</div>

<div class="part-label">(a) \( 3.\dot{4} - 2.1\dot{3} \)</div>

<div class="step-box">
<div class="step-label">Step 1 — Convert \( 3.\dot{4} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 3.\dot{4} = 3.4444\ldots \)<br>
0 non-recurring digits, 1 recurring digit → multiply by 10:
\[ 10x = 34.\dot{4} \]
\[ 10x - x = 34.\dot{4} - 3.\dot{4} \implies 9x = 31 \implies x = \frac{31}{9} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Convert \( 2.1\dot{3} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 2.1\dot{3} = 2.1333\ldots \)<br>
1 non-recurring digit (1), 1 recurring digit (3) → multiply by 10 and 100:
\[ 10x = 21.333\ldots \qquad 100x = 213.333\ldots \]
\[ 90x = 192 \implies x = \frac{192}{90} = \frac{32}{15} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Subtract the fractions</div>
<div class="step-body arithmatex">
\[ \frac{31}{9} - \frac{32}{15} \]
LCM(9, 15) = 45:
\[ \frac{31 \times 5}{45} - \frac{32 \times 3}{45} = \frac{155 - 96}{45} = \frac{59}{45} \]
Converting: \( 59 \div 45 = 1 \) rem 14; \( 140 \div 45 = 3 \) rem 5; \( 50 \div 45 = 1 \) rem 5 (repeats).
\[ \frac{59}{45} = 1.3\dot{1} \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) \( 8.49 - 5.35\dot{6} \)</div>

<div class="step-box">
<div class="step-label">Step 4 — Convert \( 5.35\dot{6} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 5.35\dot{6} = 5.35666\ldots \)<br>
2 non-recurring digits (35), 1 recurring digit (6) → multiply by 100 and 1000:
\[ 100x = 535.666\ldots \qquad 1000x = 5356.666\ldots \]
\[ 900x = 4821 \implies x = \frac{4821}{900} = \frac{1607}{300} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 5 — Subtract the fractions</div>
<div class="step-body arithmatex">
Write \( 8.49 = \dfrac{849}{100} \). The LCM of 100 and 300 is 300:
\[ \frac{849}{100} - \frac{1607}{300} = \frac{2547}{300} - \frac{1607}{300} = \frac{940}{300} = \frac{47}{15} \]
Converting: \( 47 \div 15 = 3 \) rem 2; \( 20 \div 15 = 1 \) rem 5; \( 50 \div 15 = 3 \) rem 5 (repeats).
\[ \frac{47}{15} = 3.1\dot{3} \]
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) \( 3.\dot{4} - 2.1\dot{3} = \dfrac{59}{45} = 1.3\dot{1} \)<br>
(b) \( 8.49 - 5.35\dot{6} = \dfrac{47}{15} = 3.1\dot{3} \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(7)">◀ Previous</button>
  <span class="q-counter">Question 8 of 13</span>
  <button class="q-nav-btn" onclick="showQ(9)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 9  —  Multiply recurring decimals  (Hard)
════════════════════════════════════════════════════════════ -->
<div id="q9" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(8)">◀ Previous</button>
  <span class="q-counter">Question 9 of 13</span>
  <button class="q-nav-btn" onclick="showQ(10)">Next ▶</button>
</div>
<div class="q-header">Question 9 <span class="badge badge-hard">🔴 Hard</span></div>
<div class="q-body">

<p class="q-text">Multiply:</p>
<ol class="q-options">
  <li class="arithmatex">\( 0.\dot{3} \times 0.\dot{6} \)</li>
  <li class="arithmatex">\( 2.4 \times 0.\dot{8}\dot{1} \)</li>
</ol>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Convert every recurring decimal to a fraction. Multiply the fractions using \( \dfrac{a}{b} \times \dfrac{c}{d} = \dfrac{ac}{bd} \). Simplify the result and convert back to a decimal.
</div>
</div>

<div class="part-label">(a) \( 0.\dot{3} \times 0.\dot{6} \)</div>

<div class="step-box">
<div class="step-label">Step 1 — Convert both decimals to fractions</div>
<div class="step-body arithmatex">
\[ 0.\dot{3} = \frac{3}{9} = \frac{1}{3} \qquad 0.\dot{6} = \frac{6}{9} = \frac{2}{3} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Multiply the fractions</div>
<div class="step-body arithmatex">
\[ \frac{1}{3} \times \frac{2}{3} = \frac{2}{9} = 0.\dot{2} \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) \( 2.4 \times 0.\dot{8}\dot{1} \)</div>

<div class="step-box">
<div class="step-label">Step 3 — Convert both numbers to fractions</div>
<div class="step-body arithmatex">
\[ 2.4 = \frac{24}{10} = \frac{12}{5} \]
For \( 0.\dot{8}\dot{1} = 0.818181\ldots \), the repeating block "81" has 2 digits, so multiply by 99:
\[ 99x = 81 \implies x = \frac{81}{99} = \frac{9}{11} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Multiply the fractions</div>
<div class="step-body arithmatex">
\[ \frac{12}{5} \times \frac{9}{11} = \frac{108}{55} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 5 — Convert \( \dfrac{108}{55} \) back to a decimal</div>
<div class="step-body arithmatex">
\( 108 \div 55 = 1 \) rem 53<br>
\( 530 \div 55 = 9 \) rem 35<br>
\( 350 \div 55 = 6 \) rem 20<br>
\( 200 \div 55 = 3 \) rem 35 → remainder 35 repeats, so block "63" recurs.
\[ \frac{108}{55} = 1.9\dot{6}\dot{3} \]
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) \( 0.\dot{3} \times 0.\dot{6} = \dfrac{2}{9} = 0.\dot{2} \)<br>
(b) \( 2.4 \times 0.\dot{8}\dot{1} = \dfrac{108}{55} = 1.9\dot{6}\dot{3} \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(8)">◀ Previous</button>
  <span class="q-counter">Question 9 of 13</span>
  <button class="q-nav-btn" onclick="showQ(10)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 10  —  Divide recurring decimals  (Hard)
════════════════════════════════════════════════════════════ -->
<div id="q10" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(9)">◀ Previous</button>
  <span class="q-counter">Question 10 of 13</span>
  <button class="q-nav-btn" onclick="showQ(11)">Next ▶</button>
</div>
<div class="q-header">Question 10 <span class="badge badge-hard">🔴 Hard</span></div>
<div class="q-body">

<p class="q-text">Divide:</p>
<ol class="q-options">
  <li class="arithmatex">\( 0.\dot{3} \div 0.\dot{6} \)</li>
  <li class="arithmatex">\( 2.\dot{3}\dot{7} \div 0.\dot{4}\dot{5} \)</li>
</ol>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Convert every recurring decimal to a fraction. Use the rule \( \dfrac{a}{b} \div \dfrac{c}{d} = \dfrac{a}{b} \times \dfrac{d}{c} \) (multiply by the reciprocal). Simplify fully, then convert back to a decimal.
</div>
</div>

<div class="part-label">(a) \( 0.\dot{3} \div 0.\dot{6} \)</div>

<div class="step-box">
<div class="step-label">Step 1 — Convert to fractions and divide</div>
<div class="step-body arithmatex">
\[ 0.\dot{3} = \frac{1}{3}, \qquad 0.\dot{6} = \frac{2}{3} \]
\[ \frac{1}{3} \div \frac{2}{3} = \frac{1}{3} \times \frac{3}{2} = \frac{1}{2} = 0.5 \]
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) \( 2.\dot{3}\dot{7} \div 0.\dot{4}\dot{5} \)</div>

<div class="step-box">
<div class="step-label">Step 2 — Convert \( 2.\dot{3}\dot{7} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 2.\dot{3}\dot{7} = 2.373737\ldots \)<br>
0 non-recurring digits, 2 recurring digits → multiply by 100:
\[ 100x = 237.\dot{3}\dot{7} \]
\[ 100x - x = 235 \implies 99x = 235 \implies x = \frac{235}{99} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Convert \( 0.\dot{4}\dot{5} \) to a fraction</div>
<div class="step-body arithmatex">
Let \( x = 0.\dot{4}\dot{5} = 0.454545\ldots \)<br>
\[ 99x = 45 \implies x = \frac{45}{99} = \frac{5}{11} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Divide the fractions</div>
<div class="step-body arithmatex">
\[ \frac{235}{99} \div \frac{5}{11} = \frac{235}{99} \times \frac{11}{5} = \frac{235 \times 11}{99 \times 5} = \frac{2585}{495} \]
Simplify. The GCD of 2585 and 495:
\[ 2585 = 5 \times 11 \times 47, \qquad 495 = 5 \times 9 \times 11 \]
GCD = \( 5 \times 11 = 55 \):
\[ \frac{2585}{495} = \frac{47}{9} \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 5 — Convert \( \dfrac{47}{9} \) to a decimal</div>
<div class="step-body arithmatex">
\( 47 \div 9 = 5 \) rem 2; \( 20 \div 9 = 2 \) rem 2 (repeats immediately).
\[ \frac{47}{9} = 5.\dot{2} \]
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) \( 0.\dot{3} \div 0.\dot{6} = \dfrac{1}{2} = 0.5 \)<br>
(b) \( 2.\dot{3}\dot{7} \div 0.\dot{4}\dot{5} = \dfrac{47}{9} = 5.\dot{2} \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(9)">◀ Previous</button>
  <span class="q-counter">Question 10 of 13</span>
  <button class="q-nav-btn" onclick="showQ(11)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 11  —  Prove √5 and √10 are irrational  (Hard)
════════════════════════════════════════════════════════════ -->
<div id="q11" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(10)">◀ Previous</button>
  <span class="q-counter">Question 11 of 13</span>
  <button class="q-nav-btn" onclick="showQ(12)">Next ▶</button>
</div>
<div class="q-header">Question 11 <span class="badge badge-hard">🔴 Hard</span></div>
<div class="q-body">

<p class="q-text">Prove that the following numbers are irrational:</p>
<ol class="q-options">
  <li class="arithmatex">\( \sqrt{5} \)</li>
  <li class="arithmatex">\( \sqrt{10} \)</li>
</ol>

<div class="theory-box">
<div class="theory-header">Theory — Proof by Contradiction</div>
<div class="theory-body arithmatex">
A <strong>proof by contradiction</strong> works like this:<br>
1. Assume the opposite of what you want to prove is true.<br>
2. Follow the logical consequences of that assumption.<br>
3. Arrive at something that is impossible or contradicts your assumption.<br>
4. Conclude that your assumption must have been false — so the original statement is true.<br><br>
We also use the fact: <em>if a prime \( p \) divides \( n^2 \), then \( p \) divides \( n \)</em>. This follows because if \( n = p_1^{a_1} p_2^{a_2}\cdots \), then \( n^2 = p_1^{2a_1}p_2^{2a_2}\cdots \) — a prime that appears in \( n^2 \) must have already appeared in \( n \).
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Assume \( \sqrt{5} \) (and then \( \sqrt{10} \)) is rational, i.e. it equals \( \dfrac{p}{q} \) in lowest terms (where \( p \) and \( q \) share no common factor). Square both sides, then show that both \( p \) and \( q \) must share a common factor — contradicting the assumption.
</div>
</div>

<div class="part-label">(a) Prove \( \sqrt{5} \) is irrational</div>

<div class="step-box">
<div class="step-label">Step 1 — Assume the opposite</div>
<div class="step-body arithmatex">
Suppose, for contradiction, that \( \sqrt{5} \) is rational.<br>
Then we can write \( \sqrt{5} = \dfrac{p}{q} \) where \( p \) and \( q \) are integers with no common factor (the fraction is in its lowest terms) and \( q \neq 0 \).
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Square both sides</div>
<div class="step-body arithmatex">
\[ \left(\sqrt{5}\right)^2 = \left(\frac{p}{q}\right)^2 \implies 5 = \frac{p^2}{q^2} \implies p^2 = 5q^2 \]
This tells us that 5 divides \( p^2 \).
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Show 5 divides p</div>
<div class="step-body arithmatex">
Since 5 is prime and \( 5 \mid p^2 \), we conclude \( 5 \mid p \).<br>
So write \( p = 5k \) for some integer \( k \).
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Substitute and find the contradiction</div>
<div class="step-body arithmatex">
Substitute \( p = 5k \) into \( p^2 = 5q^2 \):
\[ (5k)^2 = 5q^2 \implies 25k^2 = 5q^2 \implies q^2 = 5k^2 \]
So 5 divides \( q^2 \), and since 5 is prime, \( 5 \mid q \).<br><br>
But now both \( p \) and \( q \) are divisible by 5. This contradicts our assumption that \( \dfrac{p}{q} \) is in its lowest terms.<br><br>
Therefore \( \sqrt{5} \) is <strong>irrational</strong>. \( \blacksquare \)
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) Prove \( \sqrt{10} \) is irrational</div>

<div class="step-box">
<div class="step-label">Step 5 — Assume the opposite</div>
<div class="step-body arithmatex">
Suppose \( \sqrt{10} = \dfrac{p}{q} \) in lowest terms (\( p, q \) share no common factor, \( q \neq 0 \)).
</div>
</div>

<div class="step-box">
<div class="step-label">Step 6 — Square both sides</div>
<div class="step-body arithmatex">
\[ 10 = \frac{p^2}{q^2} \implies p^2 = 10q^2 \]
Since \( 10q^2 \) is even, \( p^2 \) is even, which means \( p \) is even (an odd number squared is always odd).<br>
Write \( p = 2k \).
</div>
</div>

<div class="step-box">
<div class="step-label">Step 7 — Find the contradiction</div>
<div class="step-body arithmatex">
Substitute \( p = 2k \):
\[ (2k)^2 = 10q^2 \implies 4k^2 = 10q^2 \implies 2k^2 = 5q^2 \]
The left side is even. For \( 5q^2 \) to be even, since 5 is odd, \( q^2 \) must be even, so \( q \) is even.<br><br>
Both \( p \) and \( q \) are divisible by 2, contradicting lowest terms.<br><br>
Therefore \( \sqrt{10} \) is <strong>irrational</strong>. \( \blacksquare \)
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
Both \( \sqrt{5} \) and \( \sqrt{10} \) are irrational. In each case, assuming rationality leads to a contradiction: both \( p \) and \( q \) end up sharing a common factor, which is impossible if the fraction is in lowest terms.
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(10)">◀ Previous</button>
  <span class="q-counter">Question 11 of 13</span>
  <button class="q-nav-btn" onclick="showQ(12)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 12  —  Prove divisibility by 8  (Hard)
════════════════════════════════════════════════════════════ -->
<div id="q12" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(11)">◀ Previous</button>
  <span class="q-counter">Question 12 of 13</span>
  <div class="q-nav-spacer"></div>
</div>
<div class="q-header">Question 12 <span class="badge badge-hard">🔴 Hard</span></div>
<div class="q-body">

<p class="q-text">Prove that the product of any two consecutive even integers is divisible by 8.</p>

<div class="theory-box">
<div class="theory-header">Theory — Consecutive Even Integers</div>
<div class="theory-body arithmatex">
An <strong>even integer</strong> can always be written as \( 2n \) for some integer \( n \).<br><br>
The <strong>next</strong> even integer after \( 2n \) is \( 2n + 2 = 2(n+1) \).<br><br>
Key fact: among any two consecutive integers \( n \) and \( n+1 \), exactly one is even and one is odd. Therefore their product \( n(n+1) \) is always even — it equals \( 2m \) for some integer \( m \).
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
Write the two consecutive even integers in general form as \( 2n \) and \( 2(n+1) \). Multiply them, then factor the result to show it is a multiple of 8.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 1 — Write the two consecutive even integers in general form</div>
<div class="step-body arithmatex">
Let the two consecutive even integers be \( 2n \) and \( 2(n+1) \), where \( n \) is any integer.
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Write out their product</div>
<div class="step-body arithmatex">
\[ \text{Product} = 2n \times 2(n+1) = 4n(n+1) \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 3 — Show that \( n(n+1) \) is always even</div>
<div class="step-body arithmatex">
\( n \) and \( n+1 \) are consecutive integers. One of them must be even (integers alternate between odd and even). The product of any even number with anything is even, so:
\[ n(n+1) = 2m \quad \text{for some integer } m \]
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Conclude the product is divisible by 8</div>
<div class="step-body arithmatex">
Substitute \( n(n+1) = 2m \) into the product:
\[ \text{Product} = 4 \times n(n+1) = 4 \times 2m = 8m \]
Since the product equals \( 8m \) for some integer \( m \), it is divisible by 8. \( \blacksquare \)
</div>
</div>

<div class="note-box">
<div class="note-header">Note — Quick Check</div>
<div class="note-body arithmatex">
Try it with examples: \( 2 \times 4 = 8 \) ✓, \( 4 \times 6 = 24 = 8 \times 3 \) ✓, \( 6 \times 8 = 48 = 8 \times 6 \) ✓. The general proof covers all cases at once.
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
Any two consecutive even integers can be written as \( 2n \) and \( 2(n+1) \). Their product is:
\[ 2n \cdot 2(n+1) = 4n(n+1) \]
Since \( n \) and \( n+1 \) are consecutive, one is even, so \( n(n+1) = 2m \) for some integer \( m \). Therefore the product equals \( 8m \), which is divisible by 8. \( \blacksquare \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(11)">◀ Previous</button>
  <span class="q-counter">Question 12 of 13</span>
  <button class="q-nav-btn" onclick="showQ(13)">Next ▶</button>
</div>
</div></div>


<!-- ══════════════════════════════════════════════════════════
     QUESTION 13  —  Find rational & irrational numbers  (Medium)
════════════════════════════════════════════════════════════ -->
<div id="q13" class="question-block" style="display:none">
<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(12)">◀ Previous</button>
  <span class="q-counter">Question 13 of 13</span>
  <div class="q-nav-spacer"></div>
</div>
<div class="q-header">Question 13 <span class="badge badge-medium">🟡 Medium</span></div>
<div class="q-body">

<ol class="q-options">
  <li class="arithmatex">Find two irrational numbers between \( 0.12 \) and \( 0.31 \).</li>
  <li class="arithmatex">Find a rational number and an irrational number between \( \dfrac{1}{\sqrt{2}} \) and \( \sqrt{2} \).</li>
</ol>

<div class="theory-box">
<div class="theory-header">Theory — Density of Rational and Irrational Numbers</div>
<div class="theory-body arithmatex">
Between any two distinct real numbers, no matter how close, there are infinitely many rational numbers <em>and</em> infinitely many irrational numbers. This property is called <strong>density</strong>.<br><br>
To <em>find</em> an irrational in a range, a practical method is to take a known irrational (like \( \sqrt{2} \) or \( \sqrt{3} \)) and scale it by a rational number to land inside the target range.
</div>
</div>

<div class="strategy-box">
<div class="strategy-header">Strategy</div>
<div class="strategy-body arithmatex">
For part (a): divide a known irrational (\( \sqrt{2} \) or \( \sqrt{3} \)) by a suitable integer so the result falls between 0.12 and 0.31. A rational times an irrational remains irrational.<br><br>
For part (b): estimate \( \dfrac{1}{\sqrt{2}} \approx 0.707 \) and \( \sqrt{2} \approx 1.414 \). Pick one obvious rational and one irrational in that interval, then verify algebraically.
</div>
</div>

<div class="part-label">(a) Two irrational numbers between 0.12 and 0.31</div>

<div class="step-box">
<div class="step-label">Step 1 — Scale known irrationals into the target range</div>
<div class="step-body arithmatex">
\( \sqrt{2} \approx 1.41421\ldots \) and \( \sqrt{3} \approx 1.73205\ldots \)<br>
Dividing each by 10:
\[ \frac{\sqrt{2}}{10} \approx 0.14142\ldots \qquad \frac{\sqrt{3}}{10} \approx 0.17320\ldots \]
Both lie strictly between 0.12 and 0.31. ✓
</div>
</div>

<div class="step-box">
<div class="step-label">Step 2 — Confirm both are irrational</div>
<div class="step-body arithmatex">
\( \sqrt{2} \) is irrational (its decimal expansion never terminates or repeats). Dividing by the non-zero rational 10 keeps it irrational — a rational divided into an irrational never produces a rational result.<br><br>
The same reasoning applies to \( \dfrac{\sqrt{3}}{10} \).
</div>
</div>

<hr class="part-hr">
<div class="part-label">(b) A rational and an irrational between \( \dfrac{1}{\sqrt{2}} \) and \( \sqrt{2} \)</div>

<div class="step-box">
<div class="step-label">Step 3 — Estimate the endpoints</div>
<div class="step-body arithmatex">
\[ \frac{1}{\sqrt{2}} = \frac{\sqrt{2}}{2} \approx \frac{1.41421}{2} \approx 0.7071 \]
\[ \sqrt{2} \approx 1.4142 \]
We need one rational and one irrational strictly between \( 0.7071 \) and \( 1.4142 \).
</div>
</div>

<div class="step-box">
<div class="step-label">Step 4 — Choose a rational number in the range</div>
<div class="step-body arithmatex">
The whole number 1 satisfies \( 0.707 < 1 < 1.414 \).<br><br>
<strong>Rational number: \( 1 \)</strong>
</div>
</div>

<div class="step-box">
<div class="step-label">Step 5 — Choose and verify an irrational number in the range</div>
<div class="step-body arithmatex">
Try \( \dfrac{\sqrt{3}}{2} \approx \dfrac{1.73205}{2} \approx 0.8660 \).<br><br>
<strong>Left inequality</strong> — show \( \dfrac{1}{\sqrt{2}} < \dfrac{\sqrt{3}}{2} \):
\[ \frac{1}{\sqrt{2}} < \frac{\sqrt{3}}{2} \iff \sqrt{2} < \sqrt{3} \iff 2 < 3 \;\checkmark \]
<strong>Right inequality</strong> — show \( \dfrac{\sqrt{3}}{2} < \sqrt{2} \):
\[ \frac{\sqrt{3}}{2} < \sqrt{2} \iff \sqrt{3} < 2\sqrt{2} \iff 3 < 8 \;\checkmark \]
Since \( \dfrac{\sqrt{3}}{2} \) is irrational ÷ rational, it is irrational.<br><br>
<strong>Irrational number: \( \dfrac{\sqrt{3}}{2} \)</strong>
</div>
</div>

<div class="final-box">
<div class="final-header">Final Answer</div>
<div class="final-body arithmatex">
(a) Two irrationals between 0.12 and 0.31: \(\;\dfrac{\sqrt{2}}{10} \approx 0.1414\ldots\) and \(\dfrac{\sqrt{3}}{10} \approx 0.1732\ldots\)<br><br>
(b) Between \( \dfrac{1}{\sqrt{2}} \) and \( \sqrt{2} \):<br>
&nbsp;&nbsp;&nbsp;Rational: \( 1 \)<br>
&nbsp;&nbsp;&nbsp;Irrational: \( \dfrac{\sqrt{3}}{2} \approx 0.8660\ldots \)
</div>
</div>

<div class="q-nav">
  <button class="q-nav-btn" onclick="showQ(12)">◀ Previous</button>
  <span class="q-counter">Question 13 of 13</span>
  <div class="q-nav-spacer"></div>
</div>
</div></div>

</div><!-- end ex-page -->

<script>
function showQ(n) {
  var blocks = document.querySelectorAll('.question-block');
  for (var i = 0; i < blocks.length; i++) {
    blocks[i].style.display = 'none';
  }
  var target = document.getElementById('q' + n);
  if (target) {
    target.style.display = 'block';
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
}
</script>
