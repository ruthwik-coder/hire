# Chalus Jude J

| Field | Value |
|---|---|
| Current role | Autonomous Systems Intern, Automind Dynamics, ARTPARK (since Sep 2026) [CC] H007 |
| Location / willing to move | Chennai, Tamil Nadu (LinkedIn) [CC] H007. ARTPARK is at IISc Bengaluru [INF], so he may already be in Bengaluru |
| Education | **B.E. Mechanical Engineering, Bannari Amman Institute of Technology, Erode: Aug 2023 – May 2027 (still a student, final year)** [CC] H007 |
| Previous | Full-Stack Robotics Intern, "AI-Based Industrial Automation Lab", Erode (Nov 2025 – Oct 2026) · Design/Product Development, "Aquatech Innovation Lab", Erode (Dec 2023 – Nov 2025; AUVs, autonomous waste-collection boat, rescue buoy, single-thruster ROV) · Industrial Design Engineer (intern), IIT Madras (Jul–Oct 2025; mechanical design, FEA, GD&T) [CC] H007. The two Erode "labs" are probably college labs at BIT [INF] |
| Links | [LinkedIn](https://www.linkedin.com/in/chalus-jude-j-921b9620a) · [Portfolio](https://chalus-jude.github.io/Portfolio/) (not yet read) · MuJoCo clip https://lnkd.in/gp9xnByX (not yet viewed) |
| Sources | H007, H008 |

## Evidence by requirement
| Requirement (ROLE.md) | Evidence | Tag |
|---|---|---|
| 1. Robot software architecture | ROS 2 Humble; industrial AGV "developed and deployed" at OPEL on a live shop floor: FSM junction control, encoder–IMU–odometry fusion | [CC] H007 H008 |
| 2. Manipulation | Built his own **5-DOF arm + 1-DOF gripper** (Dynamixel servos, 3D-printed links). Benchmarks analytical Jacobian IK, neural IK and RL policies in one Cartesian pose-target framework. Not a 6-axis industrial arm; whether the learned controllers run on the **real** arm is not shown (the 100-arm run is "Simulation only") | [CC] H007; post H008 |
| 3. Mobile navigation | AGV: classical vision (HSV/HLS/LAB segmentation, Hough lane extraction, ArUco pose references). That is **lane following, not SLAM/Nav2-type planning**. Lists Nav2 and EKF. "Fault-tolerant navigation with RL-based recovery" claimed | [CC] H007 |
| 4. ML from scratch | Post H008 gives real design detail. **IKNet**: 9-D input with the continuous 6-D rotation representation (vs Euler angles); 4-block residual MLP, about 2.1M parameters; tanh head scaled to joint limits; **trained with a forward-kinematics loss so it doesn't average multiple IK solutions**. W&B tracking. **PPO reaching policy**: 36-D observation, separate actor/critic, 2,048 parallel envs (Stable-Baselines3), curriculum on success tolerance. Those are correct, non-trivial design choices [INF], but the RL uses an off-the-shelf library and a textbook reaching task. Code not seen. Headline also lists VLA and Isaac Lab, with no evidence for either | [CC] H008; [INF] |
| 5. Simulation & sim-to-real | Gazebo + MuJoCo twins of his arm; 100 arms in MuJoCo; CAD-grounded Gazebo digital twins "for sim-to-real verification"; Isaac Sim / Isaac Lab listed. No real sim-to-real result shown | [CC] H007 H008 |
| 6. Hardware literacy | Mechanical engineer: CAD, FEA, DFM, GD&T. 6-thruster ROV, AUVs, Dynamixel arm, AGV sensors. Hands-on builder | [CC] H007 |
| Field / competitions | **Winner, AquaVision'25 + Best Algorithm Development Award** (vision-based AUV challenge). AGV at OPEL | [CC] H007 |
| Collaborator | The arm project was done with "ARUNKUMAR M" (named in the post). His share is not known | [CC] H008 |

## Three-axis summary (2026-11-27)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **3/10 (D)** | Edu 1 (Bannari Amman, Other) · Employer 1 (ARTPARK/IITM internships) · Signal 1 (AquaVision'25 win) |
| Can we get them? | **High (intern now) / Medium (full-time after May 2027)** | Tamil Nadu / ARTPARK (IISc ecosystem); undergraduate until May 2027; startup-minded |
| Technical (v2) | **39/100, Tier C** | See score below |
| Contact priority | **P2** | ROLE.md rule |

## Score (v2 rubric, 2026-11-24): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 2 | Own hobby-grade 5-DOF Dynamixel arm, analytical Jacobian IK; learned control on the real arm not shown |
| B Robot learning & PyTorch | 20% | 3 | Neural IK (FK loss, 6-D rotation rep) + PPO with curriculum in sim; PyTorch, W&B. [CC] only, so capped at 3 |
| C Sim–real–sim | 20% | 2 | Gazebo + MuJoCo twins, 2,048 parallel envs; no transfer shown |
| D Experimental optimisation / cleaning physics | 15% | 1 | Mechanical engineering fundamentals (FEA, vibration); AUV/ROV thrusters |
| E RGB-D perception & calibration | 10% | 1 | Classical 2D vision (HSV, Hough, ArUco) |
| F Research & reproducibility | 10% | 2 | Tracked experiments, clear technical write-up; no papers |
**Total: 39 / 100 → Tier C** (junior: undergraduate until May 2027) · confidence Low–Medium. Best robot-learning signal of the three, so intern/junior track.

## Score v1 (superseded: old Head-of-stack brief)
| Criterion | 0–3 | Why |
|---|---|---|
| 1 Robot software stack | 2 | ROS 2 AGV built and claimed deployed |
| 2 Manipulation | 1 | Own hobby-grade 5-DOF arm; learned control shown in sim only. Becomes 2 if it runs on the real arm |
| 3 Navigation | 2 | Real AGV on a shop floor, but classical lane following, not SLAM |
| 4 ML from scratch | 2 | Trains his own models with sound design reasoning (neural IK, PPO). Not novel research |
| 5 Simulation & sim-to-real | 2 | Builds sim twins and parallel RL envs; no transfer shown |
| 6 Hardware literacy | 2 | Strong mechanical and builder skills across arms, AUVs and AGVs |
| 7 Shipped / field | 2 | AGV pilot at OPEL + competition win (both [CC]) |
| 8 Ownership / leadership | 2 | Led AUV design work; builds whole systems end to end |
| 9 Pedigree & signal | 1 | Tier-3 college, no publications; one competition win; good public technical writing |
| 10 Fit & availability | 2 | Local (TN, ARTPARK/IISc), but a student until May 2027. Intern now, full-time mid-2027 |
**Total:** 18 / 30 → **Tier C** for the head role, because he is still an undergraduate. **High-potential intern / junior hire**: the most hands-on ML + RL + hardware mix seen so far for his level.

## Availability signals
- Graduates May 2027. A final-year internship or job offer could be timed for that [INF].
- Already in the IISc/ARTPARK ecosystem, the same one as Ubanthu's incubation [INF].

## Concerns / gaps
- **Very junior:** undergraduate, and every role so far is an internship or college lab.
- **LinkedIn inflation:** buzzword headline (DeepRL • VLA • Isaac Lab), phrases like "redefining the boundaries", and overlapping lab roles. Discount the claims until code or video is seen [INF].
- The RL and neural IK are well explained, but the task is a standard benchmark (reaching), done in sim with SB3. That shows he can do the method; it doesn't show research depth.
- No real 6-axis industrial arm, and no SLAM.

## Outreach notes
- Not contacted. **Warm path:** ARTPARK at IISc. Ubanthu's IISc incubation network could reach him through Automind Dynamics or ARTPARK staff.
- Natural offer: an internship (now or from Jan 2027), converting to full-time after May 2027.

## Open questions
- Did the neural IK or PPO policy run on the physical Dynamixel arm? Which share of the work was his and which was Arunkumar M's?
- Is the code public (portfolio/GitHub)? View the MuJoCo clip and the post's architecture document.
- What does Automind Dynamics build at ARTPARK, and what does he do there?
- How real was the OPEL AGV deployment (duration, uptime, is it still running)?
