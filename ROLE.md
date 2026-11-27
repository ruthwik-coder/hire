# Role v2: Robotics AI Research Engineer (Robot Learning, Manipulation & Sim-to-Real)

**Brief:** Vishal, 2026-11-24. It replaces v1 "Head of Robot Software, AI & Simulation" (archived in [ROLE_v1_2026-11-21.md](ROLE_v1_2026-11-21.md)).

**Company:** Ubanthu Robotics, NORM 100. FANUC CRX-5iA 6-axis arm on a 2WD base; Jetson Orin NX; Orbbec RGB-D; 2D LiDAR; steam/water/chemistry cleaning tools. Bengaluru (IISc incubation).

## Mission
Build NORM's **cleaning intelligence**. **NORM must learn how to clean, not just how to move an arm.** The person owns this loop:

**perception → cleaning decision → manipulation → measuring the cleaning outcome → learning**

The model observes contamination and toilet geometry. It chooses a target, tool, nozzle pose, angle, standoff, pressure/flow (within safe limits), duration and sweep path. It executes, verifies the result, decides whether to clean again or stop, and improves through repeated physical trials. Independent safety controls stay separate from the learning loop.

It is an optimisation problem: choose a* = argmax_a E[Q_clean(a) | x], subject to limits on water, time, temperature, pressure, splash and safety. In-house IP = the cleaning-action dataset + the learned cleaning-response model + the adaptive policy + the real-world feedback loop.

## Profile
- **Mid–senior, 3–6+ years of hands-on robotics.** This is a recommendation, not a hard rule. **Demonstrated real-robot results matter more than the degree.**
- Has **trained learning-based manipulation policies and deployed them on physical arms**, built simulation environments, and iterated using real sensor data and experiment results.
- Preferred domains: contact-rich manipulation, surface treatment / robotic spraying / cleaning, autonomous inspection, industrial robotics, embodied-AI research.
- Strongest in **robot learning, real-robot integration and experimental validation**. Works with a mechanical/fluids engineer on cleaning physics.
- **Understands simulator limits.** Physics sims don't reproduce stain adhesion, biofilm removal, spray interaction or disinfection. They should use a **hybrid approach**: experimentally measured outcomes train a surrogate model or reward estimator. They also know that a stain disappearing visually is not proof of microbiological cleanliness.

## Skills
| Domain | Examples | Importance |
|---|---|---|
| Robot learning | Imitation learning, RL, behaviour cloning, policy evaluation; LeRobot, ACT, diffusion policy, DAgger, PPO/SAC | Critical |
| Physical robotics | 6/7-axis arms, IK, frames, calibration, motion execution; ROS 2, MoveIt 2, TF2, vendor SDKs; turning AI actions into safe executable motion | Critical |
| Sim → real → sim | Isaac Sim/Lab, USD, PhysX, URDF; domain randomisation, system identification, real-to-sim calibration | Critical |
| Computer vision | RGB-D, point clouds, segmentation, surface normals, 3D reconstruction; OpenCV, Open3D | Critical |
| ML engineering | PyTorch, dataset pipelines, training, fine-tuning, evaluation | Critical |
| Task optimisation | Learning action parameters, experiment design (DoE), Bayesian optimisation / active learning, contextual bandits / offline RL, MPC, multi-objective trade-offs | Critical |
| Fluid & cleaning physics | Jet impingement, spray coverage, surface interaction, contamination removal, thermal effects | High |
| Deployment | Low-latency edge-GPU inference (Jetson), monitoring | High |
| Research methods | Reads and implements papers; runs controlled experiments | High |
| VLA / foundation models | Fine-tuning pretrained VLAs on a real robot | Desirable |
| MLOps | W&B/MLflow, versioning, reproducible and distributed training | Desirable |

## Résumé signals
| Background | Value |
|---|---|
| Trained policies and deployed them on real manipulators | Excellent |
| Custom Isaac Lab environments with sim-to-real transfer | Excellent |
| Diffusion policy / imitation learning for manipulation | Excellent |
| Industrial surface processing, robotic spraying or cleaning | Excellent |
| RGB-D perception + closed-loop manipulation | Very high |
| VLA with real-robot fine-tuning | High |
| Simulation only, never deployed on a robot | Useful, not enough alone |
| Image classification / object detection only | Not enough alone |
| LLMs / agents / chatbots / RAG only | Low → usually Tier X |

