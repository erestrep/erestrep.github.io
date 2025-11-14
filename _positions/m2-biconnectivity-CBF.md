---
layout: page
title: Resilient Coordination of Multi-robot Systems
description: Open research internship position (stage M2)
img: assets/img/connect.png
importance: 1
category: Master thesis
giscus_comments: true
---

**Short abstract:** The objective of this Master’s thesis is to develop a **distributed strategy** for the coordination of a multi-robot system subject to **multiple constraints** (e.g. collision avoidance, connectivity and visibility maintenance) and performing **multiple objectives** (etc. coverage missions, clustering), while being **resilient** to robot failure or mission and environmental changes.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/connect.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Snapshot of an simulation of drone coordination using the generalized connectivity model in [1].
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Esteban Restrepo](https://erestrep.github.io/), [Nicola De Carli](https://www.kth.se/profile/ndc)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [ndc@kth.se](mailto:ndc@kth.se)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-res-coord/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description and motivation:** The deployment of **robotic fleets** has proven effective for various cooperative tasks such as reconnaissance, surveillance, load transportation, and imaging. While a fixed number of agents can perform short-term tasks like formation tracking or area coverage, this approach becomes limiting in practical, **long-term missions**. Such missions often exceed the robots’ battery life, requiring agents to temporarily leave for recharging and rejoin later. Additionally, in dynamic or adversarial environments, robot failures or attacks are inevitable, and new robots may need to join as tasks or environments evolve. Hence, agent addition and removal are inherent to realistic multi-robot operations. These additions and removals, however, demand **resilient strategies** capable of managing agent changes while ensuring the satisfaction of **inter-agent constraints** and overall mission objectives.

To address these challenges, this master thesis builds upon a **generalized biconnectivity framework** [1,2] where the interconnection between robots is defined as a product of weights that encode factors like **proximity-based interactions** (distance-dependent), **sensing limitations** (field-of-view constraints), **hard constraints** (collision avoidance, connectivity maintenance) and **soft constraints** (formation control, cooperative behavior), and that is resilient to the removal or addition of agents due to, e.g., failure, battery discharge, changing mission specifications or environmental conditions. Then, relying on the **distributed Control Barrier Function (CBF) framework** [3]​, this thesis will study how to provide an optimal controller for the coordination of a multi-robot system that satisfies the system’s constraints and that is resilient to a change in the number of robots.


**General Objectives:** The goal of this Master Thesis is to propose a distributed strategy based on the results of [1,2,3] in order to achieve **resilient coordination in a team of multiple robots subject to multiple constraints and objectives**. The proposed algorithms will be **validated through simulations and experiments** using a team of mobile robots (ground robots and mini-drones).

By integrating a **resilient generalized biconnectivity strategy with the CBF framework**, this thesis will contribute to the development of **next-generation resilient multi-robot systems** capable of operating in real-world, dynamic environments.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the experimental setup in the team.

2. Take over the existing works and work on the CBF-based distributed and resilient coordination strategy for a multi-robot system.

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

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-res-coord/).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Nicola De Carli

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Restrepo, E., & Robuffo Giordano, P. (2024, December). A Distributed Strategy for Generalized Biconnectivity Maintenance in Open Multi-robot Systems. In 2024 IEEE 63rd Conference on Decision and Control (CDC) (pp. 3043-3050). IEEE.

2. Restrepo, E., & Robuffo Giordano, P. (2023). Distributed biconnecitvity achievement and preservation in multi-agent systems. IEEE Control Systems Letters, 7, 3289-3294.

3. De Carli, N., Salaris, P., & Giordano, P. R. (2024, May). Distributed control barrier functions for global connectivity maintenance. In 2024 IEEE International Conference on Robotics and Automation (ICRA) (pp. 12048-12054). IEEE.

4. P. Robuffo Giordano, Q. Delamare, A. Franchi. Trajectory Generation for Minimum Closed-Loop State Sensitivity. In IEEE Int. Conf. on Robotics and Automation, ICRA’18, Pages 286-293, Brisbane, Australia, May 2018

5. Ames, A. D., Coogan, S., Egerstedt, M., Notomista, G., Sreenath, K., & Tabuada, P. (2019, June). Control barrier functions: Theory and applications. In 2019 18th European control conference (ECC) (pp. 3420-3431). IEEE.

