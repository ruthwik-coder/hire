# Aayush Rath

Competitor-KB view (his Nolon work): [../competitors/nolon/nolon.md](../competitors/nolon/nolon.md#people-directory). Nolon robot sim stack: see "Robot: Nolon Bot" in that file.

| Field | Value |
|---|---|
| Current role | Research Assistant / research intern, Robotics Research Center (RRC), IIIT Hyderabad, under Prof. Antony Thomas; motion planning (since Aug/Sep 2025: the site says Aug, LinkedIn says Sep) [CC] H004 H006 |
| Location / willing to move | Hyderabad, India [CC] H004 · moving to Bengaluru is probably easy [INF] |
| Education | B.Tech, Dept. of Ocean Engineering, IIT Madras, 2024. The CV says "Naval Architecture"; CGPA 7.16/10 [CC] H005. Coursework includes Intro to Robotics, Motion Planning, Guidance of Autonomous Vehicles, Multi-Body Dynamics [CC] H005 |
| Previous | Robotics Intern, Nolon.AI (Jul–Sep 2025; on his site but **not on LinkedIn**) · Robotics Engineer, Swaayatt Robots, Bhopal (Aug 2024 – Jul 2025; autonomous-driving perception/SLAM) · Research intern, LBMC Lyon (gait biomechanics, 2023) · Raftar Formula Racing, IITM (2021–24; Chassis Lead with about 20 people) [CC] H004 H005 H006 |
| Links | [LinkedIn](https://www.linkedin.com/in/aayush-rath-008584201/) · [GitHub](https://github.com/aayush-rath) · [Site](https://aayush-rath.github.io/) |
| Sources | H004, H005, H006 · competitor KB S132 (sim-stack repo, code read), S133 |

## Evidence by requirement
| Requirement (ROLE.md) | Evidence | Tag |
|---|---|---|
| 1. Robot software architecture | Nolon sim stack: ROS 2 Jazzy, ros2_control, Nav2 (Smac + RPP), slam_toolbox, MoveIt 2 (OMPL, Servo), Docker, Isaac Sim USD export. Single author, 12 commits in 1 week. It is a **scaffold**: no perception, no task planner, no real-hardware drivers | [V] S132 |
| 2. 6-axis manipulation | xArm6 + MoveIt 2 **in sim only**. His RRC work is complete motion planning for n-R planar manipulators and infeasibility detection (theory) | [V] S132; [CC] H006 |
| 3. Mobile navigation / SLAM | Swaayatt: LiDAR clustering (Euclidean/DBSCAN), IMM/UKF/PHD tracking filters to give a stable occupancy grid, LiDAR + image meshed maps, point-to-plane ICP + g2o localisation. Real AV programme. Nav2 + slam_toolbox in sim. B.Tech project: PRM + PID on a scale-model boat with a Raspberry Pi | [CC] H005; [V] S132 |
| 4. ML from scratch | **Thin.** Claims: a GAN + NeRF data-augmentation pipeline at Swaayatt ("500% faster") H005; a small CNN predicting suspension load from shock deflection, plus an NN checking aero CFD (Formula Student) H005; a Coursera DL course. GitHub: Hopfield net in C++, a fork of PointTransformerV3 (his changes not visible), QuotientFlow3D ("differentiable ray-tracing for 3D generative modelling"), SegFuser (no description, Nov 2026). **No RL, imitation learning, diffusion policy, VLA, PyTorch or Isaac Lab mentioned anywhere** | [CC] H005 H006; repos not opened |
| 5. Simulation & sim-to-real | Built the Gazebo sim of a mobile manipulator with Isaac Sim export. Wrote his own simulators (MMG ship sim, lap-time sim). **PaGeRo**: his own CUDA geometry engine for collision and distance queries in robot sims. No sim-to-real transfer shown | [V] S132; [CC] H006 |
| 6. Hardware literacy | Formula Student EV (PWM fan control, shock potentiometers, servo-driven DRS, battery thermal); Raspberry Pi boat; motion-capture labs (Vicon/Qualisys). Mostly mechanical and vehicle-side; no CAN/EtherCAT/robot-arm drivers seen | [CC] H005 |
| Research | "Towards Kinematic Actionable Infeasibility Detection in Motion Planning", Rath, Jindal, Thomas, listed as **IEEE RA-L 2026**. A second arXiv paper on complete planning for nR-planar manipulators. Both site entries point to the same arXiv ID (2608.01172), so this is **not verified** | [CC] H006 |
| Domain | Has already worked on a toilet-cleaning robot (Nolon). Knows our problem | [V] S132 |

## Three-axis summary (2026-11-27)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **7/10 (B)** | Edu 3 (IIT Madras UG) · Employer 2 (Swaayatt; IIIT-H RRC research) · Signal 2 (RA-L 2026 first author, unverified) |
| Can we get them? | **High** | In India; research-intern contract; risk: PhD abroad |
| Technical (v2) | **38/100, Tier C** | See score below |
| Contact priority | **P2** | ROLE.md rule |

## Score (v2 rubric, 2026-11-24): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 2 | xArm6 + MoveIt 2 in sim; strong manipulator motion-planning theory; no real arm |
| B Robot learning & PyTorch | 20% | 1 | No IL/RL; ML evidence thin and [CC] |
| C Sim–real–sim | 20% | 2 | Built custom sim envs + Isaac export + his own CUDA collision engine; no transfer |
| D Experimental optimisation / cleaning physics | 15% | 2 | Ocean/naval engineering: CFD (Ansys Fluent), iterative CFD optimisation, physical test rigs. The closest fluids background so far |
| E RGB-D perception & calibration | 10% | 2 | LiDAR clustering, ICP, LiDAR+image meshing (AV) |
| F Research & reproducibility | 10% | 3 | RA-L 2026 first author (unverified) + arXiv |
**Total: 38 / 100 → Tier C** (was B under v1) · confidence Medium. A classical planning/sim builder; the v2 role centres on robot learning, which is his gap.

## Score v1 (superseded: old Head-of-stack brief)
| Criterion | 0–3 | Why |
|---|---|---|
| 1 Robot software stack | 2 | Built a full ROS 2 mobile-manipulator stack (in sim) fast; AV perception modules at Swaayatt |
| 2 6-axis manipulation | 1 | Sim only (xArm6 + MoveIt 2); strong planning theory |
| 3 Navigation / SLAM | 2 | Real AV perception/SLAM at Swaayatt; Nav2 in sim |
| 4 ML from scratch | 1 | Applies models; small own networks; GAN/NeRF claim unverified. **Main gap** |
| 5 Simulation & sim-to-real | 2 | Sim pipelines and his own CUDA sim engine; no transfer to a real robot |
| 6 Hardware literacy | 2 | Vehicle hardware, sensors, PWM, RPi; not robot-arm/industrial buses |
| 7 Shipped / field | 1 | Competitions, R&D vehicle, sim |
| 8 Ownership / leadership | 2 | Chassis Lead (20 people); built Nolon's stack alone |
| 9 Pedigree & signal | 2 | IIT Madras (CGPA 7.16); RA-L first author (to verify); CUDA/geometry depth |
| 10 Fit & availability | 3 | In India; on a research-intern contract; already chose toilet cleaning once [INF] |
**Total:** 18 / 30 → **Tier B** (strong builder, good #2 / founding robotics engineer). **Not Tier A:** fails the A gate on criteria 2 (manipulation) and 4 (ML), and is about 2 years out of his B.Tech.

## Availability signals
- RRC role is a research internship/assistantship, usually 1–2 years, often a step toward an MS/PhD abroad [INF]. **Risk:** he may be heading to a PhD rather than a job.
- Left Swaayatt after 1 year and Nolon after 3 months. The Nolon exit makes sense since Nolon went dormant [INF].

## Concerns / gaps
- **AI/ML depth is the main gap**, as Vishal suspected. His strength is classical robotics: estimation filters, ICP/graph SLAM, sampling and complete motion planning, computational geometry, CUDA. That is a valuable profile, but it is not "builds ML models from scratch".
- The Nolon sim stack is good fast work, but it is a standard open-source scaffold with off-the-shelf models. Don't overrate "built a competitor's stack".
- The degree is ocean/naval engineering, not CS/EE. He moved into robotics through projects.
- Self-reported numbers ("500% faster", "RMSE 3%") have no verification.

## Outreach notes
- Not contacted. Warm path: through the Nolon people (Vijeth Rai, Raushan Kumar), or IIT Madras alumni.
- **Competitor hygiene:** talk only about his public work. Don't ask for Nolon internal material (CLAUDE.md rule).

## Open questions / how to test the AI gap
1. Read SegFuser, QuotientFlow3D and the PTv3 fork. Do they contain real training code (PyTorch, own training loops, results)? This is the cheapest check.
2. Ask him to walk through the Swaayatt GAN/NeRF pipeline: architecture, data, loss, failure cases. This separates "used it" from "built it".
3. Paid take-home (2–3 days): train a segmentation model for stains/wet patches on restroom tiles using synthetic Isaac Sim data, then evaluate on 30 real photos. This tests ML, sim-to-real and our real problem together.
4. Plans: PhD abroad, or industry? Timeline?
5. Verify the RA-L paper on arXiv/IEEE (both site links point to the same ID). **2026-11-27:** the paper is *not* on IIIT-H RRC's own publications list for 2023–26 (H015). The lab page may lag, or the paper may still be under review.
