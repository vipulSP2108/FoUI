# Historical Baseline Reference Database (Pre-Renovation Medical Centre)

**Data Classification:** Strictly Internal Baseline Reference Dataset  
**Facility Context:** Old IITGN Medical Centre (Pre-Renovation Setup)  
**Primary Function:** Longitudinal comparative baseline for Group 9's evaluation of the renovated facility  

---

## 1. Historical Operational Baseline

* **Daily Patient Footfall:** 100 to 150 patients/visitors daily (students, faculty, campus staff, external dependents).
* **Total Waste Bins Audited:** 15 bins distributed across five primary clinical zones.
* **Collection Schedule:** Once-daily internal custodial sweep; daily external municipal bio-hazard collection by authorized agency.
* **Governing Regulatory Standard:** Central Pollution Control Board (CPCB) Bio-Medical Waste Management Rules, 2016.

---

## 2. Room-by-Room Distribution & Observed Breakdown Issues

| Functional Room | Waste Bins Present | Observed Usability & Operational Breakdown Issues |
| :--- | :--- | :--- |
| **Doctor Cabin 1** | Yellow (Infectious), Red (Plastics) | High polybag-to-bin color mismatch; poor luminance contrast against floor tiles; hurried disposal by physicians leading to category slips. |
| **Treatment Room** | Yellow, Blue (Glass), Sharps Container | Severe afternoon overfilling (15:00–17:00); sharps container mounted at awkward ergonomic angle; high risk of cross-contamination during rush procedures. |
| **Sample Room** | Red, White (Puncture-Proof Sharps) | Faded handwritten stickers; poor localized task lighting causing color misidentification; zero visual feedback upon disposal. |
| **Observation Area** | Yellow, Black (General Waste) | Severe patient/visitor misuse; general solid waste (wrappers, tissues) routinely discarded into hazardous Yellow bins due to ambiguous affordances. |
| **Corridors & Hallways** | General Waste Receptacles | Frequent mis-segregation by visitors; lack of intuitive signifiers; bins positioned in peripheral visual blind spots. |

---

## 3. Historical Ethnographic Observation Schedule

The baseline study conducted 255 minutes of structured field observations across three targeted operational windows:

| Session ID | Time Window | Target Locations Audited | Focus of Inquiry |
| :--- | :--- | :--- | :--- |
| **Day 1** | 09:30–11:00 (90 min) | Treatment Room, Doctor Cabins | High clinical activity, doctor-nurse handoffs, urgent disposals. |
| **Day 2** | 15:00–16:15 (75 min) | Sample Room, Public Corridor | Specimen handling, blood draws, visitor footfall patterns. |
| **Day 3** | 17:00–18:30 (90 min) | Observation Ward, Hallways | Evening rush, visitor waiting behaviors, cleaning staff bag clearance. |

### Stakeholder Interview Demographics
* **5 Staff Nurses:** Reported severe cognitive fatigue during rush hours, frustration with ill-fitting polybags, and reliance on spatial habit rather than reading bin labels.
* **3 Housekeeping Staff:** Reported physical strain lifting heavy, overfilled bags, frequent punctures from improperly segregated sharps, and lack of notification before bins overflowed.
* **2 Administrative Officers:** Focused on municipal compliance risks, supply chain delays for color-coded bags, and audit documentation burdens.

---

## 4. Quantitative Audit Metrics & Variables Recorded

The baseline audit tracked seven operational variables:
1. **Bin Colour / Category:** Categorical (Yellow, Red, Blue, White, Black).
2. **Waste Material Observed:** Anatomical, plastic, glass, sharp, municipal.
3. **Bag Mass (grams):** Measured via digital hanging scale upon bag sealing.
4. **Mis-Segregated Items (count):** Quantified items placed into incorrect waste streams.
5. **Fill-Level Estimate (%):** Visual percentage estimation at replacement time.
6. **Time of Replacement (HH:MM):** Timestamp of custodial bag removal.
7. **Room / Specific Location:** Categorical functional zone.

---

## 5. Computer Vision & Environmental Contrast Analysis

To investigate why medical staff committed disposal slips, the baseline study executed algorithmic color analysis using Python and OpenCV:

### 5.1 Chromatic Analysis (HSV & CIELAB Space)
* Measured RGB and HSV histograms of bins under hospital fluorescent lighting.
* Quantified color degradation and label fading against standard CPCB color vectors ($\Delta E$ color deviation).
* Proved that aged Yellow and Red bins faded substantially, drifting toward neutral amber and brown hues.

### 5.2 Environmental Contrast Ratios ($L_1 / L_2$)
* In-situ photographs analyzed bin bodies against surrounding floor tiles and wall paint.
* **Finding:** Institutional cream and beige wall paint exhibited dangerously low contrast ratios ($<2.5:1$) with Yellow and Red bins. Bins effectively blended into the visual background, causing cognitive tunnel vision and hesitation for staff under stress.

---

## 6. Synthesis: The "Attentive Segregation System (ASS)" Concept & Its Critical Limitations

### 6.1 What the Baseline Study Proposed
Group 8 conceptualized the **Attentive Segregation System (ASS)**:
* **Physical Structure:** 800×1000 mm acrylic backplate; 30L Yellow HDPE bin, 30L Red HDPE bin, 20L Blue HDPE bin, 2–3L PP sharps box; laminated A5/A6 bilingual signage.
* **Electronics Module:** Single ESP32 MCU, 3× HC-SR04 ultrasonic distance sensors, 0.96-inch monochrome I2C OLED display, addressable NeoPixel RGB LED strip, micro-SD logging module, 12V/5V power converter.
* **Firmware Behavior:** Monitored ultrasonic fill distance; triggered green tick / red cross icons on OLED; issued alerts when fill exceeded 80%.

### 6.2 Critical UX & Architectural Limitations of the Baseline Concept
Group 9's project directly addresses the significant operational gaps left open by this baseline system:
1. **Rigid, Static Physical Footprint:** The 30L/20L bin capacities were permanently fixed. On heavy procedure days (e.g., campus vaccination drives or seasonal outbreaks), the Yellow bin rapidly overwhelmed while the Red bin remained nearly empty.
2. **Purely Reactive Thresholding:** Issuing an alert only after reaching 80% capacity provides zero advance notice. Custodial staff often take 20–30 minutes to respond, leading to inevitable overflows.
3. **Isolated Room Islanding:** The system treated each room as a silo, unable to share capacity data or recommend cross-room load rebalancing across the facility.
4. **Zero Item Verification:** Relying strictly on ultrasonic distance meant the system could not determine *what* item was dropped—a hazardous needle could be dropped into the general bin without detection.

