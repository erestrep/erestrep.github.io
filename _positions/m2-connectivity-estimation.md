---
layout: page
title: Robust Distributed Connectivity Estimation for Human-Multi-Robot Teleoperation
description: Open research internship position (stage M2)
img: assets/img/M2stage-connect.png
importance: 3
category: Master thesis
giscus_comments: true
---

**Short abstract:** This Master's Thesis will investigate a novel distributed algorithm for **estimating the algebraic connectivity** of robotic swarms, leveraging **diffusion models** to ensure numerical stability and scalability. The approach will be validated on real hardware in a **human-multi-robot teleoperation scenario**, ensuring network cohesion under dynamic human guidance.


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

**Description and motivation:** In the field of Cooperative Multi-Agent Systems, maintaining network integrity is not merely a communication issue—it is a fundamental control constraint. Whether for formation control, collision avoidance, or distributed sensing, a robot swarm must remain algebraically connected to function as a cohesive unit. This is formalized through the concept of "Generalized Connectivity" [1-3], where the graph’s algebraic connectivity (the Fiedler eigenvalue) serves as a real-time proxy for the system’s stability and operational health.

While computing connectivity centrally is trivial, estimating it in a fully distributed manner (where robots only talk to neighbors) remains an open problem for dynamic systems. Current state-of-the-art methods [5][6] rely on distributed power iteration techniques that are numerically fragile. They suffer from slow convergence and require complex parameter retuning whenever the network topology changes—making them ill-suited for real-world deployment.

This challenge is amplified in Human-Multi-Robot Interaction (HMRI). When a human operator teleoperates a fleet of robots (e.g., using a joystick to guide a swarm through a disaster zone), the human's commands can result in rapid, unpredictable changes to the swarm's formation. The system requires a fast, robust estimator to alert the controller before the network fractures, ensuring the human can guide the swarm aggressively without breaking communication links.

This Master's Thesis will develop a novel, adaptive estimation algorithm based on **diffusion graph models**. Unlike standard consensus approaches, this method will aim to be robust to topological switching, allowing the swarm to self-monitor its connectivity in real-time without constant retuning.


**General Objectives:** The main goal is to design, analyze, and validate a distributed algorithm that surpasses current methods in scalability, numerical stability, and convergence speed. The student will:

* Develop a distributed connectivity estimator leveraging diffusion models and power iteration that is mathematically robust to dynamic graph topology changes.
* Integrate the algorithm into a human-multi-robot teleoperation framework. The estimator will act as a safety layer, providing real-time feedback to ensure the swarm maintains cohesion while following human velocity commands.
* Test the complete system first in simulation (e.g., ROS2/Gazebo) and subsequently on real robotic hardware, demonstrating the system's ability to prevent network fragmentation during complex maneuvers.

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

