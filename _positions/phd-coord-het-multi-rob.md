---
layout: page
title: Coordination of Heterogeneous Multi-robot systems for Multi-objective Missions
description: Open PhD position
img: assets/img/phd_cluster.png
importance: 1
category: PhD
giscus_comments: true
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/phd_cluster.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example of a multi-ressource multi-location task allocation experimental validation with a team of Crazyflies performed in the Rainbow team.
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Paolo Robuffo Giordano](https://team.inria.fr/rainbow/fr/team/prg/) and [Esteban Restrepo](erestrep.github.io)

**Contact:** [prg@irisa.fr](mailto:prg@irisa.fr) – [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-phd-coord-het-multi-robot/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>
<h3 class="subsection-title">Context</h3>
<br>

**Multi-robot systems** are increasingly being deployed in applications such as surveillance, environmental monitoring, and industrial automation. Most of the current works focus on homogeneous multi-robot systems collaboratively carrying out a single simple task such as coverage, exploration, object pushing, etc. [1]. However, achieving seamless collaboration among **heterogeneous robots** with diverse capabilities performing complex missions remains a challenge. These missions often consist of **multi-objective tasks** (e.g., in an agricultural setting: foraging, transportation, inspection, etc.) requiring different tools or capabilities in expansive and **dynamically changing** environments, necessitating advanced interaction models.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

Interaction paradigms observed in social and biological networks such as, e.g., stubbornness, clustering, or inhibitory interactions, have the potential to improve the coordination of heterogeneous robots by enabling them to exhibit adaptive, resilient, and complex behaviors to execute multi-task missions in dynamically changing environments.

**This PhD aims to enhance the coordination of heterogeneous multi-robot systems by leveraging the dynamic models used to describe complex interactions in social and biological networks** [2]. The plan of this PhD is to adapt the latter to multi-robot systems with sensing and actuation constraints in order to resiliently perform multi-objective tasks in dynamically changing environments.

For this purpose the goal is to directly model the interactions among the robots based on **nonlinear agreement protocols** [3], **opinion dynamics** [4] and **multi-layer graphs** [5], taking into account the different capabilities of the agents and the multi-objective tasks. Current works on opinion dynamics consider only static and unconstrained agents where the model of the opinion dynamics are used to explain different phenomena occurring in social or biological networks. This PhD will investigate instead how the inclusion of an opinion layer in the interactions of multiple heterogeneous mobile robots with sensing and actuation constraints can lead to complex and resilient behaviors in the context of multi-objective missions. In a second time, and due to the complexity of the system, approaches based on reinforcement learning may be considered to increase the adaptability and robustness of the swarm to dynamic conditions.

**Experimental validation:** the control methods and algorithms will be validated and tested on tasks progressively advancing from simpler missions such as forming clusters and simultaneously aggregating at different locations of interest, to a long-term dynamical mission that needs reconfiguration of the robotic team. The experimental validation will utilize the facilities of the Rainbow team, including two indoor and multi-robot arenas and several mobile robots (e.g. a team of Crazyflie mini drones—see picture).

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* M.Sc. degree in computer science, robotics, engineering, applied mathematics (or related fields)
* Good knowledge in control theory and robot modeling
* Good experience using Matlab/Simulink
* Previous experience with Python/C++ and ROS2 is appreciated
* Basic knowledge of control and analysis of multi-agent systems is appreciated
* Scientific curiosity, large autonomy and ability to work independently

<br>
<hr>
<br>

<h3 class="subsection-title">Conditions</h3>
<br>

The Ph.D. position is full-time for **3 years** (standard duration in France)

The position will be paid according to the French salary regulations for PhD students.

<br>
<h3 class="subsection-title">How to apply</h3>
<br>

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-phd-coord-het-multi-robot/).

**Supervisor(s):** Dr. Esteban Restrepo and Dr. Paolo Robuffo Giordano

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Xia, W., & Cao, M. (2011). Clustering in diffusively coupled networks. Automatica, 47(11), 2395-2405.

1. Zhang, Z., Wu, W., & Zhang, F. (2024). Opinion-based Task Allocation Strategy for Mobile Sensor Networks. American Control Conference, 1-6.

1. Menara, T., Baggio, G., Bassett, D. S., & Pasqualetti, F. (2019). Stability conditions for cluster synchronization in networks of heterogeneous Kuramoto oscillators. IEEE Transactions on Control of Network Systems, 7(1), 302-314.
   
1. Burger, M., Zelazo, D., & Allgower, F. (2012). Hierarchical clustering of dynamical networks using a saddle-point analysis. IEEE Transactions on Automatic Control, 58(1), 113-124.

1. Sharf, M., & Zelazo, D. (2022, May). Cluster assignment in multi-agent systems. In 2022 13th Asian Control Conference (ASCC) (pp. 947-952). IEEE.