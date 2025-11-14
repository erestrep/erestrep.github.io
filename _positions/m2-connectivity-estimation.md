---
layout: page
title: Scalable Distributed Connectivity Estimation for Multi-robot Systems
description: Open research internship position (stage M2)
img: assets/img/M2stage-connect.png
importance: 2
category: Master thesis
giscus_comments: true
---

**Short abstract:** The objective of this Master’s thesis is to develop a **scalable and distributed algorithm** for connectivity estimation in a multi-robot system subject to **multiple constraints** (e.g. collision avoidance, connectivity and visibility maintenance) via **distributed diffusion models**.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/M2stage-connect.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Snapshot of an experiment of drone formation using the generalized connectivity model in [3].
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Dr. Esteban Restrepo](https://erestrep.github.io/), [Dr. Antonio Marino](https://scholar.google.fr/citations?user=bKy_YlkAAAAJ&hl=fr)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [antonio.marino@cl.cam.ac.uk](mailto:antonio.marino@cl.cam.ac.uk)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/application-form-internship-on-scalable-distributed-connectivity-estimation-for-multi-robot-systems/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description and motivation:** Ensuring robust connectivity is a foundational requirement for the successful operation of cooperative multi-agent systems [1][2], enabling the coordination and information flow necessary for complex tasks. This concept extends far beyond simple communication, forming the basis of a "generalized connectivity" framework [3] where maintaining specific inter-agent links is used to encode a wide array of operational constraints, from collision avoidance to formation keeping and task satisfaction. In this paradigm, monitoring the graph's algebraic connectivity becomes a direct proxy for mission-wide success. However, estimating this global network property in a distributed fashion, a necessity for any scalable system, remains a significant challenge. Current methods are often impractical for dynamic, large-scale systems. Many centralized or flooding-based approaches [4] are not scalable, as they implicitly require agents to reconstruct the full adjacency matrix, a non-viable solution in a distributed setting. On the other hand, existing distributed iterative and consensus-based estimators [5][6], based on a distributed version of the power iteration, suffer from a critical tuning problem: their convergence rates and stability parameters are highly sensitive to the network's topology, requiring complex re-tuning every time the graph changes. 

This Master Thesis will address this critical gap by investigating a novel adaptive estimation algorithm that is both fully distributed and robust to the very topological changes it seeks to monitor. As a starting point, this work draws inspiration from power iteration methods, which refine a random signal to predict connectivity, and proposes to design a novel diffusion graph model that achieves this purpose with increased performance regardless of topology. A key investigation will be to demonstrate that the sacrifice in communication load implied by such a diffusion model yields quantifiable improvements in estimation accuracy and robustness. The algorithm's performance, scalability, and robustness to topological changes will be rigorously validated through theoretical analysis and extensive simulation.


**General Objectives:** The goal of this Master Thesis is to propose a **distributed algorithm to compute the connectivity of a group of robots** which overcome the limitations of current state of art methods: scalability, numerical stability and convergence speed. By leveraging **distributed diffusion models** iterations [4][5][6] this thesis will stand on cutting-edge methodologies and will contribute to the real deployment of multi-robot fleets. **The approach developed will be extensively tested in simulation and on a team of mini aerial drones**.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the  current baselines.

2. Develop the methodology and analysis of the theoretical guarantees.

3. Implement and validate in simulation the proposed algorithms.

4. Validate experimentally the scenario on a team of mobile robots.

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation and interest in the topic

* Good knowledge in control theory and robot modeling

* Basic knowledge of control and analysis of multi-agent systems

* Previous experience with Python/C++ and ROS2

* Scientific curiosity

<br>
<hr>
<br>

<h3 class="subsection-title">Conditions</h3>
<br>

Expected duration of the internship: **5-6 months**

The work will be carried in English at the Centre Inria de l’Université de Rennes research center in Rennes, France.

Financial support offered to the student: gratification de 4,35 € / h

<br>
<h3 class="subsection-title">How to apply</h3>
<br>

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/application-form-internship-on-scalable-distributed-connectivity-estimation-for-multi-robot-systems/).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Antonio Marino

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Restrepo, E., & Robuffo Giordano, P. (2024, December). A Distributed Strategy for Generalized Biconnectivity Maintenance in Open Multi-robot Systems. In 2024 IEEE 63rd Conference on Decision and Control (CDC) (pp. 3043-3050). IEEE.

2. Restrepo, E., & Robuffo Giordano, P. (2023). Distributed biconnecitvity achievement and preservation in multi-agent systems. IEEE Control Systems Letters, 7, 3289-3294.

3. Robuffo Giordano, Paolo, et al. "A passivity-based decentralized strategy for generalized connectivity maintenance." The International Journal of Robotics Research 32.3 (2013): 299-323.

4. Griparic, Karlo, et al. "Consensus-based distributed connectivity control in multi-agent systems." IEEE transactions on network science and engineering 9.3 (2022): 1264-1281.

5. Yang, Peng, et al. "Decentralized estimation and control of graph connectivity for mobile sensor networks." Automatica 46.2 (2010): 390-396.

6. Stamouli, Charis J., Charalampos P. Bechlioulis, and Kostas J. Kyriakopoulos. "Multi-agent formation control based on distributed estimation with prescribed performance." IEEE Robotics and Automation Letters 5.2 (2020): 2929-2934.

