# Shaurya Kishore Panwar

| Field | Value |
|---|---|
| Current role | Software Engineer, Diaxxo AG, Zurich (since Apr 2026) [CC] H002 |
| Location / willing to move | Zurich, Switzerland [CC] H002 · willingness to move to India **unknown** |
| Education | M.S. Artificial Intelligence, University of Zurich (Sep 2024 – Oct 2026), plus ETH Zürich "Special Student" over the same dates (this is not an ETH degree) [CC] H001 H002 · B.Tech Engineering Physics, minor in CS, Delhi Technological University (2020–2024); bachelor's thesis on aerial VLN, supervised by Prof. Anil S. Parihar [CC] H001 H002 · IIT Madras online Diploma in Programming & Data Science (2021–22) [CC] H002 |
| Previous | Software Lead, MONKEE (ETH Robotics Club, bimanual tree-climbing robot), Nov 2025 – Aug 2026 · GSoC 2025 contributor at OpenCV ("SLAM system from scratch") · Visiting Researcher, BFH Biel (GPS-free drone navigation, ThinkSwiss scholarship), Jun–Aug 2023 · Autonomous Lead / Senior Autonomous Systems Architect, Team Defianz (DTU driverless Formula Student), Jan 2021 – Jun 2023 · Autonomous Driving Intern, Euler Motors, Jul–Aug 2022 [CC] H002 |
| Links | [LinkedIn](https://www.linkedin.com/in/shaurya-k-panwar) · personal site (URL not captured) · [LangLoc project](https://rzninvo.github.io/Lang-Loc/) · [BFH drone video](https://www.youtube.com/watch?v=EyqHZkrB38Q) |
| Sources | H001, H002, H003 |

## Evidence by requirement
| Requirement (ROLE.md) | Evidence | Tag |
|---|---|---|
| 1. Robot software architecture | Led the autonomy stack for India's first driverless Formula Student team: FS Italy 2022, 8th overall (H002). Euler Motors: built an autonomous delivery-vehicle stack on Autoware (H002). Made the BFH drone code production-ready on a Jetson Nano (H002). MONKEE software lead (H002). No ROS 2 repo seen yet. | [CC] |
| 2. 6-axis manipulation | Only MONKEE, a bimanual climbing robot. Arm type, DoF and his own manipulation work are **not visible**. | [CC] / gap |
| 3. Mobile navigation / SLAM | Driverless car autonomy (real vehicle, competition); Euler mapping, planning and dynamic-obstacle avoidance; "SLAM from scratch" for OpenCV under GSoC; vision-only drone navigation. Research is in VLN and language-based localisation. | [CC]; LangLoc [V] H003 |
| 4. ML from scratch | First author (equal contribution) of LangLoc, accepted at ECCV 2026: GATv2 + CLIP scene retrieval, ray-cast pose scoring, Bayesian dialog module, and a new 13k-description benchmark. Co-authors are Pollefeys and Barath (ETH). Also redesigned a UNetFormer segmentation decoder (BFH) and wrote an ICICCT 2024 aerial-VLN paper. | [V] H003; [CC] H001 H002 |
| 5. Simulation & sim-to-real | Nothing explicit. VLN work usually runs in simulators, but none is named. | gap |
| 6. Hardware literacy | Chose and integrated sensors on the drone (cameras, altimeter, IMU); LiDAR–camera fusion at Euler; Jetson Nano deployment. | [CC] H002 |
| Nice-to-have: field / shipped | Competition vehicle plus short internships only. | [CC] |
| Nice-to-have: leadership | Team Manager and Autonomous Lead of Defianz for 3 years (H001); MONKEE software lead. | [CC] |

## Three-axis summary (2026-11-27)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **7/10 (B)** | Edu 3 (MS UZH, Strong-foreign PG; ETH special student) · Employer 2 (research with ETH CVG) · Signal 2 (ECCV'26 first author; GSoC) |
| Can we get them? | **Low** | Zurich; 8 months into a Swiss job; Swiss pay gap |
| Technical (v2) | **32/100, Tier C** | See score below |
| Contact priority | **P3** | ROLE.md rule |

## Score (v2 rubric, 2026-11-24): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 1 | No arm work shown. MONKEE (bimanual climbing robot) role unclear |
| B Robot learning & PyTorch | 20% | 2 | Strong DL (ECCV), but VLN/localisation, not manipulation policies |
| C Sim–real–sim | 20% | 1 | None shown |
| D Experimental optimisation / cleaning physics | 15% | 1 | Engineering physics fundamentals only |
| E RGB-D perception & calibration | 10% | 3 | LiDAR–camera fusion, SLAM from scratch, 3D-scan localisation |
| F Research & reproducibility | 10% | 3 | ECCV first author; code "will be released" |
**Total: 32 / 100 → Tier C** · confidence Medium. Strong 3D-vision researcher, but not a robot-learning/manipulation profile.

## Score v1 (superseded: old Head-of-stack brief)
| Criterion | 0–3 | Why |
|---|---|---|
| 1 Robot software stack | 2 | Led the FS driverless autonomy stack; Autoware stack; Jetson deployment |
| 2 6-axis manipulation | 1 | Only MONKEE (bimanual), with no detail. Provisional |
| 3 Navigation / SLAM | 2 | Real vehicle and drone, plus SLAM from scratch. All lab or competition, no product |
| 4 ML from scratch | 2 | Designs his own models; ECCV first author. Early-career, so not yet a 3 |
| 5 Simulation & sim-to-real | 1 | No evidence. Assumed basic [INF] |
| 6 Hardware literacy | 2 | Sensor selection and integration, fusion, Jetson |
| 7 Shipped / field | 1 | Competitions and demos |
| 8 Ownership / leadership | 2 | Led the student team's autonomy for 3 years; MONKEE software lead |
| 9 Pedigree & signal | 2 | ECCV with the ETH CVG group, GSoC/OpenCV, UZH/ETH. DTU is not top-tier for our bar |
| 10 Fit & availability | 1 | In Zurich and 8 months into a Swiss job; relocation unlikely [INT Vishal 2026-11-22] [INF] |
**Total:** 16 / 30 → **Tier C** for the head role (scores at the B threshold, but he is too junior to lead and relocation looks unlikely). Could be a strong **B-level #2 hire** for perception, navigation and SLAM if he is open to India.

## Availability signals
- M.S. due to finish Oct 2026 [CC] H002. He started full-time at Diaxxo AG in Apr 2026, so he has already moved into Swiss industry.
- German at A2–B1 and still learning (H001) [INF]: suggests he plans to stay in Switzerland.
- Against that: Indian national, Delhi background, early career, and his site motto "Mens et Manus" suggests he likes hands-on building [INF]. A robotics head role at a startup is a step up from a general software-engineer job [INF].
- Diaxxo AG: what the company does and how robotics-related his role is are not checked.

## Concerns / gaps
- **Seniority:** about 2.5 years since his B.Tech, so he is not a stack lead yet [INF].
- No real 6-axis arm work, no sim-to-real, no shipped product.
- His research has moved toward vision-language (VLN, language localisation) and away from control and manipulation.
- The LinkedIn headline says "ETH Zurich", but his degree is from UZH. ETH is special-student status plus the research collaboration.
- LinkedIn "Top Skills" lists web development, which doesn't match the profile. Probably stale [INF].

## Outreach notes
- Not contacted. No warm path known. Possible routes: DTU alumni, or anyone we know at ETH Robotics Club or CVG.
- Low-cost pitch: lead perception and navigation on a real mobile manipulator, plus Bengaluru/IISc. Ask about relocation openly in the first message.

## Open questions
- Would he move to Bengaluru, and on what timeline?
- What does he do at Diaxxo AG?
- What was his own work on MONKEE (arm control? planning? which hardware?) What came out of the GSoC SLAM work (merged PR, repo)?
- GitHub: does he have ROS / ROS 2 code? (Not yet looked up.)
