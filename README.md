# y-combinator-fall-2026
y combinator fall 2026

Part 1: Y Combinator Core Application
1. What does your company do? (50-character limit)
Real-time edge telemetry for distributed physical security.

2. What are you building? Describe your product and the problem it solves.
Enterprise physical security systems are drowning in unmanageable raw video. Piping multi-camera 4K feeds over cellular or constrained uplinks to cloud servers results in crippling bandwidth saturation, massive cloud egress and storage bills, and unacceptable alerting latency.

We eliminate the raw video transmission bottleneck entirely. Our edge-native runtime mounts directly onto local compute nodes to distill high-dimensional video and sensor streams down into low-dimensional mathematical state vectors (kinematics, bounding-box trajectories, acoustic frequency bands, and spatial transitions).

Instead of streaming gigabytes of dead footage, our edge nodes transmit lightweight, structured telemetry bursts (sub-kilobyte JSON/protobuf) over any connection—even degraded cellular. The central platform reconstructs site dynamics, tracks multi-sensor anomalies using robust generative classification, and only queries high-resolution video retroactively when a deterministic threshold is breached.

3. What is your unfair advantage or deep technical insight?
Traditional cloud-AI security startups treat the camera as a dumb pipe and dump raw pixels into foundation models hosted in centralized data centers. This falls apart outside of fiber-connected environments.

Our technical insight is that site situational awareness is a low-dimensional state estimation problem, not a raw pixel streaming problem. By leveraging localized statistical modeling—such as additive classification scorecards and Kalman state estimation—we decouple detection and classification from bandwidth availability. We can monitor an entire 50-camera industrial facility over a 64 kbps link with zero false-alarm spam, cutting data transmission costs by 99% and dropping incident detection latency to single-digit milliseconds.

Part 2: In-Q-Tel (IQT) Dual-Use & Operational Utility Brief
Operational Challenge: Contested & DDIL Environments
Current Tactical Operations Centers (TOCs) and forward perimeter installations operate under DDIL (Denied, Disrupted, Intermittent, and Limited bandwidth) conditions. Enemy EW, satellite link degradation, or localized jamming makes offboarding full-motion video (FMV) impossible. Force protection systems that rely on persistent cloud connectivity or fat network pipes become dark instantly in contested domains.

Dual-Use Technical Architecture
Tactical Edge Distillation: The edge engine sits directly on local, low-SWaP (Size, Weight, and Power) edge appliances, processing thermal, electro-optical (EO), and acoustic arrays locally.

Low-Dimensional Telemetry Ingestion: Sensor data is compressed at ingestion into normalized feature vectors (speed, thermal area, trajectory vectors, acoustic signatures).

Bandwidth-Agnostic Telemetry: By transmitting only state vectors (<1 KB/sec per sector), comprehensive situational awareness persists over tactical radios, high-frequency (HF) links, or degraded SATCOM links.

Asymmetric Threshold Escalation: Local classification utilizes additive log-odds scoring with configurable loss matrices. False alarms on routine perimeter traffic are suppressed without saturating the link, while high-consequence anomalies immediately trigger local physical interlocks and alert operators with the precise vector anomaly data.

Next Step
We can either refine the YC founder background / "Why you?" narrative to emphasize enterprise physical security domain expertise, or outline the 10-slide technical pitch deck structure next. Which would you prefer to tackle?
