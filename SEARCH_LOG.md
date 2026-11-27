# Search log

What has been searched, when, and what came out. Check here before searching again.

| Date | Where / query | Result | Next |
|---|---|---|---|
| 2026-11-21 | Competitor KB people (Nolon, Origin, Hivebotics, Primech, Peppermint) | 6 people seeded into CANDIDATES.md (Nolon + Origin) | Build full profiles for Vijeth Rai, Saketh Vaishya, Aayush Rath |
| 2026-11-22 | Inbound: Shaurya Panwar (site + LinkedIn + ECCV paper, from Vishal) | Profiled, Tier C | Check GitHub (ROS 2 / GSoC SLAM); ask about relocation |
| 2026-11-23 | Aayush Rath: LinkedIn + CV (Vishal); GitHub repo list + site (Claude) | Profiled, Tier B; ML thin on public record | Open SegFuser / QuotientFlow3D / PTv3-fork code; verify RA-L paper |
| 2026-11-24 | Inbound: Chalus Jude J (LinkedIn post + profile, from Vishal) | Profiled, Tier C (intern track) | Read portfolio + MuJoCo clip; check ARTPARK / Automind Dynamics for more people |
| 2026-11-24 | — | Seed rows from the competitor KB removed from CANDIDATES.md (list = provided material only). Saketh Vaishya and Vijeth Rai look like possible v2 fits if re-added later | Re-add only when material is provided |
| 2026-11-26 | IISc HiRo Lab (CPS, Dr. Ravi Prakash): people/research/publications pages | Akhil R Kurup profiled (C, low confidence). Lab = robot manipulation + imitation learning on 5× Franka FR3 + AgileX arms. Leads below | Get material on the leads; consider a lab-level relationship (IISc incubation) |
| 2026-11-27 | IIIT-H Robotics Research Center publications 2024–26 (list pasted by Vishal; 10 project pages / abstracts checked by Claude) | ~14 people worth researching; ranked lead list below. Swayam Agrawal's papers confirmed; Aayush Rath's RA-L paper not on the RRC list | Vishal to research the top leads; send their material to process |
| 2026-11-28 | Vishal picked 2 RRC leads + sent Swapnil Joshi (IISc HiRo) | Md Faizal Karim (70, P1), Sarthak Mishra (57, P1), Swapnil Joshi (19, P3). New names from papers: Vignesh Vembar (DAGDiff co-first author), Keshab Patra, Shivansh Pratap Singh + Naveen Nair (AeroGrab co-first authors) | Get Faizal's LinkedIn/CV; check co-first authors |
| 2026-11-28 | Shivansh Pratap Singh LinkedIn post + his site (aerialmechx.github.io) + arXiv 2603.11638 | Shivansh: 75, first Tier A (P1). Faizal parked and Rishabh dropped (both abroad, Vishal). Remaining AeroGrab-group leads: Samaksh Ujjawal, Naveen Nair, Soham Patil | Read Shivansh's CASE paper + RL repo; get material on Samaksh / Naveen |

## Leads: IIIT-H RRC, picked from papers (2026-11-27, H015)
Picked for the v2 role: robot learning, manipulation, contact/force, sysID, RGB-D. **Liberal inference** [INF]: skills in a closely adjacent area are assumed to transfer (e.g. learned throwing parameters → learned spray parameters; aerial-manipulator contact control → arm contact control; glass/depth perception → wet and reflective restroom surfaces). Real-robot status comes from abstracts only.

