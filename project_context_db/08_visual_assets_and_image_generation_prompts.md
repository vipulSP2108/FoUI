# Visual Assets, Figure Pipeline & Image Generation Prompts

**Document Classification:** Figure Production Database & LaTeX Placeholder Reference  

---

## 1. Visual Strategy Overview
The final 10-page LaTeX report integrates three complementary categories of visual assets:
1. **Category 1: Real Field Photos** taken at the renovated IITGN Medical Centre.
2. **Category 2: Historical Comparison Screenshots** extracted from the baseline dataset.
3. **Category 3: Conceptual Diagrams & Renders** generated via AI image generation prompts or technical schematics.

---

## 2. Category 1: Real Ground Photos & Floor Plans (Captured by Group 9)

The team captured 12 real field assets stored in `ground work/`. These provide indisputable empirical proof of the failure modes discussed:

| Asset ID | Actual File Path | Visual Subject & Scene Framing | Analytical Purpose & LaTeX Tag |
| :--- | :--- | :--- | :--- |
| `FIG_REAL_BUFFER` | `ground work/outsidebins.jpeg` | Exterior balcony corridor buffer rack: 4 large pedal bins (Black, Blue, Red, Yellow). | Documents the buffer-only renovation intervention. `\label{fig:real_buffer_rack}` |
| `FIG_REAL_OVERFLOW` | `ground work/20261110_120528.jpg.jpeg` | Under-counter floor cluster: overflowing red bucket (syringe wrappers), pink bucket (uncapped syringes in orange bag), beige bucket (blood cotton). | Severe segregation breakdown, open unlidded buckets, and biohazard overflow. `\label{fig:real_overflow_cluster}` |
| `FIG_REAL_MISMATCH` | `ground work/20261110_120956.jpg.jpeg` | Wall lineup: light blue pedal bin with **yellow biohazard liner**, open orange/blue buckets, chemical jugs on bare floor. | Extreme visual mismatch and contradictory color signifiers. `\label{fig:real_color_mismatch}` |
| `FIG_REAL_BROKEN` | `ground work/20261110_120649.jpg.jpeg` | Blue swing-top bin with **cracked/broken flap** next to open yellow bin with soiled gauze. | Mechanical affordance breakdown forcing manual contact. `\label{fig:real_broken_pedal}` |
| `FIG_REAL_PEDAL` | `ground work/20261110_120642.jpg.jpeg` | Domestic pink pedal bin with grey lid and orange bag next to disinfectant cans. | Non-standard domestic hardware in clinical procedure space. `\label{fig:real_domestic_bin}` |
| `FIG_PLAN_RAW` | `ground work/rough_realplan.jpeg` | Hand-drawn architectural floor plan of renovated Medical Centre drawn on-site during initial walkthrough. | Baseline architectural footprint of renovated facility. `\label{fig:plan_hand_drawn}` |
| `FIG_PLAN_CURRENT` | `ground work/current_binplan.jpeg` | Floor plan overlay with 8 red dots marking current problematic bin coordinates. | Spatial circulation bottlenecks and corner clustering. `\label{fig:plan_current_bins}` |
| `FIG_PLAN_PROPOSED`| `ground work/proposed_binplan2.jpeg` | Floor plan with multi-tier red/green dots showing AI-AMWS optimized bin allocations. | Proposed ergonomic zoning and reach optimization. `\label{fig:plan_proposed_bins}` |

---

## 3. Category 2: Historical Baseline Screenshots (From Reference PDF)

| Asset ID | Reference Source in Baseline PDF | Subject & Purpose | LaTeX Figure Tag |
| :--- | :--- | :--- | :--- |
| `FIG_HIST_01` | **Fig. 2 (Page 3)** | Schematic floor plan of old Medical Centre showing 15 bin locations across 5 rooms. | `\label{fig:hist_old_floorplan}` |
| `FIG_HIST_02` | **Fig. 4 (Page 4)** | In-situ photos showing yellow and red bins blending into cream wall tiles. | `\label{fig:hist_wall_blending}` |
| `FIG_HIST_03` | **Fig. 8 (Page 5)** | Simplified user journey flow diagram for clinical disposal and housekeeping. | `\label{fig:hist_user_journey}` |
| `FIG_HIST_04` | **Fig. 9 (Page 6)** | Affinity diagram summarizing qualitative clusters (Visibility, Feedback, Constraints). | `\label{fig:hist_affinity_diagram}` |

