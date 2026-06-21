# Leadership OS — Logo Production Brief (hand to any AI or designer)

You are producing the final Leadership OS logo. The design is **fully decided** — your job is faithful execution in the correct typeface, not redesign. Do not propose alternative concepts. Render exactly what's specified, in true Cormorant Garamond, and output outlined-vector SVG files.

---

## THE DESIGN (decided — do not change)

A horizontal lockup: a small **triangulation mark** at left + the **wordmark** "Leadership OS" at right.

### Wordmark
- **"Leadership"** — Cormorant Garamond, **Light (300)**, **roman/upright**, color **ink `#1A1612`**.
- one normal word-space, then
- **"OS"** — Cormorant Garamond, **Bold Italic (700, italic)**, color **gold `#B8671E`**. Deliberately much heavier and italic for emphasis.
- This mirrors the website hero, which is Cormorant Garamond weight 300 with a gold italic emphasis ("ever *gave you*."). Match that hero exactly — same font, same light weight on the roman word.

### Mark (the triangulation glyph)
Three filled points arranged as a triangle around an open dashed center. Distilled from the product's methodology diagram (three evidence sources converging on a provisional read).
- Top-left point — color **violet `#6B5BD1`** (Assessment)
- Top-right point — color **green `#2E9E7E`** (Reflection)
- Bottom-center point — color **gold `#B8671E`** (Corpus)
- Point radius ≈ 5px when point spacing is ~26px (scale proportionally).
- **Open center:** a **dashed** circle (radius ≈ 12px, stroke gold `#B8671E` ~1.3px, dash pattern `2.5 3`), **not filled, not closed** — the dashes encode "hypothesis, not verdict." This is essential and must stay dashed/open.
- Optional thin convergence lines from each point to center, stroke `#CFC7BA` ~1.4px. Include for large lockups; omit for small/favicon.

---

## VARIANTS TO PRODUCE (each as its own SVG, type outlined)

1. **Horizontal — full color** (primary): mark left, wordmark right, mark vertically centered to the wordmark, gap ~24px.
2. **Horizontal — monochrome**: same, but the two top points become ink `#1A1612`; bottom point + dashed center stay gold; lines `#CFC7BA`. (For single-color/emboss/fax contexts.)
3. **Reversed on ink** (`#1A1612` background): "Leadership" in cream `#FAF8F4`; "OS" in lighter gold `#C9843A`; mark points lighten to violet `#8B7EE0`, green `#4CBF9E`, gold `#C9843A`; dashed center `#C9843A`.
4. **Stacked**: mark centered above wordmark (for square/social).
5. **Wordmark only** (no mark) — for tight headers.
6. **Mark only** — for favicon/app-icon/avatar.
7. **Favicon tile**: mark only (NO convergence lines) on a rounded-square ink tile `#1A1612` (radius ~14px @ 88px). Use the reversed/lighter point colors. NOTE: below ~24px the dashed ring muddies — for a 16px favicon, simplify (solid faint center dot instead of dashed ring, or three points only).

---

## HARD REQUIREMENTS
- **Typeface must be true Cormorant Garamond** (Light 300 roman + Bold Italic 700). Do NOT substitute Lora, EB Garamond, Georgia, or any look-alike. If you cannot load Cormorant, say so rather than substituting silently.
- **Outline all type to vector paths** in the final SVGs (no font dependency — prevents fallback errors).
- Palette is exact: ink `#1A1612`, cream `#FAF8F4`, gold `#B8671E`, light-gold `#C9843A`, violet `#6B5BD1`, green `#2E9E7E`.
- The dashed open center is non-negotiable (it's the philosophy: provisional, not final).
- No swooshes, no closed rings as the center, no gradients, no glow, no extra ornament.

## ACCEPTANCE CHECK
- Does "Leadership" match the hero (Cormorant, light, roman, ink)? 
- Is "OS" clearly heavier, italic, gold?
- Is the center dashed and open (not a solid/closed circle)?
- Do the three point-colors match the methodology diagram?
- Is the type outlined (open the SVG with the font uninstalled — does it still look right)?

---

## CONTEXT (why, so you don't "improve" it away)
The three colors and the dashed-open center come straight from the live product's triangulation diagram — they mean "three evidence sources, provisional synthesis." The light-roman / heavy-gold-italic wordmark split inherits the website hero's own type personality. Every choice is deliberate and tied to the brand's philosophy of hypotheses over verdicts. Execute faithfully.