### Tier 1: research these first
| # | Person | Paper(s) (first-author unless noted) | Real robot? | Why for NORM [INF] |
|---|---|---|---|---|
| 1 | **Haasith Venkata Sai Pasala** | *Identification and Learning-Based Control of an End-Effector for Targeted Throwing*, **RA-L** (with N. Govindan, S. Brahmbhatt) | **Yes**: arm-mounted end-effector | sysID + residual learning to hit a *physical outcome*. Closest analog to learning spray angle/pressure/duration for a cleaning result |
| 2 | **Md Faizal Karim** → profiled 2026-11-28 (H020); **parked: abroad [INT Vishal 2026-11-28]** | **DA-VIL** (RL + variable impedance, dual-arm, ICRA'25) · **DG16M** (16M force-closure dual-arm grasps + classifier, IROS'25) · **DAGDiff** (grasp diffusion, ICRA'26; MIT code github.com/DAG-Diff) | **Yes** (DAGDiff: xArm7 + xArm6 Lite, 32/50, H020); DG16M sim only | 3 first-author papers in 2 years: RL, diffusion, impedance/force. Contact-rich policy learning is the core v2 skill |
| 3 | **Soham Patil** | *NoContactNoWorries*: RGB-D + proprioception transformer contact estimation for RL in-hand manipulation (IROS'26) | **Yes**: sim + real | RGB-D + contact + RL + real hardware; knowing contact without tactile sensing = knowing when the brush or nozzle is touching |
| 4 | **Samaksh Ujjawal** (first author confirmed, H023) | *Learn Structure, Adapt on the Fly*: learned residual dynamics + RLS adaptation for aerial manipulators (IROS'26) | **Yes**: aerial manipulator | Learned dynamics + online adaptation = sysID with learning on real hardware |
| 5 | ~~**Rishabh Dev Yadav**~~ **dropped 2026-11-28: abroad [INT Vishal]** | Co-author on 4 IROS'26 aerial-manipulation papers; first author of *Bistable gripper + adaptive control* and *Modular adaptive aerial manipulation* (**IEEE/ASME T-Mech** ×2) | **Yes** (aerial grasping hardware) | Most prolific in the group; adaptive control of contact on real hardware; probably the senior student (PhD?) [INF] |
| 6 | **Sarthak Mishra** → profiled 2026-11-28 (H018–H019) | *AeroPlace-Flow* (language-grounded placement via object flow, 75% real success) · *AERMANI-VLM* (VLM reasoning for aerial manipulation), both IROS'26 | **Yes** | Foundation models / VLM → real manipulation. Covers the "desirable" VLA line |
| 7 | **Gaurav Singh** (now Brown University, per H020) | *Constrained 6-DoF grasp generation for dual-arm* (IROS'24, first author); co-author on DA-VIL / DG16M / DAGDiff | Not visible | Grasp generation on complex shapes ~ tool-pose generation on curved toilet surfaces |
| 8 | **Pranjali Pathre** | *Imagine2Servo*: diffusion-generated subgoals for visual servoing (IROS'24; code on GitHub) | **Yes** | Closed-loop vision → arm motion with generative models |

### Tier 2: perception for restroom surfaces, and planning
| Person | Paper | Why |
|---|---|---|
| **Tarun R** | *SILICA*: diffusion priors for joint glass segmentation + depth (IROS'26), Mirage-18k dataset | Mirrors, glass and glossy ceramic break depth cameras. This is directly our problem |
| **Suhani Grover**, **Astik Srivastava** | *GlassFormer*: radar + RGB-D glass segmentation, real-time on constrained hardware (IROS'26). Astik is also first author of *SPOT* (ICRA'26) | Reflective-surface perception on edge compute |
| **Siddharth Tourani** | Self-supervised RGB-D registration (ICRA'24); urban scene rendering (ICCV'25) | RGB-D / 3D reconstruction depth; probably senior (postdoc?) [INF] |
| **Kallol Saha**, **Vishal Mandadi** | *EDMP*: diffusion for manipulator motion planning (ICRA'24) | Learned motion generation for arms |
| **Anant Garg** | *Imagine-2-Drive*: diffusion policies + world models (IROS'25) | Policy learning (driving, but the method transfers) |

### Tier 3: niche signals
- **Shreya Bollimuntha**, **Mohammed Saad Hashmi**: co-authors on DA-VIL / DG16M.
- **Kushagra Srivastava**: *CrackUDA* (ICPR'24), defect segmentation with domain adaptation, close to contamination detection.
- **Jonish Abisheck Joseph**: data-driven identification of flapping-wing aerodynamic forces with CMA-ES (ICMA'26). Fluids + sysID + black-box optimisation, so possibly a fit for cleaning-physics experiments.

### PIs (warm paths, not candidates)
K. Madhava Krishna (RRC head) · **Nagamanikandan Govindan** (grasping/manipulation) · **Spandan Roy** (aerial manipulation, adaptive control; co-authored *Switched adaptive control for self-reconfigurable mobile cleaning robots*, IEEE T-ASE 2024, with SUTD's cleaning-robot group) · Samarth Brahmbhatt (learning-based control) · Arun Kumar Singh · Harikumar Kandath (UAV RL / sim-to-real) · Antony Thomas (Aayush Rath's PI).

## Leads not yet in CANDIDATES (public lab page H009; add only when material is provided)

| Name | Where / status | Thesis / project (as listed) | Why interesting for v2 |
|---|---|---|---|
| Manthan Goyal | HiRo RA | Interactive Robot Learning for Manipulation and HRI | IL on real arms |
| Ahan Panda | HiRo RA | Robust Imitation Learning from Imperfect Data | IL |
| Ishita Chaudhary | HiRo RA | Generalizing Robot Skills across Embodiments and Objects | Policy generalisation |
| Mumuksh Tayal | HiRo MTech(R) | Safe and Robust Deep Learning for Robotics | Safe learned control |
| Shanmukha Rao Jammalamadugu | HiRo MTech (EE) | Learning from Demonstration with Imperfect Teachers | IL |
| Jwalakar Vishnu Dutt | HiRo alumnus (2023–25) → Netradyne | Visual Imitation Learning for Long-horizon Tasks | IL, now outside robot learning, so possibly recruitable |
| Md. Farhad Hussain | HiRo alumnus (2023–25) → John Deere | Language-conditioned grasp pose learning from 3D point clouds | 3D perception + manipulation |
| Sahil Kishor Bobade | HiRo alumnus (2023–25) → ExxonMobil | Zero-shot task generalisation with VLMs + keypoint constraints | VLM manipulation |
| Siddharth Jain | HiRo alumnus (2024–26) → Honeywell | RL for safe and robust control | RL |
| Shreyas Kumar | HiRo RA (2025–26) → founding engineer, DexSent Robotics | not listed | Startup-minded; low availability |
| PhD students (Varuni Buereddy, Soumyajit Kushari, Basu Hela, Sasidhar Reddy Alavala, Mritunjoy Halder) | HiRo PhD | IL / foundation models / world models / mobile manipulation | Long-horizon: interns or future hires |

## Not yet searched (from ROLE.md plan)

- [ ] IISc labs (CPS / RBCCPS, Aerospace, CSA)
- [ ] IIT Madras / Bombay / Delhi / Kanpur / Hyderabad robotics labs and clubs
- [ ] IIIT Hyderabad RRC alumni
- [ ] BITS robotics clubs / alumni
- [ ] Indian robotics companies (Addverb, CynLr, Ati Motors, Ottonomy, Sastra, Anscer, Invento, GreyOrange, Unbox, Swaayatt)
- [ ] Indians abroad: CMU RI, ETH, TUM, GaTech, UMich, UPenn, Stanford, Berkeley; NVIDIA Isaac, PickNik, Boston Dynamics, Figure, etc.
- [ ] ROSCon / ROSCon India 2024–2025 speakers
- [ ] Open-source contributors: ROS 2, Nav2, MoveIt 2, Isaac Lab, LeRobot
- [ ] RSS / CoRL / ICRA / IROS Indian authors (manipulation, sim-to-real)
- [ ] Competition winners: Inter-IIT Tech Meet, ABU Robocon, ERC, IGVC
- [ ] ARTPARK (IISc) startups and interns: Automind Dynamics etc. (lead from Chalus Jude J)
- [ ] (v2) LeRobot / ACT / diffusion-policy / Isaac Lab contributors; CoRL/RSS manipulation authors
- [ ] (v2) Robotic painting / spraying / surface-finishing teams (FANUC/ABB paint integrators, finishing startups); CynLr, Sastra
