# Sarthak Mishra

| Field | Value |
|---|---|
| Current role | MS (CS, specialization Robotics) student, **IIIT Hyderabad RRC** (from Jan 2024) and Research Associate, RRC (since Jul 2023): "closed-loop control systems for various types of motors" [CC] H018. Group: Spandan Roy's aerial-manipulation lab [V] H019 |
| Location / willing to move | Hyderabad [CC] H018 |
| Education | MS CS (Robotics), IIIT-H, started Jan 2024 (end date not visible) · B.Tech Integrated Computer Engineering, NMIMS Mukesh Patel School of Technology Management & Engineering (2017–2023) [CC] H018 |
| Previous | Research Intern, AIIMS New Delhi (2021–2024; control systems and AI tools for robotic medical procedures) · **Team Captain, Team Darvin** (IGVC, 2021–23; responsible for software + electronics) · Team Leader, e-Yantra Robotics Competition (2020–21; semi-finals; drone delivery control in sim) · Core member, MRT (Baja racing team; data acquisition and electronics), 2019–20 [CC] H018 |
| Links | [LinkedIn](https://www.linkedin.com/in/sarthak-mishra-8053181b5) · no GitHub/site listed |
| Sources | H015, H018, H019 |

## Evidence by requirement
| Requirement (ROLE.md v2) | Evidence | Tag |
|---|---|---|
| A Real-robot manipulation | **AeroGrab** (IROS 2026, 4th author of 7): quadrotor + **4-DoF Dynamixel arm**, language-guided 6-DoF grasping in clutter. **Hardware: 80% collision-free grasps (24/30) in dense clutter**; window and shelf scenarios 73% and 70% (N=30 each). **AeroPlace-Flow** (IROS'26): language-grounded placement, 75% real success | [V] H019; [3P] H015 |
| B Robot learning | AeroGrab: learned hybrid CNN-ViT grasp-synthesis network + VLM target grounding executed on the real platform. AeroPlace-Flow (object flow), AERMANI-VLM (VLM reasoning for aerial manipulation). His own share of model training is **not visible** | [V] H019; [3P] H015 |
| C Sim–real–sim | AeroGrab: quadrotor dynamics simulated "prior to hardware deployment", then hardware trials | [V] H019 |
| D Controls / experiments | Closed-loop motor control (RA role); systematic N=30 hardware trials with ablations | [CC] H018; [V] H019 |
| E RGB-D perception | ZED 2i stereo RGB-D, semantic tracking under ego-motion, depth-checked grasp selection | [V] H019 (team paper) |
| Systems / hardware | ROS 2 Humble, PX4 via DDS, Jetson Orin Nano onboard, Dynamixel arm; IGVC captain (software + electronics) | [V] H019; [CC] H018 |
| F Research | 3 IIIT-H aerial-manipulation papers at IROS'26 (AeroGrab, AeroPlace-Flow, AERMANI-VLM). First-author status on AeroPlace-Flow / AERMANI-VLM **to verify** | [V] H019; [3P] H015 |

Liberal-transfer note [INF]: contact-aware grasping from a moving, vibrating drone with a light arm is harder on perception/control than a fixed arm; the skills (RGB-D grasp selection, ROS 2 + real-time control, hardware trial discipline) carry over directly to a fixed 6-axis arm.

## Three-axis summary (2026-11-28)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **7/10 (B)** | Edu 3 (IIIT-H MS, Top PG; UG NMIMS, Other) · Employer 2 (IIIT-H RRC research, 3+ years) · Signal 2 (3× IROS'26; IGVC captain) |
| Can we get them? | **Medium–High** | Hyderabad; MS since Jan 2024, so likely finishing 2026–27 [INF]; risk: PhD abroad |
| Technical (v2) | **57/100, Tier B** | See score below |
| Contact priority | **P1** | Technical ≥50 + gettability ≥Medium |

## Score (v2): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 3 | Real aerial manipulator grasping/placing with measured success rates; light 4-DoF arm, not an industrial 6/7-axis |
| B Robot learning & PyTorch | 20% | 3 | Learned grasp nets + VLM grounding run on hardware; his training role unclear, so not 4 yet |
| C Sim–real–sim | 20% | 3 | Sim-first then hardware; no explicit transfer study |
| D Experimental optimisation / cleaning physics | 15% | 2 | Controls background, disciplined hardware trials; no process optimisation |
| E RGB-D perception & calibration | 10% | 3 | RGB-D grasp perception on a moving platform |
| F Research & reproducibility | 10% | 3 | 3 IROS'26 papers; no public code seen |
**Total: 57 / 100 → Tier B** · confidence Medium. Fails the A gate on B (needs a policy he trained himself on a real robot). **First P1 in the pipeline.**

## Availability signals
- 3.4 years at RRC (RA since Jul 2023, MS since Jan 2024): a natural exit point is MS completion [INF].
- Captain/leader roles in every team listed: comfortable owning a system end to end [INF].

## Concerns / gaps
- Mostly drones; no fixed industrial arm shown.
- AeroGrab is a 7-author team paper where he is 4th author; his own modules are not identifiable.
- LinkedIn is thin on the research itself (only "closed-loop motor control").

## Outreach notes
- Not contacted. Warm paths: **Prof. Spandan Roy** (his PI; also co-authored a cleaning-robot control paper with SUTD, see SEARCH_LOG) or IIIT-H RRC network (Aayush Rath is also at RRC).
- Pitch angle: same perception→grasp→execute loop, on a fixed arm doing contact-rich cleaning, with a real product.

## Open questions
- Which modules did he build in AeroGrab / AeroPlace-Flow / AERMANI-VLM? Did he train the grasp or flow model?
- Is he first author on AeroPlace-Flow and AERMANI-VLM? Code public?
- MS thesis topic and expected completion; PhD plans?
