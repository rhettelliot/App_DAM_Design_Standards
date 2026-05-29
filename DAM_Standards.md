# DAM Design Standards

---

## 1. Visual Philosophy & Design Tone

Before writing a single line of CSS, establish the core emotional and visual principles.

- **Invisible Sophistication** — The UI should never compete with the assets. If a photographer drops a neon-heavy fashion editorial into the DAM, the interface around it should *frame* it, not clash with it.

- **Tactile Precision** — Every transition, hover state, and interaction must feel heavy and intentional. Think of the dampened mechanical click of a Leica camera or the smooth dial of a high-end audio mixer.

- **Spacious Minimalism** — Luxury brands use whitespace to signal premium quality. Give elements room to breathe, avoiding the cramped, spreadsheet-like feel of legacy enterprise software.

---

## 2. The Color System: Monetizing Monochromes

A high-end media tool requires an **asset-first** color strategy. Your primary palette must be neutral to prevent color cast interference when editors are color-correcting or selecting media.

| Color Token | Use Case / Application | Aesthetic Vibe |
|---|---|---|
| **Deep Obsidian** | Primary UI backgrounds, dark mode surfaces | Deep black, pure cinema contrast |
| **Gallery White** | Light mode surfaces, high-contrast text | Editorial, clean, gallery-wall crispness |
| **Muted Platinum** | Borders, dividers, subtle metadata text | Low-contrast, sophisticated structure |
| **The Signature Accent** | Solitary action buttons, active states | A single, striking color *(e.g., International Klein Blue, Rich Ochre, or Acid Lime)* |

### The 95/5 Rule

95% of your interface should be shades of black, white, and gray. The remaining 5% is reserved for your **signature accent color**, used exclusively to draw attention to critical actions (e.g., *"Publish Delivery Link"*).

---

## 3. Typography: Editorial Meets Utility

High-end software often uses a **dual-font system**: a premium serif for high-level brand moments and an ultra-clean sans-serif or monospaced font for heavy data.

- **Display / Header Font** — A sharp, sophisticated Neo-Grotesque or an elegant Serif *(e.g., PP Neue Montreal, Inter Tight, or Chronicle Display)*. Used for workspace titles, collection names, and top-tier navigation.

- **UI / Metadata Font** — A highly legible, utilitarian Sans-Serif or Variable font *(e.g., SF Pro, Inter, or Roboto Mono for technical specs)*. This handles file sizes, dimensions, aspect ratios, and tag clouds.

---

## 4. Key Component Anatomy

Core DAM components and how they should behave to maintain that premium feel.

### The Media Card *(Hero Component)*

Legacy DAMs pack cards with text, checkboxes, and buttons. A premium DAM treats the card like a **framed photograph**.

- **Idle State** — Pure asset preview. No text overlays, no buttons. Just the media with a perfectly rounded corner (`4px` to `8px` max for a modern, sharp look).

- **Hover State** — A micro-zoom on the image (`1.02×` scale over `300ms` with a smooth `cubic-bezier` curve), accompanied by a subtle, elegant reveal of the file name and a selection checkbox using low-opacity overlays.

### The Metadata Panel *(Inspector)*

When a user inspects an asset, the data layout should look like a **luxury watch spec sheet**.

- Use generous line heights (`1.5` to `1.6`) and clear typographic hierarchy.
- Group technical data (EXIF/IPTC data like ISO, aperture, focal length) into a beautifully spaced, minimal **two-column grid**.

---

## 5. Micro-Interactions & Motion Design

Motion is the secret sauce of expensive software. Clunky, instant snaps feel cheap. Intentionally timed transitions feel **premium**.

- **Loading States** — Ditch the generic looping spinner. Instead, use a sleek, linear *"shimmer"* effect that passes across skeleton screens, or a single, elegant fading brand mark.

- **Drag-and-Drop** — When dragging an asset into a collection, the drop zone should pulse with a soft, blurred glow rather than a harsh dotted border. The asset card should slightly tilt, simulating physics.

- **Transitions** — All drawer panels (like the metadata inspector) should slide in using an `ease-out` curve (`400ms` duration), giving the impression of a heavy, well-oiled mechanical drawer.