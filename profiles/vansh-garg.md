# Vansh Garg

| Field | Value |
|---|---|
| Current role | Student researcher, **IIIT Hyderabad RRC** (since Aug 2024), with Prof. K. Madhava Krishna (mentors Sourav Garg, Siddharth Tourani): robot navigation with geometric (3D) foundation models [CC] H026 H027 |
| Location / willing to move | Hyderabad [CC] H026 |
| Education | **B.Tech + MS (dual degree) Computer Science, IIIT Hyderabad, 2021–2026** [CC] H026. Site calls him "a master's student at RRC"; graduation date not stated [CC] H027. Vishal: still in his master's [INT Vishal 2026-11-28] |
| Previous | Undergraduate Researcher, **CVIT** IIIT-H (May 2023 – Jan 2025), with Profs. C.V. Jawahar and Vinay Namboodiri: lip-reading / lip-to-speech [CC] H026 · CoRL 2026 reviewer [CC] H027 |
| Links | [LinkedIn](https://www.linkedin.com/in/vansh-garg-81a214324/) · [Site](https://vanshg1729.github.io/) · [GitHub](https://github.com/vanshg1729) · [Scholar](https://scholar.google.com/citations?user=te_Z68kAAAAJ) |
| Sources | H013, H015, H026, H027, H028, H029 |

## Evidence by requirement
| Requirement (ROLE.md v2) | Evidence | Tag |
|---|---|---|
| A Real-robot manipulation | None. Real-robot work is **mobile navigation** (Pioneer P3DX + RealSense) | [V] H028 |
| B Robot learning | **MASt3R-Nav** (ICRA 2026, **first author**): pixel-relative topological maps from MASt3R + a **learned controller (PixelReact)** that predicts waypoints; trained/evaluated in HM3D sim (avg SPL 52.8 vs 33.4 for the best prior object-relative method). **Plann3r** (CoRL 2026, 3rd author): 3D-grounded pixel-level planning costs feeding a learned control policy, with real sim-to-real demos | [V] H028; [CC] H027 |
| C Sim–real–sim | Trained in HM3D simulation → deployed on a real P3DX in an unseen environment (qualitative, 4 locations; no real success rate on the page). PixelLoop "validated through real-world mobile robot deployments" | [V] H028 H029 |
| D Experiments / physics | Nothing | — |
| E RGB-D / 3D perception | **SegMASt3R** (NeurIPS 2025 **Spotlight**, co-first author with Rohit Jayanti and Swayam Agrawal): segment matching under up to 180° viewpoint change using MASt3R 3D priors. Builds on 3D foundation models throughout. RealSense on the robot | [V] H013 H028 |
| F Research & reproducibility | NeurIPS'25 spotlight (co-1st), ICRA'26 (1st), IROS'26 PixelLoop (2nd), CoRL'26 Plann3r (3rd), all within ~2 years; public code (mast3r-nav, pixelloop); CoRL reviewer | [V] H013 H028 H029; [CC] H027 |

Liberal-transfer note [INF]: 3D-foundation-model correspondence (MASt3R) is exactly what's needed to register a toilet/sink across visits, find stains relative to fixtures, and handle viewpoint changes on a mobile manipulator. His perception and learned-controller skills sit next to our problem; manipulation and contact are not.

## Three-axis summary (2026-11-28)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **9/10 (A)** | Edu 4 (IIIT-H CS dual degree with research MS, Top) · Employer 2 (IIIT-H RRC + CVIT) · Signal 3 (NeurIPS spotlight, ICRA first author, CoRL) |
| Can we get them? | **Medium** | In India, still a student [INT Vishal]; record is strong enough for a top PhD abroad [INF] |
| Technical (v2) | **47/100, Tier C** | See score below |
| Contact priority | **P2** | Technical 35–49 + gettability ≥Medium |

## Score (v2): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 1 | Real mobile robot only; no arm |
| B Robot learning & PyTorch | 20% | 3 | Learned navigation controllers deployed on a real robot; not manipulation policies |
| C Sim–real–sim | 20% | 3 | Sim-trained → real P3DX deployment; Plann3r sim-to-real |
| D Experimental optimisation / cleaning physics | 15% | 0 | Nothing |
| E RGB-D perception & calibration | 10% | 4 | Top-venue 3D-foundation-model perception |
| F Research & reproducibility | 10% | 5 | 4 top-venue papers in 2 years incl. NeurIPS spotlight + ICRA first author; public code |
**Total: 47 / 100 → Tier C** · confidence Medium. **Highest-scoring student-researcher outside manipulation**: brilliant 3D-vision + learned-navigation profile. Would score B if he had any arm work. Best fit: perception/spatial-AI side of NORM (registration, change detection, stain localisation), or a manipulation hire who learns fast.

## Availability signals
- Dual degree 2021–2026; still enrolled per Vishal, so graduation is likely 2026–27 [INF].
- Two of his SegMASt3R co-authors have gone abroad; Swayam went to Google DeepMind Bengaluru [INT Vishal 2026-11-28]. He is the one still here.
- Profile (NeurIPS + CoRL + ICRA, reviewer) is PhD-abroad material; approach before applications close [INF].

## Concerns / gaps
- No manipulation, contact or hardware-building beyond running a mobile robot.
- Real-robot results are qualitative on the pages read.

## Outreach notes
- Not contacted. Warm path: RRC (Madhava Krishna); Swayam Agrawal (co-first author, same lab, in Bengaluru).
- Pitch: 3D foundation models on a real mobile manipulator with a product; perception lead for spatial understanding of restrooms.

## Open questions
- Graduation date; PhD plans?
- Interest in manipulation? Has he touched the lab's arms?
- Real-robot success numbers for MASt3R-Nav / PixelLoop (in the papers).