---

## 4. Category 3: AI Image Generation Prompts (Ready-to-Use)

Use these prompts in Midjourney (v6), Google Imagen 3, or DALL-E 3:

### Diagram 1: AI-AMWS System Architecture Diagram
* **Asset ID:** `FIG_AI_ARCH`
* **LaTeX Placeholder:** `[DIAGRAM PLACEHOLDER: AI-AMWS System Architecture Diagram]`
* **Prompt:**
  > `"A sleek, professional technical system architecture diagram for an AI-powered smart hospital waste management system. On the left, an IoT-enabled medical waste bin station inside a modern clinic room with sensor waves emanating from ultrasonic and optical sensors. In the center, a glowing cloud-based AI predictive engine showing neural network nodes and time-series forecasting graphs. On the right, two outputs: a mobile smartphone screen displaying an optimized custodial routing map, and a desktop hospital administration dashboard displaying real-time bin capacity heatmaps. Clean engineering schematic style, isometric vector art, dark slate background with cyan and amber accents, crisp typography, 8k resolution, photorealistic studio lighting."`

### Diagram 2: Interactive Smart Bin UI/UX Physical Concept
* **Asset ID:** `FIG_AI_BIN_CAD`
* **LaTeX Placeholder:** `[DIAGRAM PLACEHOLDER: Interactive Smart Bin UI/UX Layout]`
* **Prompt:**
  > `"Industrial design rendering of a state-of-the-art hospital biomedical waste station, front 3/4 perspective. Four modular, hygienic stainless-steel and antimicrobial matte-finish composite compartments aligned horizontally. Each aperture features a recessed glowing diffused LED rim ring corresponding to medical waste standards: deep Yellow, vibrant Red, bright Blue, and matte Charcoal Black. A subtle capacitive touchless sensor icon is visible near each aperture. The front face features a vertical slender digital LED fill-level progress bar. High-end medical equipment aesthetics, sterile clinical environment, soft directional lighting, photorealistic product photography, ultra-detailed."`

### Diagram 3: Spatial Floor Plan Comparison & AI Heatmap
* **Asset ID:** `FIG_AI_FLOORPLAN`
* **LaTeX Placeholder:** `[DIAGRAM PLACEHOLDER: Old vs. New Room Layout and Dynamic Bin Heatmap]`
* **Prompt:**
  > `"An architectural 2D top-down isometric hospital floor plan comparison. On the left side labeled 'Current Static Layout', red exclamation marks show congested, overflowing waste bins tucked awkwardly into treatment room corners. On the right side labeled 'AI-Optimized Adaptive Layout', clean green circulation pathways show dynamically positioned modular waste stations with glowing coverage radius circles indicating optimal ergonomic reach for doctors and nurses. Clean CAD blueprint style, white background with blue and slate line work, professional architectural presentation."`

### Diagram 4: Custodial Mobile App & Admin Dashboard UI
* **Asset ID:** `FIG_AI_UI_MOCKUP`
* **LaTeX Placeholder:** `[DIAGRAM PLACEHOLDER: Custodial Mobile App & Facility Admin UI]`
* **Prompt:**
  > `"UI/UX interface mockup display. A modern bezel-less smartphone showing a mobile custodial dispatch app with a clean floor plan map, turn-by-turn waste collection route, and urgency badges ('Yellow Bin - Minor OT at 88% capacity - Urgent'). Floating next to it is a desktop browser window showing a facility management analytics dashboard with predictive bar charts forecasting weekly waste volume surges, peak hours, and contamination incident logs. Modern Figma UI design style, clean typography, vibrant data visualization cards, subtle drop shadows."`

