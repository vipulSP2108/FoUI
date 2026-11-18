# Regulatory BMW Standards & HCI Theoretical Reference Library

**Document Purpose:** Academic citations, regulatory mandates, and theoretical frameworks grounding the project  

---

## 1. Indian Bio-Medical Waste Management (BMW) Rules, 2016

Published by the Ministry of Environment, Forest and Climate Change (MoEFCC) and regulated by the Central Pollution Control Board (CPCB):

### Color Coding & Segregation Schedule

| Category / Color | Permissible Waste Types | Container / Bag Specifications | Mandatory Treatment & Disposal Stream |
| :--- | :--- | :--- | :--- |
| **Yellow** | Human & animal anatomical waste, soiled cotton, bandages, plaster casts, expired/cytotoxic drugs, chemical waste. | Non-chlorinated yellow plastic bags with biohazard symbol. | Incineration or Plasma Pyrolysis; Deep burial only in remote areas. |
| **Red** | Contaminated recyclable plastics: disposable tubing, IV bottles, catheters, urine bags, disposable gloves, syringes without needles. | Non-chlorinated red plastic bags or autoclavable containers. | Autoclaving or microwaving followed by shredding; plastic sent to registered recyclers. |
| **Blue** | Contaminated broken or intact glassware, medicine vials, glass ampoules, metallic orthopedic implants. | Puncture-proof, leak-proof cardboard box or plastic container with blue marking. | Disinfection (sodium hypochlorite) or autoclaving followed by glass recycling. |
| **White (Translucent)** | Waste sharps: contaminated needles, scalpels, surgical blades, fixed-needle syringes, contaminated trocars. | Rigid, puncture-proof, tamper-proof, translucent container. | Dry heat sterilization or autoclaving followed by shredding / encapsulation. |
| **Black / Green** | Non-biomedical municipal solid waste: paper wrappers, office waste, non-contaminated food remnants. | Standard municipal bins (Black/Green). | Handled under Solid Waste Management (SWM) Rules, 2016. |

---

## 2. Foundational HCI & Human Factors Theoretical Frameworks

### 2.1 Don Norman: Cognitive Engineering & The Design of Everyday Things
* **Affordance:** The physical properties of a waste station signaling its function. A round narrow opening affords dropping vials; a wide foot-pedal lid affords bulky gauze disposal.
* **Signifier:** High-luminance colored LED rings and clear pictograms that communicate *where* specific waste streams belong without requiring text deciphering.
* **Mapping:** The spatial congruence between where clinical procedures take place and where bins are positioned. Poor mapping forces nurses to turn $180^\circ$ and walk across rooms.
* **Feedback:** Instant, multi-modal acknowledgment that the user's action was registered (e.g., green LED confirmation pulse).
* **Constraints:** Physical and visual boundaries preventing wrong disposal (e.g., small slots preventing large general trash bags from entering sharps containers).
* **Gulf of Execution:** The cognitive effort required for a nurse to translate an intention (*"I need to discard this blood-soaked syringe body"*) into physical action (*"Which bin does it go into?"*).
* **Gulf of Evaluation:** The cognitive effort required to assess whether the disposal was correct and safe.

### 2.2 Jens Rasmussen: Skills, Rules, Knowledge (SRK) Framework
* **Skill-Based Behavior:** Highly automated, sensory-motor disposal performed routinely by experienced nurses. Highly susceptible to **action slips** when attention is captured by patient distress.
* **Rule-Based Behavior:** Applying memorized protocols (e.g., *"If plastic tubing, use Red bin"*). Vulnerable to **rule misapplication** if signage is ambiguous or contradictory.
* **Knowledge-Based Behavior:** Deliberate, conscious problem-solving when encountering novel items (e.g., a multi-material disposable surgical kit). Requires clear ambient signifiers and instant system confirmation.

### 2.3 James Reason: Human Error & The Swiss Cheese Model
In safety-critical hospital environments, accidents rarely stem from isolated human failure. Instead, they occur when latent organizational failures align with active slips:
* **Latent Failures:** Faded bin labels, institutional beige walls matching bin colors, rigid custodial pickup schedules, ill-fitting replacement polybags.
* **Active Failures:** Clinician fatigue, rush during emergency resuscitation, cognitive tunnel vision.
* **AI-AMWS Intervention:** Closes the "holes in the cheese" by introducing active, redundant defenses: ambient chromatic lighting, predictive surge forecasting, and real-time custodial dispatching.

