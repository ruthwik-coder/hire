# Shivansh Pratap Singh

| Field | Value |
|---|---|
| Current role | M.S. by Research student (2nd year) + Research Assistant, Control Lab, **IIIT Hyderabad RRC**, advisor Prof. Spandan Roy (RA since Apr 2024). Research: learned dynamics and latent world models working alongside adaptive controllers, tested on real aerial manipulators [CC] H022 |
| Location / willing to move | Hyderabad [CC] H022 |
| Education | M.S. by Research, ECE (Robotics and Control), IIIT-H, 2024–present, CGPA 9.67/10 · B.Tech Mechanical Engineering, Bundelkhand Institute of Engineering and Technology (BIET), Jhansi, 2019–2023 [CC] H022 |
| Previous | **Robotics Student Fellow, Autonomous Systems Lab (ASL), ETH Zürich**, Jul–Aug 2026: disturbance-aware latent world models for a tethered tilt-rotor omnidirectional aerial robot (domain-randomised sim-to-real, JEPA-style latent dynamics, Jetson inference 3–4 ms → 0.7 ms, better disturbance estimation on unseen real flights) [CC] H022; ETH stint also noted by Vishal [INT Vishal 2026-11-28] · Robotics Engineer, Arka Aerospace, Hyderabad (May 2023 – Mar 2024; AprilTag visual servoing for UAV landing, multi-UAV swarming) [CC] H022 |
| Links | [LinkedIn](https://www.linkedin.com/in/shiva2023/) · [Site](https://aerialmechx.github.io/) · [GitHub](https://github.com/AerialMechX) · [Scholar](https://scholar.google.com/citations?user=wUdlS-EAAAAJ) · CV linked from site (not read) |
| Sources | H019, H021, H022, H023 |

## Evidence by requirement
| Requirement (ROLE.md v2) | Evidence | Tag |
|---|---|---|
| A Real-robot manipulation | **AeroGrab** (IROS'26, **first author**, equal contribution with Naveen Nair): language-guided 6-DoF grasping in clutter on a real quadrotor + 4-DoF Dynamixel arm, **80% collision-free grasps (24/30) in dense clutter**, 41 ms perception-to-plan | [V] H019 |
| B Robot learning & PyTorch | **Whole-body PPO policy** (thrust + body-rate commands) with adaptive INDI inner loop at 250 Hz, **validated on a real 3-DoF aerial manipulator** with 200/400 g payloads, grasp-and-drop (IEEE CASE 2026, first author, arXiv 2606.16621; code public at AerialMechX/RL-adaptive_Aerial_manipulation). AERMANI-Diffusion: diffusion model of residual dynamics, real flights (IFAC 2026, co-first). JEPA-style latent world models (ETH ASL). Paper and code **not yet read by us** | [CC] H022 |
| C Sim–real–sim & sysID | *Learn Structure, Adapt on the Fly* (IROS'26, 3rd author): transformer-learned residual dynamics + online RLS adaptation, real aerial manipulator with unseen payloads. Domain-randomised sim-to-real at ETH ASL | [V] H023 (abstract); [CC] H022 |
| D Experimental optimisation / physics | Residual dynamics learned from real flight data, then adapted online: the same pattern as learning a process-response model from physical trials [INF]. Adaptive/impedance control (ICCAS 2025) | [CC] H022; [INF] |
| E RGB-D perception & calibration | AeroGrab ZED 2i RGB-D grasp perception (CNN-ViT grasp prediction) on a moving platform; AprilTag visual servoing (Arka) | [V] H019; [CC] H022 |
| F Research & reproducibility | 5 papers listed: AeroGrab (IROS'26, 1st), RL + inner-loop estimator (CASE'26, 1st), AERMANI-Diffusion (IFAC'26, co-1st), Learn Structure (IROS'26, 3rd), ICCAS 2025. Public GitHub org with code | [V] H019 H023; [CC] H022 |
| Industry | ~11 months as a robotics engineer at a UAV company before the MS | [CC] H022 |

Liberal-transfer note [INF]: RL policies + learned residual dynamics + online adaptation on a floating-base manipulator carrying unknown payloads is a harder version of the same problem as learning contact/scrubbing dynamics on a fixed arm. Controls depth (INDI, adaptive control) is a real asset for force-controlled cleaning.

## Three-axis summary (2026-11-28)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **9/10 (A)** | Edu 3 (IIIT-H MS by Research, CGPA 9.67; UG BIET Jhansi, Other) · Employer 3 (ETH Zürich ASL fellowship + IIIT-H RRC) · Signal 3 (2× IROS'26 incl. first author, CASE'26 first author, IFAC'26) |
| Can we get them? | **Medium** | In India; 2nd-year MS, likely finishing 2026–27 [INF]. Risk: ETH ASL stint + publication record = strong PhD-abroad candidate |
| Technical (v2) | **75/100, Tier A (provisional)** | See score below |
| Contact priority | **P1** (top of the list) | Technical ≥50 + gettability ≥Medium |

## Score (v2): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 4 | First-author real aerial grasping in clutter (80%) [V]; learned RL policy on a real aerial manipulator [CC]. Not a fixed industrial arm |
| B Robot learning & PyTorch | 20% | 4 | PPO whole-body policy on hardware, diffusion residual dynamics, JEPA world models. **Provisional:** relies on his site + arXiv/code we haven't read; drops to 3 if not confirmed |
| C Sim–real–sim | 20% | 4 | Learned residual dynamics + online adaptation on real hardware [V abstract]; domain-randomised sim-to-real |
| D Experimental optimisation / cleaning physics | 15% | 3 | Learns physical response models from real trials; no cleaning/fluids |
| E RGB-D perception & calibration | 10% | 3 | RGB-D grasp perception; AprilTag servoing |
| F Research & reproducibility | 10% | 4 | 3 first/co-first papers in 2026 + public code |
**Total: 75 / 100 → Tier A (provisional)** · confidence Medium. **First Tier A in the pipeline.** Passes the gate (A 4, C 4, B 4) and has ~3.5 years of hands-on robotics (Arka 2023 → RRC). Confirm B=4 by reading arXiv 2606.16621 and the RL repo.

## Availability signals
- 2nd-year MS by Research (started 2024): thesis completion is the natural exit [INF].
- ETH ASL fellowship in summer 2026 suggests PhD applications abroad (ETH/EU) [INF]. Approach early, before offers land.
- Has already done one industry job (Arka Aerospace), so not purely academic [INF].

## Concerns / gaps
- Everything is aerial; no fixed industrial arm or contact-rich surface task.
- Most learning claims are from his own site; read the CASE paper and repo before the interview.
- Likely PhD-bound.

## Outreach notes
- Not contacted. LinkedIn 2nd-degree. Warm paths: **Prof. Spandan Roy** (also co-authored a cleaning-robot control paper with SUTD, see SEARCH_LOG); Sarthak Mishra (same group, reposted his post) [V] H021.
- Pitch: world models + adaptive control on a real fixed-arm product doing contact-rich cleaning; a founding research role vs a PhD.

## Open questions
- Plans after MS (PhD abroad? timing)?
- CASE paper: did the PPO policy transfer zero-shot to hardware, and how robust was it?
- Interest in fixed-arm manipulation / contact-rich tasks?
