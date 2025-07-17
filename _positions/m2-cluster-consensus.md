---
layout: page
title: Cluster-consensus control of teams of robotic vehicles for dosimetry
description: Open research internship position (stage M2)
img: assets/img/phd_cluster.png
importance: 3
category: closed
giscus_comments: true
---

**Short abstract:** The goal of this Master Thesis is to setup an experimental testbed for a heterogeneous multi-robot system and to design and analyse distributed control laws to achieve autonomous formation of clusters in a group of heterogeneous mobile robots in order to perform measurement and sensing of electromagnetic radiation (dosimetry).

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

**Advised by:** [Esteban Restrepo](https://erestrep.github.io/), [Dr. Gianluca Corsini](https://team.inria.fr/rainbow/fr/team/gianluca-corsini/), and [Antonio Marino](https://team.inria.fr/rainbow/fr/antonio-marino/)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [gianluca.corsini@irisa.fr](mailto:gianluca.corsini@irisa.fr) – [antonio.marino@irisa.fr](mailto:antonio.marino@irisa.fr)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-int-clus-cons/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description:** The deployment of teams of robotic vehicles has been shown to be effective for a wide range of applications based on cooperative tasks such as reconnaissance, surveillance, foraging, search and rescue and active sensing. Most of the time, in such collaborative missions, such as dosimetry, the field of interest is relatively large with respect to the size of the multi-robot system. Therefore, the heterogeneous team must be divided into smaller groups (clusters), based on the task (the electromagnetic field to measure) or the robots capabilities (sensors, mobility), in order to perform the mission successfully.

**Motivations:** Most of the current works addressing the problem of clustering for multi-agent systems are concerned with generic unconstrained agents, thus neglecting the constraints and specificity of networks of mobile robots in terms of limited sensing capabilities. Moreover, they only study the conditions for convergence of the agents to small groups, i.e. cluster consensus, rather than the autonomous formation of clusters. There are few works addressing the autonomous achievement of clusters in a network of heterogeneous mobile robots based on distributed and local interactions among the robots, none of which take also into account the sensing constraints inherent to these types of systems.

**General Objectives:** The goal of this Master Thesis is twofold: 1. Design and validate theoretically (using Lyapunov methods, graph theory, etc.) novel distributed control laws for the autonomous achievement of cluster consensus of a team of heterogeneous robotic vehicles subject to sensing constraints (limited range, limited field of view) based on the general connectivity framework in [1]; 2. Setup an experimental testbed for heterogeneous (aerial/ground) multi-robot systems based on the Cambridge RoboMaster platform [2] and Crazyflie drones [3] to test and validate the algorithms both in simulation and experiments.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the experimental setup in the team

1. Take over the existing works and work on the design and analysis of a control algorithm for autonomous cluster consensus of heterogeneous multi-robot systems

1. Setup the hardware and software for a team of heterogeneous aerial/ground robots 

1. Implement and validate in simulation the proposed algorithms

1. Validate experimentally the scenario on the heterogeneous team of robots

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation and interest in the topic

* Good experience with robotics hardware and software (Python/C++ and ROS2)

* Knowledge in control theory and robot modeling

* Basic knowledge of control and analysis of multi-agent systems is appreciated

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

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-int-clus-cons/).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Gianluca Corsini, and Antonio Marino

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Robuffo Giordano, P., Franchi, A., Secchi, C., & Bülthoff, H. H. (2013). A passivity-based decentralized strategy for generalized connectivity maintenance. The International Journal of Robotics Research, 32(3), 299-323.

1. Blumenkamp, J., Shankar, A., Bettini, M., Bird, J., & Prorok, A. (2024). The cambridge robomaster: An agile multi-robot research platform. arXiv preprint arXiv:2405.02198.

1. https://store.bitcraze.io/collections/platforms/products/crazyflie-2-1-plus

1. Xia, W., & Cao, M. (2011). Clustering in diffusively coupled networks. Automatica, 47(11), 2395-2405.

1. Zhang, Z., Wu, W., & Zhang, F. (2024). Opinion-based Task Allocation Strategy for Mobile Sensor Networks. American Control Conference, 1-6.

1. Menara, T., Baggio, G., Bassett, D. S., & Pasqualetti, F. (2019). Stability conditions for cluster synchronization in networks of heterogeneous Kuramoto oscillators. IEEE Transactions on Control of Network Systems, 7(1), 302-314.

1. Burger, M., Zelazo, D., & Allgower, F. (2012). Hierarchical clustering of dynamical networks using a saddle-point analysis. IEEE Transactions on Automatic Control, 58(1), 113-124.

1. Sharf, M., & Zelazo, D. (2022, May). Cluster assignment in multi-agent systems. In 2022 13th Asian Control Conference (ASCC) (pp. 947-952). IEEE.
