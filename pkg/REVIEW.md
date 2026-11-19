# Report Review: Group 9 FUX AI-AMWS

## Overall Impression

Vipul has done a genuinely excellent job. This is a **very strong 10-page report** — well-structured, densely evidence-grounded, theoretically rigorous (Norman, Rasmussen, Reason), and methodologically honest in its self-critique. The writing is academic and tight. The LaTeX typesetting is professional.

That said, here's a thorough pass addressing your three suggestions and additional observations.

---

## 1. 🎙️ Audio Transcripts — Your Suggestion

The report mentions audio recordings twice:
- §4.2 says *"raw audio recordings are withheld from public hosting and preserved under confidential academic custody"*
- The repo has an audio file: `ground work 2/WhatsApp Audio 2026-11-18 at 4.13.26 PM.mp4`
- There's already a written summary in [`ground work 2/conversation.txt`](file:///tmp/FoUI/ground%20work%202/conversation.txt) based on the P1 interview

**What I'd recommend:**
- Transcribe the audio (Hindi/Gujarati → English), keeping it anonymised
- Add the transcript as an **appendix** or put it in the repo under `pkg/transcripts/`
- In the report's §4.2 or Acknowledgements, add a line like: *"Anonymised English transcripts of audio-recorded staff inquiries are archived in the project repository (`transcripts/`); raw audio is withheld to protect voice biometrics."*
- The conversation.txt already has a good written summary of P1's interview — you could formalise this as the transcript and reference specific quotes with timestamps

> [!IMPORTANT]
> Since the report mentions "qualitative transcripts and summaries are archived in the project repository" (§4.2, line 254), the reader expects to find them there. Currently, only `conversation.txt` exists. Making this more formal strengthens the claim.

---

## 2. 📐 Figure 4 (a, b) — Positioning & Orientation

**The problem:** Both `p_broken.jpg` (Fig 4a) and `p_pedal.jpg` (Fig 4b) are **rotated 90°** — they appear sideways/tilted in their original files. When placed side-by-side in the two-column layout, they look misaligned because:
- Fig 4a (blue bin with cracked flap) is shot at a tilted downward angle
- Fig 4b (domestic pedal bin) is photographed from a different angle/orientation entirely
- Neither has been cropped or straightened to align visually

**LaTeX code (lines 207–212 of report.tex):**
```latex
\begin{figure}[!ht]
\centering
\begin{subfigure}[t]{0.485\columnwidth}\includegraphics[width=\linewidth]{fig/p_broken.jpg}...
\begin{subfigure}[t]{0.485\columnwidth}\includegraphics[width=\linewidth]{fig/p_pedal.jpg}...
```

**Recommended fixes:**
1. **Rotate the source images** so both bins appear upright (use `\includegraphics[width=\linewidth,angle=90]` or pre-process with ImageMagick)
2. **Add a fixed height** to make them visually aligned: `height=4.5cm,keepaspectratio` on both
3. **Crop** to focus on the bin itself — both images have a lot of surrounding floor/wall

Suggested LaTeX:
```latex
\begin{subfigure}[t]{0.485\columnwidth}
  \includegraphics[width=\linewidth,height=4.5cm,keepaspectratio,trim=0 0 0 0,clip]{fig/p_broken.jpg}
  \caption{Cracked swing flap beside an open yellow bin.}
\end{subfigure}\hfill
\begin{subfigure}[t]{0.485\columnwidth}
  \includegraphics[width=\linewidth,height=4.5cm,keepaspectratio,trim=0 0 0 0,clip]{fig/p_pedal.jpg}
  \caption{Domestic pedal bin, orange liner, solvent cans.}
\end{subfigure}
```

---

## 3. 🖼️ Figures 7–10 — Quality Assessment

Here's my honest take on each:

| Figure | File | Verdict | Notes |
|--------|------|---------|-------|
| **Fig 7** (Swiss cheese) | `fig_swiss.png` | ✅ **Keep** | Simple, clean, and effectively communicates Reason's model. The cheese-slice metaphor is well-rendered with clear before/after. This is good. |
| **Fig 8** (Architecture) | `fig_arch.png` | ✅ **Keep** | Clean block diagram with the 4-tier structure. Professionally made, colour-coded, readable. No issues. |
| **Fig 9** (Station concept) | `fig_station_generated.png` | ⚠️ **Consider replacing** | This is an AI-generated 3D render composited with the technical `fig_station.png` diagram. The 3D render (left side) has that uncanny "AI art" look — the hand has a glove that looks slightly off, text on bins is slightly garbled ("GLASSHER"), and the biohazard symbols look a bit fuzzy. The clean technical diagram version (`fig_station.png`) is actually much better and more professional. |
| **Fig 10** (UI mockups) | `fig_ui_generated.png` | ⚠️ **Consider replacing** | The phone and laptop mockups are AI-generated and have tell-tale artifacts: "Prierity-ranked" (typo), "KPI KPI" (duplicated), and the floor plan inside the dashboard is oddly overlaid. The clean `fig_ui.png` technical version would be better if it exists. |
| **Fig 11** (Floor plans) | `fig_plans.png` | ✅ **Keep** | Very clean, the current-vs-proposed comparison is effective and reads well. |

