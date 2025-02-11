---
layout: page
title: Cluster-consensus control for swarms of robotic vehicles
description: Open research internship position
img: assets/img/M2stage-cluster.png
importance: 3
category: Master thesis
giscus_comments: true
---

**Short abstract:** The goal of this Master Thesis is to exploit recent advancements on the topic of multi-robot control for the design and analysis of distributed control laws to achieve autonomous formation of clusters in a swarm of mobile robots.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/M2stage-cluster.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Previous experiment with the fleet of Crazyflies (left) and example of multi-robot clustering [Gandhe, M., Otte, M. (2023). Decentralized Robot Swarm Clustering: Adding Resilience to Malicious Masquerade Attacks. In: LaValle, S.M., O’Kane, J.M., Otte, M., Sadigh, D., Tokekar, P. (eds) Algorithmic Foundations of Robotics XV. WAFR 2022. Springer Proceedings in Advanced Robotics, vol 25. Springer] (right)
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Paolo Robuffo Giordano](https://team.inria.fr/rainbow/fr/team/prg/), [Esteban Restrepo](https://erestrep.github.io/), and Antonio Marino

**Contact:** [prg@irisa.fr](mailto:prg@irisa.fr) – [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [antonio.marino@irisa.fr](mailto:antonio.marino@irisa.fr)

**How to apply:**  Interested candidates are requested to apply via [this form](https://forms.gle/nqmRwCzMqTVN41C1A). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description:** The deployment of swarms of robotic vehicles has been shown to be effective for a wide range of applications based on cooperative tasks such as reconnaissance, surveillance, foraging or search and rescue. Most of the time, in such collaborative missions, the field of interest is relatively large with respect to the size of the multi-robot system. Therefore, the swarm must be divided into smaller groups (clusters) to move towards different areas and conduct different tasks simultaneously.

**Motivations:** Most of the current works addressing the problem of clustering for multi-agent systems are concerned with generic unconstrained agents, thus neglecting the constraints and specificity of networks of mobile robots in terms of limited sensing capabilities. Moreover, they only study the conditions for convergence of the agents to small groups, i.e. cluster consensus, rather than the autonomous formation of clusters. There are few works addressing the autonomous achievement of clusters in a network of mobile robots based on distributed and local interactions among the robots, none of which take also into account the sensing constraints inherent to these types of systems.

**General Objectives:** The goal of this Master Thesis is to design and validate theoretically (using Lyapunov methods, graph theory, etc.) novel control laws for the autonomous achievement of cluster consensus of a swarm of robotic vehicles subject to sensing constraints (limited range, limited field of view) based on local and distributed interaction laws among the robots. The work done during the the internship will be validated in simulation and experimentally using a fleet of Crazyflie drones.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the experimental setup in the team.

1. Take over the existing works and work on the design and analysis of a control algorithm for autonomous cluster consensus of multi-robot systems

1. Implement and validate in simulation the proposed algorithms.

1. Validate experimentally the scenario on a fleet of Crazyflie drones.

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation and interest in the topic

* Good knowledge in control theory and robot modeling

* Good experience using Matlab/Simulink

* Basic knowledge of control and analysis of multi-agent systems is appreciated

* Previous experience with Python/C++ and ROS2 is appreciated

* Scientific curiosity

<br>
<hr>
<br>

<h3 class="subsection-title">Conditions</h3>
<br>

The work will be carried in English at the Centre Inria de l’Université de Rennes research center in Rennes, France.

Financial support offered to the student: gratification de 4,35 € / h

<br>
<h3 class="subsection-title">How to apply</h3>
<br>

Interested candidates are requested to apply via [this form](https://forms.gle/nqmRwCzMqTVN41C1A).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Paolo Robuffo Giordano, and Antonio Marino

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Xia, W., & Cao, M. (2011). Clustering in diffusively coupled networks. Automatica, 47(11), 2395-2405.

1. Zhang, Z., Wu, W., & Zhang, F. (2024). Opinion-based Task Allocation Strategy for Mobile Sensor Networks. American Control Conference, 1-6.

1. Menara, T., Baggio, G., Bassett, D. S., & Pasqualetti, F. (2019). Stability conditions for cluster synchronization in networks of heterogeneous Kuramoto oscillators. IEEE Transactions on Control of Network Systems, 7(1), 302-314.

1. Burger, M., Zelazo, D., & Allgower, F. (2012). Hierarchical clustering of dynamical networks using a saddle-point analysis. IEEE Transactions on Automatic Control, 58(1), 113-124.

1. Sharf, M., & Zelazo, D. (2022, May). Cluster assignment in multi-agent systems. In 2022 13th Asian Control Conference (ASCC) (pp. 947-952). IEEE.
