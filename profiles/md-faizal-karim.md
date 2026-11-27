# Md Faizal Karim

| Field | Value |
|---|---|
| Current role | Researcher, **Robotics Research Center, IIIT Hyderabad** (K. Madhava Krishna's group); degree/position **not visible** (no LinkedIn yet) [V] H020 |
| Location / willing to move | Hyderabad (affiliation) [V] H020 · willingness not known |
| Education | Not visible. Need LinkedIn/CV |
| Previous | Not visible |
| Links | [DAGDiff project page](https://dag-diff.github.io/dagdiff/) · code github.com/DAG-Diff (per H015) · LinkedIn not yet found |
| Sources | H015, H020 |

## Evidence by requirement
| Requirement (ROLE.md v2) | Evidence | Tag |
|---|---|---|
| A Real-robot manipulation | **DAGDiff** (ICRA 2026, first author, equal contribution with Vignesh Vembar): dual-arm grasps generated from real point clouds and **executed on a heterogeneous xArm7 + xArm6 Lite setup**: 32/50 successful grasp-and-lift on unseen objects (tray 6/10, bucket 8/10, saucepan 7/10, frypan 6/10, drone 5/10). Failures mostly from point-cloud reconstruction | [V] H020 |
| B Robot learning | DAGDiff: SE(3)×SE(3) **diffusion model** with classifier guidance (force-closure, collision and geometry heads; VN-PointNet encoder), trained by the team; ablations show the FC head doubles success. **DA-VIL** (ICRA'25, first author): RL + variable impedance for dual-arm manipulation. **DG16M** (IROS'25): 16M-grasp dual-arm dataset + classifier | [V] H020; [3P] H015 |
| C Sim–real–sim | Large-scale **Isaac** physics evaluation (grasp success / collision rates), then **zero-shot transfer** to real sensor data | [V] H020 |
| D Contact physics / experiments | Force-closure analysis; variable impedance (contact-rich control) in DA-VIL | [V] H020; [3P] H015 |
| E RGB-D perception & calibration | Two RealSense D455 point clouds fused via ICP; arms calibrated with an AprilTag | [V] H020 |
| F Research | 3 first-author papers at ICRA/IROS in about 2 years; DAGDiff code public (MIT) per H015 | [V] H020; [3P] H015 |

Liberal-transfer note [INF]: contact-aware, stability-guided generation of tool/grasp poses on large curved objects (buckets, saucepans) maps closely onto generating brush/spray poses on curved toilet and sink surfaces; variable-impedance RL maps onto controlled scrubbing force.

## Three-axis summary (2026-11-28)
| Axis | Result | Basis |
|---|---|---|
| Reputation | **8/10 (A), provisional** | Edu 3 (IIIT-H research; degree not visible) · Employer 2 (IIIT-H RRC) · Signal 3 (3 first-author ICRA/IROS papers, open code) |
| Can we get them? | **Unknown (assume Medium)** | In Hyderabad; career stage unknown; strong PhD-abroad candidate profile [INF] |
| Technical (v2) | **70/100, Tier B (A-candidate)** | See score below |
| Contact priority | **P1** (provisional) | Technical ≥50; gettability assumed ≥Medium |

## Score (v2): pre-interview estimate
| Criterion | Weight | 0–5 | Why |
|---|---|---|---|
| A Real-robot manipulation | 25% | 4 | Learned grasp model executed on real xArm7 + xArm6 dual-arm setup [V] |
| B Robot learning & PyTorch | 20% | 4 | Guided SE(3) diffusion + RL/impedance work; learned model on a real robot [V] |
| C Sim–real–sim | 20% | 3 | Isaac evaluation → zero-shot real; no sim calibration from real data |
| D Experimental optimisation / cleaning physics | 15% | 2 | Force-closure and impedance; no process optimisation |
| E RGB-D perception & calibration | 10% | 4 | Multi-camera fusion + AprilTag arm calibration |
| F Research & reproducibility | 10% | 4 | 3 first-author ICRA/IROS + public code |
**Total: 70 / 100.** Passes the A gate on paper (A 4, C 3, B 4) and hits the 70 threshold, **the first in the pipeline to do so**. Held at **Tier B** until we confirm ≥3 years of hands-on robotics (ROLE.md junior rule) and his personal share of the work. Confidence Medium (team papers; no CV).

Caveat: the real-robot result is open-loop grasp-and-lift, not a closed-loop learned policy. A strict reading of the gate ("learned policy on a real robot") could keep B at 3; DA-VIL's real-robot status would settle it.

## Availability signals
- Not visible. Need LinkedIn: degree (MS by Research? PhD?), start year, plans.

## Concerns / gaps
- No CV / LinkedIn: degree, years of experience and gettability are guesses.
- Equal-contribution first author; Vignesh Vembar's share vs his not known.
- Profile looks PhD-bound (3 top-venue first-author papers) [INF].

## Outreach notes
- Not contacted. Warm path: **K. Madhava Krishna** (RRC head) or IIIT-H RRC network (Aayush Rath is at RRC).
- Pitch angle: take grasp/contact generation from lab objects to a real product doing contact-rich cleaning on curved surfaces.

## Open questions
- LinkedIn/CV: degree, year, plans (PhD abroad?).
- Did DA-VIL run on the real arms? Closed-loop policies anywhere?
- What did he build personally in DAGDiff (model, training, real-robot pipeline)?
- Co-authors worth a look: **Vignesh Vembar** (co-first author), **Keshab Patra**, **Gaurav Singh** (now Brown University, per DAGDiff affiliation).
