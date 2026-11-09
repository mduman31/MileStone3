## Project Milestone 3: Accessibility & Visual Design Refinements

### 1. Accessibility & WAVE Fixes
* **WAVE Fix 1:** Added explicit `alt="Biscuit Macaroni the puppy guarding our family farm"` attributes to all images to ensure screen readers can describe visual context to visually impaired users.
* **WAVE Fix 2:** Fixed missing document structure by ensuring every page starts with a sequential `<h1>` header, preventing assistive technologies from skipping structural layout points.
* **WAVE Fix 3:** Linked all form `<label>` elements explicitly to their corresponding `<input>` tags using matching `for` and `id` properties so fields are read correctly when focused.
* **WAVE Fix 4:** Swapped out low-contrast gray text links for high-contrast matte teal `#2A75D3` over light backgrounds to pass WebAIM WCAG AA requirements.

### 2. Visual Design & Gestalt Principles
* **Principle of Proximity:** I grouped my personal biography, family metrics (6 kids, 2 stepboys), and tech education milestones inside closely bounded cards with tight vertical margins to indicate they belong to a single cohesive profile.
* **Principle of Continuity:** I used a consistent top navigation banner and aligned grid lines across all three pages to naturally guide the user's eyes from left to right along our developmental roadmap.
* **Color Palette (WCAG AA Compliant Matte Tones):**
  * Primary Dark Background/Headers: `#1E293B` (Deep Slate Blue)
  * Accent Tech Teal Link Color: `#0284C7` (High-Contrast Sky Blue)
  * Page Body Background: `#F8FAFC` (Matte Light Slate Pearl)
  * Text Color: `#0F172A` (Rich Dark Slate - Over 7:1 contrast ratio)

### 3. Accessible Contact Form Architecture
* **Semantic Elements:** Utilized `<fieldset>` and `<legend>` to wrap and identify the user credentials block.
* **Aria Attributes:** Employed `aria-live="assertive"` on dynamically updated error zones to announce layout mistakes immediately to screen reader users without using blocking JavaScript `alert()` boxes.
