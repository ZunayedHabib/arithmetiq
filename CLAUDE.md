# ArithmetiQ — Project Rules

## What This Project Is
A free mathematics tutoring website called ArithmetiQ.
Built with MkDocs Material + MathJax. Hosted on GitHub Pages.
Audience: students with little to no prior knowledge of the topic.

## Teaching Philosophy — Non-Negotiable, Apply Everywhere
- Assume zero prior knowledge — introduce every concept from scratch
- Break everything down to its simplest form
- Never skip steps — show every single line of working
- Every formula must be stated and explained before it is used
- Be thorough but never overwhelming — do not over-explain
- Tone is friendly, clear and encouraging — never cold or textbook-dry
- Use THEORY boxes to introduce a concept before using it
- Use FORMULA boxes to display key formulas cleanly
- Use NOTE boxes for tricky steps or common mistakes only
- Do not use these boxes excessively — only where genuinely needed

## Multi-Part Questions
- All parts (a), (b), (c) solved within one question block
- Parts separated by a horizontal rule <hr>
- Each part clearly labelled: (a), (b), (c)
- Final answer covers all parts together at the end

## Formatting — Identical Across The Whole Site, No Exceptions
- Difficulty badge on every question: 🟢 Easy / 🟡 Medium / 🔴 Hard
- STRATEGY box before the solution of every question
- Numbered steps — each step says what it does, not just shows algebra
- NOTE boxes at tricky moments only
- FINAL ANSWER box at the end of every question
- Inline math: \( \) — Display math: $$ $$
- This structure never changes anywhere on the site

## Color Schemes
- ArithmetiQ global/homepage: #e67e22 → #f39c12 (orange)
- NCTB General Math 9-10:     #f39c12 → #e67e22 (amber/orange)
- NCTB Higher Math 9-10:      #e74c3c → #c0392b (red/rose)
- Edexcel P1:                  #667eea → #764ba2 (purple)
- Edexcel P2:                  #11998e → #38ef7d (teal/green)

## Diagrams
- All diagrams are inline SVG — never external image files
- Recreate any diagram from question images as accurate inline SVG
- Axes must be labelled, points marked, measurements must match exactly

## File Structure
docs/
├── index.md
├── nctb-general-math-9-10/chapter-X-slug/exercise-X-Y.md
├── nctb-higher-math-9-10/chapter-X-slug/exercise-X-Y.md
├── edexcel-p1/chapter-X/section-Xa.md
└── edexcel-p2/chapter-X/section-Xa.md

## After Every New File
Run automatically: git add . && git commit -m "add [filename]" && git push
Never ask — just run it every time.
