```markdown
# Design System Strategy: Luxury Wellness Editorial

## 1. Overview & Creative North Star
**The Creative North Star: "The Curated Sanctuary"**

This design system moves away from the sterile, clinical aesthetic of traditional "pharmacy" branding and embraces the world of high-end editorial wellness. Our goal is to create a digital experience that feels like a private consultation in a luxury lounge—hushed, intentional, and deeply premium. 

We break the "template" look by utilizing **intentional asymmetry** and **tonal depth**. Instead of a rigid grid of boxes, we use overlapping elements, vast "negative" space to let product photography breathe, and a dramatic typography scale that balances the authority of a serif with the modernity of a clean sans-serif. Every pixel must feel like a deliberate choice, not a default setting.

---

## 2. Colors & Atmospheric Depth
The palette is rooted in the "Dark Mode" of nature—night forests and raw minerals—punctuated by the warmth of gold and the vitality of emerald.

### Surface Hierarchy & Nesting
We reject the flat UI. We build depth through **Tonal Layering**.
*   **Base Layer:** `surface` (#131313) is our canvas.
*   **Elevated Containers:** Use `surface-container-low` (#1C1B1B) for large sectioning and `surface-container-high` (#2A2A2A) for interactive cards.
*   **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. Boundaries are defined solely by background shifts. To separate a feature section from the hero, transition from `surface` to `surface-container-low`.

### The "Glass & Gold" Signature
*   **Glassmorphism:** Use `surface-variant` with a 60% opacity and a `24px` backdrop blur for floating navigation bars or overlay modals. This creates a "frosted obsidian" effect.
*   **Luminous Accents:** Use the `primary` (#F2CA50) for high-impact CTAs. Apply a subtle linear gradient from `primary` to `primary-container` (#D4AF37) at a 135-degree angle to give the gold "soul" and metallic dimension.

---

## 3. Typography: The Editorial Voice
Typography is our primary tool for persuasion. We pair the intellectual weight of a Serif with the functional clarity of a Geometric Sans.

*   **Display & Headlines (Noto Serif):** These are our "hero" moments. Use `display-lg` for value propositions. The Serif conveys heritage, trust, and luxury.
*   **Body & UI (Manrope):** All functional text uses Manrope. Its wide apertures maintain legibility against dark backgrounds, preventing "light bleed" (halation) which often plagues dark-mode designs.
*   **Hierarchy Tip:** For a premium editorial feel, use `label-md` in all-caps with a `0.1em` letter-spacing for category tags or "eyebrow" headlines above main titles.

---

## 4. Elevation & Depth
We define space through light and shadow, mimicking natural environments.

*   **The Layering Principle:** To lift a card, place a `surface-container-highest` card atop a `surface-container-low` section. This creates a "soft lift."
*   **Ambient Shadows:** For floating elements, use a shadow with a `40px` blur, 0% spread, and 8% opacity. The shadow color should be `#000000`, creating a natural fall-off rather than a "dirty" grey smudge.
*   **The "Ghost Border" Fallback:** If a container requires definition against a similar background (e.g., product images), use a `1px` stroke of `outline-variant` at **15% opacity**. It should be felt, not seen.
*   **Emerald Vitality:** Use `secondary` (#88D982) sparingly. It is not a primary UI color; it is a "biological accent"—use it for success states, health-benefit icons, or organic highlights.

---

## 5. Components

### Buttons (The "Jewelry" of the UI)
*   **Primary:** Solid `primary` (Gold) with `on-primary` text. Use `full` roundedness (capsule) for a modern, ergonomic feel.
*   **Secondary:** `Ghost Border` (outline-variant at 20%) with `primary` text. No fill.
*   **Tertiary:** No border, no fill. `primary` text with a `label-md` weight.

### Premium Cards
*   **Layout:** Forbid divider lines. Use `32px` padding (internal) and background shifts to separate the image from the text.
*   **Interaction:** On hover, a card should transition from `surface-container-high` to `surface-container-highest` and receive a subtle `primary` (gold) outer glow (5px blur, 10% opacity).

### Input Fields
*   **Base:** `surface-container-lowest` background with a bottom-only `1px` border of `outline-variant` (20% opacity). 
*   **Focus State:** The bottom border animates to 100% opacity `primary` (gold). This minimalist approach avoids the "clunky box" look of standard forms.

### Selection Chips
*   **Unselected:** `surface-container-high` background, no border.
*   **Selected:** `primary-container` background with `on-primary-container` text. Use `sm` (0.125rem) roundedness for a sharper, more "architectural" look.

---

## 6. Do’s and Don’ts

### Do:
*   **Do** use high-quality, lifestyle photography with dark, moody lighting that complements the graphite base.
*   **Do** embrace extreme white space. If you think there is enough space between sections, double it.
*   **Do** use the Emerald Green (`secondary`) only for elements related to "Life," "Growth," or "Health"—never for decorative UI lines.

### Don't:
*   **Don't** use pure white (#FFFFFF) for body text. Use `on-surface-variant` (#D0C5AF) to reduce eye strain and maintain the "warm" luxury feel.
*   **Don't** use standard "Drop Shadows." Use tonal layering.
*   **Don't** use icons with heavy fills. Use light, `1.5pt` stroke-based icons that match the `outline` token.
*   **Don't** use "pharmacy green." If a green feels too bright, it’s wrong. It must feel like a deep, emerald leaf in a shadowed forest.

---

## 7. Spacing & Rhythm
We follow a 4px-base grid, but for luxury, we favor **Large-Scale Spacing**:
*   **Section Gaps:** Use `80px` to `120px` to separate major content blocks.
*   **Inner Card Spacing:** Use `24px` or `32px` to ensure content never feels cramped. 
*   **The Golden Ratio:** When placing text over images, use an asymmetrical 60/40 split to create a more dynamic, editorial composition.```