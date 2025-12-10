# S2-Insignia-Glyphs
S2 Glyph Library — README.txt

This project contains an SVG-based library of the S2 10.3–style hull number glyphs:
digits 0–9, the letter S, the letter A, the letter C, and the decimal point.

These shapes were manually traced and measured from original S2 graphics so they can be reused consistently in digit strings such as “S2 10.3”, sail numbers, graphics documents, or any custom layouts.

1. What This File Is
S2_glyph_library.svg contains:
- All glyphs defined as SVG <symbol> elements
- A small visual layout showing a 2-row grid of glyphs
- Each glyph retains its original coordinate space so numbers stay aligned when assembled

This file is meant as a source of vector definitions, not a standalone graphic.

2. What You Can Do With It
You can:
- Copy individual glyphs (the <path> elements) into your own SVGs
- Reuse them in web designs or GUI applications that support <symbol> and <use>
- Produce consistent S2-style hull numbers at any scale
- Use them in external tools that support SVG symbols (most browsers, many renderers)

3. What This File Will Not Do
- Microsoft Visio cannot open this file directly. It does not support <symbol>/<use> in imported SVG.
- This file does not claim compatibility with Illustrator or Inkscape. Behavior may vary.

4. Using the Glyphs
To assemble text (e.g., “10.3”):
1. Copy the <symbol> definitions from the library into your project.
2. Use <use href="#s2-1">, <use href="#s2-0">, etc.
3. Position glyphs by adjusting x and y.
4. Scale the container, not the glyphs, to preserve stroke fidelity.

Glyph alignment:
- All digits share a common baseline.
- “S” aligns with the digits.
- Decimal point is baseline-aligned via internal translation.

5. Known Limitations
- Kerning is manual.
- Decimal positioning is handled inside the symbol.
- Designed for SVG-native environments, not WYSIWYG vector editors.

6. File Organization
Symbols included:
s2-0 s2-1 s2-2 s2-3 s2-4
s2-5 s2-6 s2-7 s2-8 s2-9
s2-S s2-A s2-C s2-decimal

Preview layout:
Row 1: digits 0–9
Row 2: S, A, C, decimal

Preview alignment may vary across viewers.

7. Future Options
Optional future exports:
- Flattened Visio-compatible SVG
- Individual per-glyph SVGs
- Visio stencil
- OpenType-SVG font

End of README.