## Scorecard (v2): six weighted criteria, each 0–5 → total /100
This is the founders' interview scorecard. **At screening** I score it from public evidence as a *pre-interview estimate*. **At interview** the founders re-score the same rubric, so the two numbers can be compared directly.

Score = Σ (criterion score / 5 × weight).

| # | Criterion | Weight | 0 | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|---|---|---|
| A | **Real-robot manipulation & controls** | 25% | none | coursework / sim only | MoveIt/IK in sim, or a hobby-grade real arm | real industrial 6/7-axis arm in a lab: calibration, frames, motion execution | **learned policies executed on a real arm**, or contact-rich real tasks | deployed / field manipulation; contact-rich or surface-treatment product |
| B | **Robot learning & PyTorch** | 20% | none | uses pretrained models / tutorials | trains own DL models (not robot policies), or RL on a toy sim task | trains IL/RL manipulation policies in sim with sound design | **policies trained and validated on a real robot** | novel robot-learning methods (publications / widely used OSS) plus real results |
| C | **Sim–real–sim & system ID** | 20% | none | uses simulators | builds custom sim envs / digital twins / synthetic data | trained in randomised sim and **transferred to a real robot** | **closed the loop**: calibrated the sim from real data (sysID) and retrained | repeated sim→real→sim at product scale |
| D | **Experimental optimisation & cleaning physics** | 15% | none | engineering fundamentals (coursework, FEA) | controlled experiments, or fluids/CFD work | systematic parameter optimisation of a physical process (DoE, Bayesian optimisation) | learned process-response / surrogate models from physical trials | robotic spraying/cleaning/surface-treatment expertise |
| E | **RGB-D perception & sensor calibration** | 10% | none | basic 2D vision | point-cloud / LiDAR / RGB-D processing | built 3D reconstruction or calibration (extrinsics, hand-eye) | RGB-D perception closing a manipulation loop on a real robot | novel 3D perception, deployed |
| F | **Research implementation & reproducibility** | 10% | none | follows tutorials | implements from papers; tracked, clean experiments | first-author paper or merged OSS | top-venue robot-learning papers with released code | recognised research leader |

### Tiers
- **A: shortlist for founders.** ≥ 70 **and** the gate: A ≥ 3, C ≥ 3, and **B ≥ 4** (has put a learned policy on a real robot).
- **B: strong.** 50–69, or ≥ 70 but failing the gate.
- **C: watch / junior / later.** < 50, or less than 3 years of hands-on robotics (maximum tier for juniors is B, unless they have exceptional real-robot results).
- **X: not a fit.** LLM/RAG-only or detection-only profiles, or < 25 with no learning/robotics path.

### Rules
- **Evidence beats claims.** A score of 4 or 5 on A, B or C needs `[V]` evidence (video, code, paper). With `[CC]` only, cap the score at 3 and say so.
- **Availability and seniority are not in the score.** Track them in the CANDIDATES.md columns.
- Record a **confidence** for each total: High (mostly [V]) · Medium · Low (mostly [CC]).

## Three-axis view (added 2026-11-27, Vishal)
Every candidate gets **three separate scores**. They are not merged into one number:

| Axis | Question | Scale |
|---|---|---|
| **1. Reputation** | How strong is their institutional and employer pedigree? | 0–10 → grade A/B/C/D |
| **2. Can we get them?** | How realistic is it to hire them now? | High / Medium / Low / Very low |
| **3. Technical** | Can they build NORM's cleaning intelligence? | v2 scorecard /100 (above) → Tier A/B/C/X |

### 1. Reputation (0–10) = Education (0–4) + Employer/lab (0–3) + Signal (0–3)
**Institution classes:**
- **Top:** IISc; IITs (Bombay, Delhi, Madras, Kanpur, Kharagpur, Roorkee, Guwahati, Hyderabad); IIIT Hyderabad; top-50 global (CMU, ETH, Stanford, MIT, Berkeley, Oxford, TUM, etc.)
- **Strong:** other IITs/IIITs, BITS, top NITs (Trichy, Surathkal, Warangal, Calicut), DTU/NSUT, good foreign universities (e.g. UZH)
- **Other:** less-known colleges

