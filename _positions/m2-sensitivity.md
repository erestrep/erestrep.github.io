---
layout: page
title: Robust Multi-Robot Coordination -- Sensitivity-Driven Interaction Optimization
description: Open research internship position (stage M2)
img: assets/img/drones_exp.png
importance: 1
category: Master thesis
giscus_comments: true
---

**Short abstract:** The objective of this Master’s thesis is to develop robust connectivity maintenance strategies for multi-robot systems by dynamically optimizing the interconnection weights between robots instead of taking them as fixed functions of the state (as typically done [1]). Using the **closed-loop state sensitivity framework** [2], this work will ensure robustness to **sensing and model uncertainties**—such as bias or gain errors in distance and relative-position measurements—by optimizing the shape and values of interaction weights that govern robot coordination for minimizing a norm of the corresponding sensitivity matrix.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/drones_exp.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Snapshot of an experiment of drone formation using the generalized connectivity model in [1].
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Esteban Restrepo](https://erestrep.github.io/), [Tommaso Belvedere](https://team.inria.fr/rainbow/fr/tommaso-belvedere/), and [Paolo Robuffo Giordano](https://team.inria.fr/rainbow/fr/team/prg/)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [tommaso.belvedere@inria.fr](mailto:tommaso.belvedere@inria.fr) – [prg@irisa.fr](mailto:prg@irisa.fr)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-rob-multi-rob-sens/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description and motivation:** Multi-robot systems rely on dynamic interactions between robots to perform complex collaborative tasks such as distributed exploration or cooperative manipulation. However, real-world sensing and modeling uncertainties—such as measurement bias, sensor noise, and unknown system dynamics—can degrade performance and lead to failures in coordination (collisions, loss of connectivity etc.).
To address these challenges, this master thesis builds upon a **generalized connectivity model** where the interconnection between robots is defined as a product of **weights** that encode factors like **proximity-based interactions** (distance-dependent), **sensing limitations** (field-of-view constraints), **hard constraints** (collision avoidance, connectivity maintenance) and **soft constraints** (formation control, cooperative behavior) [1]. Then, relying on the **closed-loop state sensitivity analysis** [2]​, this thesis will study how to optimize the shape of these interaction weights for **minimizing the multi-robot state sensitivity to sensing and model uncertainties**—such as bias or gain errors in distance and relative-position measurements. The final goal is to ensure a proper coordination of the robots in real-world conditions where models of the robots and measurements can only be approximately known.

**General Objectives:** The goal of this Master Thesis is to formulate inter-robot interactions as a product of dynamically varying weights, incorporating sensing limitations, hard and soft constraints. Then, use the planning and control formalism of closed-loop state sensitivity analysis to optimize the shape and values of the interaction weights to minimize deviations from nominal behavior while maintaining coordination in the presence of sensing uncertainties such as **biases, sensor drifts, and noise**. The proposed algorithms will be **validated through simulations and possibly experiments** using a team of mobile robots.

By integrating **closed-loop sensitivity theory** with dynamic interaction modeling, this thesis will contribute to the development of **next-generation resilient multi-robot systems** capable of operating in real-world, uncertain environments.

<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the experimental setup in the team.

2. Take over the existing works and work on the optimization of interactions in a multi-robot system subject to sensing uncertainties.

3. Implement and validate in simulation the proposed algorithms.

4. Validate experimentally the scenario on a team of mobile robots.

<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation and interest in the topic

* Good knowledge in control theory and robot modeling

* Good experience using Python and Matlab/Simulink

* Basic knowledge of control and analysis of multi-agent systems is appreciated

* Previous experience with C++ and ROS2 is appreciated

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

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-rob-multi-rob-sens/).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Tommaso Belvedere, and Dr. Paolo Robuffo Giordano

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Robuffo Giordano, P., Franchi, A., Secchi, C., & Bülthoff, H. H. (2013). A passivity-based decentralized strategy for generalized connectivity maintenance. The International Journal of Robotics Research, 32(3), 299-323​.

2. Afifi, A., Belvedere, T., Pupa, A., Giordano, P. R., & Franchi, A. (2024). Safe and robust planning for uncertain robots: A closed-loop state sensitivity approach. IEEE Robotics and automation letters.

3. P. Robuffo Giordano, Q. Delamare, A. Franchi. Trajectory Generation for Minimum Closed-Loop State Sensitivity. In IEEE Int. Conf. on Robotics and Automation, ICRA’18, Pages 286-293, Brisbane, Australia, May 2018

4. A. Srour, S. Marcellini, T. Belvedere, M. Cognetti, A. Franchi, P. Robuffo Giordano. Experimental Validation of Sensitivity-Aware Trajectory Planning for a Quadrotor UAV Under Parametric Uncertainty. In Int. Conference on Unmanned Aircraft Systems, ICUAS 2024, Pages 572-578, Chania, Crete, Greece, June 2024

5. S. Wasiela, P. Robuffo Giordano, J. Cortes, T. Simeon. A Sensitivity-Aware Motion Planner (SAMP) to Generate Intrinsically-Robust Trajectories. In IEEE Int. Conf. on Robotics and Automation, ICRA'23, Pages 12707-12713, London, UK, May 2023