**My recommendation for Fig 9 & 10:**
- The original technical/clean versions (`fig_station.png` for Fig 9) are more professional. Use those instead of the AI-generated renders.
- For the UI mockups (Fig 10), either:
  - Create proper wireframes in Figma/draw.io (fastest option)
  - Fix the typos and artefacts in the generated version
  - Or use the cleaner `fig_ui.png` if available
- The report already disclaims them: *"Concept visualization rendered using generative image modeling with composite technical diagrams"* — which is good, but the AI artefacts ("GLASSHER", "Prierity", "KPI KPI") undermine credibility

> [!TIP]
> If you want to keep the AI-generated renders, at minimum fix the text artefacts. The typo "Prierity-ranked" on the phone screen and "KPI KPI" on the dashboard are noticeable on close inspection.

---

## 4. 📝 Additional Observations (Full Report Pass)

### Minor Issues

| Location | Issue | Suggestion |
|----------|-------|------------|
| §1.2, line 60 | Acronym "ASS" for "Attentive Segregation System" — this is acknowledged as the prior group's naming, but it reads... awkwardly | Nothing to do — it's their name, and the report handles it respectfully |
| §5.10, Table 4 | "Our plan marks 10 locations (Fig. 11A; the field-note summary lists 8, a discrepancy we have not yet resolved)" | Good that it's flagged, but try to resolve it before submission. Count the red dots in Fig 11A — there are exactly 10. If the field notes say 8, clarify which 2 are supplementary |
| §5.8, line 598 | The 72-hour vs 48-hour compliance gap is a strong finding. It's mentioned multiple times across §5.8, §7.6, and Table 4 | Could be slightly consolidated to avoid repetition, but honestly it's fine given how important the point is |
| §6.4 / Table 5 | "the briefing given to the peer evaluators is not documented in this report; both are limitations" | This is commendable transparency. No action needed |
| §7.8, BOM | Very detailed and well-researched BOM. The ≈87 INR/USD exchange rate is reasonable for 2026 | ✅ No issues |
| References | 35 references for a 10-page UX critique is excellent. All seem legitimate and properly cited | ✅ Solid |

### Typographic / Formatting

| Location | Issue |
|----------|-------|
| Table 3 (card-sort matrix) | The extracted text shows this table reads well, but in the PDF the alignment of K column values should be double-checked |
| §4.2 bullet 3 | "semi-structured contextual inquiries" — this paragraph is quite dense. Consider splitting into sub-bullets for Visit 1 and Visit 2 |
| Fig 5 caption | "single photograph; indicative" — nice disclaimer |

### Strengths Worth Noting

- **Inter-rater reliability** (§4.4, §5.4): Computing Cohen's κ and reporting raw agreement percentages is methodologically strong for a course project
- **Luminance contrast analysis** (§5.7): Computing WCAG contrast ratios for physical bins against walls is creative and rigorous
- **Evidence-grounding table** (Table 7): Explicitly mapping each design decision to field evidence, literature, and what's unvalidated is excellent academic practice
- **Self-critique** (§9.2): Remarkably honest about limitations — Hawthorne effect, proxy sample vs. actual patients, single-operator account, etc.
- **Phased approach** (Phase 0 → 1 → 2): Shows design maturity — standardise before sensing, sense before predicting

---

## Summary of Recommended Changes

| Priority | Change | Effort |
|----------|--------|--------|
| 🔴 High | Add audio transcripts (at least in repo, reference in §4.2) | Medium — needs transcription + translation |
| 🟡 Medium | Fix Figure 4 (a,b) orientation/alignment | Low — rotate images + adjust LaTeX |
| 🟡 Medium | Replace Fig 9 with clean `fig_station.png` version | Low — swap the file reference in LaTeX |
| 🟡 Medium | Fix or replace Fig 10 (UI mockups) — at minimum fix "Prierity", "KPI KPI", "GLASSHER" | Medium — re-generate or make wireframes |
| 🟢 Low | Resolve the 10 vs 8 bin location discrepancy (§5.10) | Low — recount and update text |
| 🟢 Low | Minor text consolidation of 72h/48h gap across sections | Low |