| Points | Education (best degree; counts if in progress) | Employer / lab (best) | Signal |
|---|---|---|---|
| 4 | PhD / MS / MTech(R) at a **Top** institution | — | — |
| 3 | UG at a Top institution, or PG at a Strong institution | **Google DeepMind / Google Research / NVIDIA / Meta FAIR / OpenAI**, top robotics companies (Boston Dynamics, Figure, Physical Intelligence, Agility, Covariant…), or a research role in a world-top lab (CMU RI, ETH, Stanford…) | Several first-author papers at top venues (NeurIPS/ICML/ICLR/CVPR/ICCV/ECCV/CoRL/RSS) |
| 2 | UG at a Strong institution | Respected robotics/AI company or startup (Origin, CynLr, Addverb, Swaayatt…), or a research position in an IISc/IIT/IIIT-H lab | One top-venue paper, or RA-L/ICRA/IROS first author |
| 1 | UG/PG at an Other institution | Internships, college labs, general software jobs | Competition wins, GSoC, journal papers |
| 0 | — | none | none |

**Grade:** A 8–10 · B 6–7 · C 4–5 · D 0–3. Reputation shows **potential and signal**; it does **not** override the technical score.

### 2. Can we get them?
Factors: location (Bengaluru/India vs abroad) · current commitment (just joined a job, mid-degree, PhD-bound) · pay gap (big tech or a Swiss/US salary) · timing (graduation date) · pull of our mission (real-robot cleaning, IISc ecosystem).
- **High:** in India, between roles or near the end of a contract/degree, startup-minded.
- **Medium:** gettable with timing (graduating within about 12 months) or a moderate pull.
- **Low:** settled abroad, or recently joined a good job.
- **Very low:** big-tech research or PhD-bound, with a large pay or career gap.

### Contact priority (from axes 2 + 3)
- **P1:** Technical ≥ 50 **and** gettability ≥ Medium → reach out now
- **P2:** Technical 35–49 and gettability ≥ Medium (intern/junior track), or Technical ≥ 50 with Low gettability
- **P3:** everything else → watch
- Reputation breaks ties within a priority band.

## Interview assignment (shortlist)
> A six-axis arm with a spray nozzle, an RGB-D camera and a dirty curved ceramic surface. Design a learning system that finds the contamination, selects a cleaning trajectory and spray parameters, executes safely, measures the result and improves over repeated trials.

- **Strong answers** cover sensor calibration, surface normals, uncertainty, where the training data and **ground-truth cleaning signal** come from, action constraints, simulation limits, evaluation, and cleaning-outcome metrics.
- **Weak answers** jump straight to "train a big VLA / RL agent" without saying where the reward or labels come from.

## First 90 days (suggested, not promised)
| Days | Deliverable |
|---|---|
| 1–30 | Integrate arm, camera and tools; data-recording pipeline; define contamination and cleaning metrics |
| 31–60 | Baseline cleaning policy; physical cleaning trials; first cleaning-response model |
| 61–90 | Train and compare learned policies; real→sim feedback; show improvement over the baseline |

## Where to look (updated for v2)
- **Robot-learning people with real arms:** LeRobot / ACT / diffusion-policy contributors; Isaac Lab contributors; CoRL / RSS / ICRA manipulation authors (Indian or India-willing).
- **Indian labs:** IISc (CPS/RBCCPS, CSA), IIT Madras, IIT Bombay, IIT Delhi, IIT Kanpur, IIIT Hyderabad RRC; ARTPARK.
- **Companies:** CynLr (vision-guided manipulation), Addverb, Sastra Robotics, Origin, Genrobotics; robotic painting/spraying/finishing integrators (FANUC/ABB paint, surface-finishing startups); Covariant, Dexterity, PickNik, NVIDIA Isaac, Physical Intelligence, Figure, Wandelbots.
- **Abroad (Indians willing to return):** CMU RI, Stanford IRIS/SVL, Berkeley, ETH RSL/CRL, TUM, GaTech, UMich, UPenn GRASP.
