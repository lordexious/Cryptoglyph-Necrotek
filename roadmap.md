# Cryptoglyph-Necrotek Roadmap

This document outlines planned updates, structural improvements, and known issues for Cryptoglyph-Necrotek.

Current Version: **v1.0.0**

---

## Known Issues

### K1 — Connector Geometry Refinement

The bottom-arc connector is functionally correct but requires additional refinement for optimal visual balance.

**Observed behavior:**
- Slight visual heaviness at higher stroke widths  
- Minor proportional imbalance between arc and oval  
- Connector spacing sensitivity in dense layouts  

**Planned improvements:**
- Micro-offset tuning based on stroke width  
- Normalize arc-to-oval proportions  
- Refine vertical spacing for consistent rhythm  
- Evaluate optional alternate connector style  

---

## Planned Updates

### v1.1.0 — Numbers & Punctuation Expansion

Primary goal: achieve full sentence and numeric support.

---

### Expanded Punctuation Set

Add glyph support for:

- `!` Exclamation  
- `?` Question mark  
- `:` Colon  
- `;` Semicolon  
- `'` Apostrophe  
- `"` Quotation marks  
- `-` Dash / Hyphen  
- `(` `)` Parentheses  

**Acceptance criteria:**
- All punctuation renders correctly in Canvas  
- SVG export matches Canvas output  
- No connector behavior applied to punctuation  
- Consistent spacing rules maintained  

---

### Numeric Glyph System (0–9)

Add glyph definitions for digits:

- `0 1 2 3 4 5 6 7 8 9`

**Design requirements:**
- Inline placement (not stacked)  
- No connector linking between digits  
- Consistent vertical rhythm with letter glyphs  
- Compatible with column wrap mode  

**Acceptance criteria:**
- Numbers render anywhere in text  
- SVG export parity maintained  
- No layout corruption  

---

### Symbol Layer Expansion

Initial symbol candidates:

- `@ # $ % & * + =`
- `/ \ _`
- `[ ] { } < >`

**Acceptance criteria:**
- Unsupported characters degrade gracefully  
- Optional placeholder glyph support  

---

## Structural Improvements

### Data-Driven Glyph Architecture

Refactor glyph definitions into a structured system to:

- Reduce duplicated geometry logic  
- Simplify adding punctuation and numbers  
- Improve long-term maintainability  
- Ensure Canvas and SVG share a single source definition  

---

### Export Controls Enhancement

Planned additions:

- Transparent vs solid background toggle (PNG)  
- Export scale multiplier  
- SVG stroke scaling toggle  

---

## Version Targets

| Version | Focus |
|---------|--------|
| v1.0.0  | Initial public release |
| v1.1.0  | Numbers + punctuation |
| v1.2.x  | Symbol expansion + connector refinement |
| v1.3.x  | Structural refactor + export improvements |

---

## Long-Term Vision

- Fully extensible glyph definition engine  
- Multiple connector styles  
- Glyph preview palette  
- Themed rendering presets  
- Advanced export configuration  
