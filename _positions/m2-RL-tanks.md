---
layout: page
title: RL-driven Energy Tanks for Aerial Physical Interaction
description: Open research internship position (stage M2)
img: assets/img/pushing-drone.png
importance: 1
category: closed
giscus_comments: true
---

**Short abstract:** This goal of this Master's Thesis is to combine Reinforcement Learning with Passivity-Based Control to enable safe Aerial Physical Interaction. The proposed system autonomously tunes rechargeable energy tanks, allowing a fully actuated UAV to perform robust 'push-and-slide' contact tasks in uncertain environments.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/pushing-drone.png" title="cluster image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Snapshot of a push-and-slide experiment with a fully-actuated hexarotor at IRISA.
</div>

<hr>

**Hired by** the [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Advised by:** [Esteban Restrepo](https://erestrep.github.io/), [Cristian Secchi](https://www.arscontrol.unimore.it/cristian-secchi/), [Marco Tognon](https://marco-tognon-robotics.com/), [Paolo Robuffo Giordano](https://team.inria.fr/rainbow/fr/team/prg/)

**Contact:** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [csecchi@unimore.it](mailto:csecchi@unimore.it) – [marco.tognon@inria.fr](mailto:marco.tognon@inria.fr)  – [prg@irisa.fr](mailto:prg@irisa.fr)

**How to apply:**  Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-rl-energy-tanks/). The position will remain open until a satisfactory candidate is found.

<hr>

<br>

**Description and motivation:** For a standard drone, touching the environment is usually a prelude to a crash. However, the next generation of UAVs must do more than just look; they must interact—perform contact inspection, industrial cleaning, or manipulation. This field, **Aerial Physical Interaction (APhI)**, faces a critical problem: contact dynamics are nonlinear and unpredictable. 

To prevent instability during contact, we use **Passivity-Based Control** with **Virtual Energy Tanks**. Think of the "Energy Tank" as a virtual battery that monitors the system's energy flow. If the drone behaves aggressively (injecting too much energy), the tank drains to limit the control action, guaranteeing mathematical stability [1]. While Energy Tanks ensure safety, tuning them is notoriously difficult. A tank that is too conservative makes the drone sluggish and unable to push hard enough to do its job. A tank that is too aggressive might drain empty mid-task, causing the drone to freeze. Furthermore, in unknown environments, fixed parameters fail.

This thesis proposes a hybrid approach: AI-tuned Control. Instead of manually tuning the tank, we will train a **Reinforcement Learning (RL)** agent to act as a "supervisory pilot." The RL agent will observe the robot’s state and interaction forces in real-time and dynamically adjust the rechargeable energy tank's parameters (capacity, refill rate). This allows the UAV to be compliant when necessary and stiff when pushing, optimizing performance without ever sacrificing the safety guarantee provided by the passivity layer.

The algorithms will be tested on a Fully Actuated UAV (a drone capable of independent translation and rotation, allowing it to exert precise lateral forces) performing a **"Push-and-Slide" mission**—continuously maintaining force against a surface while sliding along it.

**General Objectives:** The goal of this Master's Thesis is to design an RL-based energy policy that autonomously tunes a rechargeable energy tank to maximize interaction performance while guaranteeing passivity. The student will:

* Implement a control architecture that couples a passivity-based controller (the safety layer) with a Reinforcement Learning agent (the optimization layer).
* Design the reward functions and state-space to train the agent to recognize when to replenish the tank and when to conserve energy during contact.
* Validate the approach in a physics simulator (e.g., Gazebo) on a fully actuated UAV model, demonstrating that the RL-tuned tank outperforms a static tank in a "push-and-slide" scenario against surfaces with varying friction/stiffness.


<br>
<h3 class="subsection-title">Envisaged activities</h3>
<br>

1. Literature review of the related works and familiarize with the experimental setup in the team.

1. Implement in simulation and experimentally a push-and-slide task with the rechargeable energy tank framework.

1. Take over the existing works and propose an RL-based strategy for parameter learning.

1. Implement and validate in simulation the proposed algorithms.

1. Validate experimentally the scenario on a fully actuated UAV.


<br>
<h3 class="subsection-title">Skills/Requirements</h3>
<br>

* High motivation and interest in the topic

* Knowledge in control theory and robot modeling

* Knowledge in Reinforcement Learning

* Previous experience with Python/C++

* Previous experience with ROS2 is desirable

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

Interested candidates are requested to apply via [this form](https://team.inria.fr/rainbow/appl-form-rl-energy-tanks/).

**Supervisor(s):** Dr. Esteban Restrepo, Dr. Cristian Secchi, Dr. Marco Tognon, Dr. Paolo Robuffo Giordano

<br>
<h3 class="subsection-title">References</h3>
<br>

1. Califano, F., Rashad, R., Secchi, C., & Stramigioli, S. (2022, September). On the use of energy tanks for robotic systems. In International Workshop on Human-Friendly Robotics (pp. 174-188). Cham: Springer International Publishing.

2. Benzi, F., Brunner, M., Tognon, M., Secchi, C., & Siegwart, R. (2022). Adaptive tank-based control for aerial physical interaction with uncertain dynamic environments using energy-task estimation. IEEE Robotics and Automation Letters, 7(4), 9129-9136.

3. Zanella, R., Califano, F., Secchi, C., & Stramigioli, S. (2024, March). Learning Passive Policies. In European Robotics Forum (pp. 338-343). Cham: Springer Nature Switzerland.

4. Sacerdoti, D., Benzi, F., & Secchi, C. (2024, May). A reinforcement learning-based control strategy for robust interaction of robotic systems with uncertain environments. In 2024 IEEE International Conference on Robotics and Automation (ICRA) (pp. 5788-5794). IEEE.

