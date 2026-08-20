---
layout: page
title: Resilient Coordination of Multi-robot Systems -- Enabling Long-Term Autonomy
description: Open research internship position (stage M2)
img: ms_cbf-resistance.jpeg
importance: 1
category: Master thesis
giscus_comments: true
---

**Short abstract:** Multi-robot teams sustaining long-duration missions must tolerate the loss of individual agents to depleted batteries or faults without the communication network splitting apart. This thesis develops a distributed coordination framework to maintain redundant connectivity that is resilient to agents’ loss to enable long term autonomy. The approach will be validated in simulation and on a real robot fleet in a persistent-mission scenario where agents cycle to a charging station.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ms_cbf-resistance.jpeg" title="resilient" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Esteban Restrepo](https://erestrep.github.io/), [Nicola De Carli](https://www.kth.se/profile/ndc)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [ndc@kth.se](mailto:ndc@kth.se)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-res-coord/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description and motivation:** A multi-robot team relies on communication to function as a team. Robots exchange sensor data, agree on task allocation, hand off responsibilities when one of them withdraws, and remain reachable by a supervisor. Distributed coordination algorithms such as consensus, distributed estimation, task assignment, assume an information path exists between any two agents. When the network splits, that assumption fails as well as the guarantees these algorithms provide. Connectivity is thus a fundamental requirement for coordinated behaviour.

Missions such as environmental monitoring, perimeter surveillance and warehouse logistics run for hours or days, far beyond the endurance of any single platform. A team sustaining such a mission loses and regains members continuously, whether by scheduled recharging or by unplanned failure. In those scenarios, standard connectivity maintenance falls short since it does not certify that the team would stay connected after losing a robot. Long-term autonomy requires redundant connectivity that is resilient to the loss of any single agent.

This thesis will aim to propose a distributed controller to achieve redundant connectivity guarantees using resistance-based graph measures (effective resistance and biharmonic distance [1,2]), which quantify how many independent paths connect two robots. This will be based on two previous results: generalized connectivity maintenance, in which each communication link is modeled by a smooth state-dependent weight encoding range, line-of-sight and field-of-view constraints [3]; and Control Barrier Functions (CBF), which enforce the resulting constraints and compose them with the mission task in a single quadratic program [4–5].


**General Objectives:** 

The student will:

* Formulate robust-connectivity constraints from resistance-based graph measures as control barrier functions, starting from effective resistance and extending to the biharmonic distance.

* Integrate the resulting constraints into a distributed CBF-QP controller alongside a nominal mission task (e.g. area coverage or patrolling).

* Design and validate a persistent-mission scenario in which robots cycle between active duty and a charging station, demonstrating that the departure of any agent leaves the network connected.

* If time allows: extend the framework to explicit join and leave manoeuvres, treating the team population as time-varying and certifying safety through the transition itself.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review and familiarization with the team’s experimental platform.

1. Build on existing work on distributed CBFs and generalized connectivity maintenance; extend the resistance-based formulation.

1. Implement and validate the algorithms in simulation.

1. Experimental validation on a heterogeneous team of mobile robots

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation, scientific curiosity, and genuine interest in graph theory applied to control.

* Good knowledge of control theory and robot modeling; familiarity with algebraic graph theory and multi-agent systems is a plus.

* Previous experience with Python/C++; experience with ROS2 is desirable.

<br>
<hr>
<br>

<h3 class="subsection-title">Conditions</h3>
<br>

Research Internship (M2)

Expected duration of the internship: **5-6 months**

The work will be carried in English at the Centre Inria de l’Université de Rennes research center in Rennes, France.

Financial support offered to the student: 4,50 € / h

<br>
<h3 class="subsection-title">How to apply</h3>
<br>

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-res-coord/).

The position will remain open until a satisfactory candidate is found. In case of positive feedback, you will be contacted. If not positive, you won’t hear back.

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Nicola De Carli

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Ghosh, A., Boyd, S., & Saberi, A. (2008). Minimizing effective resistance of a graph. SIAM review, 50(1), 37-66.

2. Black, M., Lin, L., Nayyeri, A., & Wong, W. K. (2024). Biharmonic distance of graphs and its higher-order variants: Theoretical properties with applications to centrality and clustering. arXiv preprint arXiv:2406.07574.

3. Robuffo Giordano, P., Franchi, A., Secchi, C., & Bülthoff, H. H. (2013). A passivity-based decentralized strategy for generalized connectivity maintenance. The International Journal of Robotics Research, 32(3), 299-323.

4. De Carli, N., Salaris, P., & Giordano, P. R. (2024, May). Distributed control barrier functions for global connectivity maintenance. In 2024 IEEE International Conference on Robotics and Automation (ICRA) (pp. 12048-12054). IEEE.

5. Ames, A. D., Coogan, S., Egerstedt, M., Notomista, G., Sreenath, K., & Tabuada, P. (2019, June). Control barrier functions: Theory and applications. In 2019 18th European control conference (ECC) (pp. 3420-3431). IEEE.

