# Leadership OS — Logo Build Spec (mark "B")

*Everything needed to produce the final logo accurately. The design is locked; only the rendering needs a machine that has Cormorant Garamond installed (this build environment does not, and its font CDNs are blocked — so this spec exists to be executed in Figma, Illustrator, a browser, or any tool with the font).*

---

## The wordmark

**"Leadership"**
- Font: **Cormorant Garamond, Light (weight 300), roman (upright)**
- Color: **Ink `#1A1612`**
- This matches the website hero exactly (the hero is Cormorant Garamond weight 300).

**"OS"**
- Font: **Cormorant Garamond, Bold Italic (weight 700, italic)** — deliberately much heavier than "Leadership," for contrast
- Color: **Gold `#B8671E`**
- Set tight to "Leadership" with a single normal word-space between.

Rationale: the black-roman / gold-heavy-italic split mirrors the hero's own move ("ever *gave you*." — roman, then a gold italic emphasis). The logo inherits the brand's established type personality instead of inventing one.

---

## The mark (triangulation glyph)

Distilled from the methodology page's triangulation diagram. Three points around an open center.

- **Three points**, arranged as a triangle (two top, one bottom-center):
  - Top-left point — **Assessment** — color `#6B5BD1` (the violet from the site diagram)
  - Top-right point — **Reflection** — color `#2E9E7E` (the green from the site diagram)
  - Bottom-center point — **Corpus** — color `#B8671E` (gold)
  - Point radius ≈ 5px at a 64px cap height; solid filled circles.
- **Faint convergence lines** from each point toward the center: stroke `#CFC7BA`, ~1.4px. (Optional — omit for the minimal version.)
- **Open center:** a **dashed circle**, radius ≈ 12px, stroke `#B8671E` (gold) ~1.2px, `stroke-dasharray: 2.5 3`. The center is NOT filled and NOT closed — the dashes are the "hypothesis, not verdict" cue, taken straight from the diagram's dashed "triangulation" ring.

**Monochrome fallback (required for single-color use):** the two top points become ink `#1A1612`, the bottom point and the dashed center stay gold `#B8671E`. Convergence lines `#CFC7BA`.

---

## Lockups to produce

1. **Horizontal (primary):** mark at left, vertically centered to the wordmark, ~24px gap. Wordmark baseline aligned to the mark's vertical center.
2. **Stacked:** mark centered above the wordmark (mark, then ~18px gap, then wordmark centered). For square/social/avatar use.
3. **Wordmark only:** for tight horizontal spaces (site header).
4. **Mark only:** for favicon / app icon / avatar — the three points + dashed center, no text.

## Color variants for each lockup

- **Full color** (three source-colors) — primary
- **Monochrome ink** (ink + single gold accent) — for single-color contexts
- **Reversed** (on `#1A1612` ink background): wordmark in cream `#FAF8F4`, "OS" stays gold `#C9843A` (the lighter gold reads better on dark), mark points lighten one step (`#8B7EE0` violet, `#4CBF9E` green, `#C9843A` gold).

## Favicon
- Mark only, in a rounded-square ink tile `#1A1612`, radius ~8px on a 48px tile.
- Points: `#8B7EE0` / `#4CBF9E` / `#C9843A`; dashed center in `#C9843A`.
- Verified legible down to ~32px (three colored points survive the shrink; lines/labels do not — so drop convergence lines in the favicon).

---

## Two-minute build recipe (any environment with the font)

**In Figma / Illustrator:**
1. Type "Leadership " — Cormorant Garamond Light 300, `#1A1612`.
2. Type "OS" — Cormorant Garamond Bold Italic 700, `#B8671E`. Keep as one text line.
3. Draw the mark per the spec above (3 circles, dashed center circle, optional convergence lines).
4. Group, align mark to wordmark, export SVG **with text outlined** ("Outline stroke" / "Create outlines") so the file carries no font dependency.

**In code (browser, where the font loads):** an HTML/SVG file referencing the Google Fonts Cormorant import will render correctly in a real browser (unlike the sandboxed preview that failed here). Then convert text→paths once before shipping.

**Critical:** always **outline the type to vector paths** in the final asset. A logo that references a webfont can silently fall back to the wrong font (this is exactly what kept happening in preview). Outlined paths are pixel-identical everywhere, forever.

---

## What's locked vs. open
- **Locked:** the concept (triangulation mark + wordmark), the type (Cormorant Light roman "Leadership" + Bold Italic gold "OS"), the three source-colors, the dashed open center.
- **Still your call:** whether the convergence lines stay (fuller) or go (minimal/points-only); exact point sizes and gap; whether the mark sits left (horizontal) or above (stacked) as the *primary*.
