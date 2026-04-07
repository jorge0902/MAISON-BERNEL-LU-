```markdown
# Design System: The Crimson Nocturne

## 1. Overview & Creative North Star

This design system is orchestrated around the Creative North Star of **"The Seductive Curator."** It is a digital experience that mirrors the olfactory transition from a crisp Parisian evening to the heavy, incense-laden opulence of a Dubai night. 

To move beyond the predictable "luxury template," this system rejects rigid symmetry in favor of **Intentional Editorial Imbalance.** We utilize expansive negative space, overlapping high-fidelity imagery, and a typographic scale that values "the silence between notes" as much as the content itself. This is not a website; it is a digital vault of sensory experiences.

---

## 2. Colors: Tonal Depth & Liquid Light

The palette is anchored in the deep, visceral red of a pomegranate’s heart and the reflective qualities of polished gold.

### Core Palette
- **Primary High-Contrast:** `primary` (#ffb3ad) and `primary_container` (#861117) represent the ruby liquid.
- **Opulence Accents:** `secondary` (#e9c349) and `secondary_container` (#af8d11) provide the "gold foil" sheen.
- **The Void:** `surface` (#131313) and `surface_container_lowest` (#0e0e0e) provide the matte black foundation.

### The "No-Line" Rule
Luxury is seamless. **1px solid borders are strictly prohibited for sectioning.** Boundaries between content must be defined exclusively through:
1.  **Tonal Shifts:** Transitioning from `surface` to `surface_container_low`.
2.  **Atmospheric Gradients:** Using sophisticated dark gradients that move from `surface` to a deep `primary_container` (ruby) to guide the eye without structural "fences."

### Glass & Gradient Signature
To evoke the perfume bottle's materiality, floating elements (modals, navigation bars) must utilize **Glassmorphism.** Use semi-transparent `surface_container` colors with a `backdrop-blur` of 20px–40px. CTAs should never be flat; they should utilize a subtle radial gradient from `secondary` to `secondary_fixed_dim` to simulate the curvature of a gold cap.

---

## 3. Typography: The Franco-Arabic Dialogue

The typography is a study in contrast: the historical weight of the French serif and the clinical precision of modern sans-serif.

*   **Display & Headline (Noto Serif):** These are your "Editorial Statements." Use `display-lg` (3.5rem) for hero moments. The serif evokes the heritage of French perfumery. Tighten letter-spacing slightly for a more "expensive" feel.
*   **Body & Labels (Manrope):** The modern sans-serif provides the "Dubai" edge—clean, efficient, and architectural. Use `body-lg` for product descriptions to ensure a premium reading experience.
*   **Hierarchical Tension:** Pair a very large `display-sm` headline with a very small, wide-tracked `label-md` in all-caps gold (`secondary`) to create a high-fashion editorial tension.

---

## 4. Elevation & Depth: Tonal Layering

We do not use elevation to "lift" objects; we use it to "submerge" or "reveal" them within the dark environment.

*   **The Layering Principle:** Depth is achieved by stacking surface tiers. A product detail card (`surface_container_high`) should sit on a section background of `surface_container_low`. This creates a soft, natural "glow" rather than a hard edge.
*   **Ambient Shadows:** If a floating element requires a shadow, it must be an **Ambient Glow.** Use a blur radius of 40px+ with 4-6% opacity, using the `primary_container` color (ruby) instead of black. This mimics light passing through the ruby perfume liquid.
*   **The "Ghost Border" Fallback:** For input fields or essential containment, use the `outline_variant` token at **15% opacity.** It should be felt, not seen.

---

## 5. Components: Sculpted Elements

### Buttons
*   **Primary:** A "Gold Foil" effect. Gradient from `secondary` to `secondary_container`. No border. Text in `on_secondary` (#3c2f00).
*   **Secondary/Ghost:** `outline` token at 20% opacity. Upon hover, the background fills with a microscopic `surface_bright` shimmer.
*   **Shape:** Follow the `sm` scale (0.125rem) for a sharp, architectural look, or `full` for a "soft-touch" pill shape.

### Input Fields
*   **Styling:** Forgo the box. Use a single bottom border (`outline_variant` at 30% opacity). Labels use `label-md` in `on_surface_variant`. 
*   **Error State:** Use `error` (#ffb4ab) but keep the typography in `serif` to maintain the brand's sophisticated voice even in failure states.

### Cards & Lists
*   **Rule:** Forbid all divider lines.
*   **Implementation:** Use vertical whitespace (from the 32px/64px scale) or a subtle shift from `surface_container` to `surface_container_highest` to denote a new item.
*   **Visual Integration:** Product cards should feature imagery that "breaks out" of the container, with pomegranates or gold flakes overlapping the edges to create a 3D effect.

### Selection & Chips
*   For fragrance notes (e.g., "Amber," "Oud"), use chips with a `surface_variant` background and `on_surface` text. Shape should be `full` (pill) to contrast with the sharp edges of the typography.

---

## 6. Do's and Don'ts

### Do
*   **Embrace Asymmetry:** Place a product image off-center and counter-balance it with a small, high-contrast text block.
*   **Use Liquid Imagery:** Every page must feature "Macro Visuals"—high-resolution textures of glass, liquid ripples, or gold foil.
*   **Maintain Breathability:** If you think there is enough white space (or "black space"), double it.

### Don't
*   **No Pure White:** Never use #FFFFFF. Use `on_surface` (#e5e2e1) for a softer, creamier "silk" feel.
*   **No Standard Grids:** Do not align everything to a 12-column grid. Let elements breathe and overlap.
*   **No Generic Icons:** Icons must be ultra-thin (0.5pt or 1pt stroke) or replaced with elegant text labels in `label-sm`.
*   **No High-Opacity Borders:** Never use a 100% opaque border; it breaks the illusion of the "seductive" atmosphere.

---
*Director's Final Note: Every pixel must feel intentional. If an element does not contribute to the "Seductive Curator" persona, remove it. We are not building a store; we are building a desire.*```