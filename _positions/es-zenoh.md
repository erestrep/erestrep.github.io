---
layout: page
title: Plateforme expérimentale multi-robots hétérogènes : communication décentralisée P2P avec Zenoh
description: Stage de fin d’études, parcours ingénieur (Bac+5)
img: es_zenoh.jpeg
importance: 2
category: Master thesis
giscus_comments: true
---

**Résumé :** Ce stage vise à doter la plateforme expérimentale multi-robots de l’équipe Rainbow (robots terrestres et drones) d’une couche de communication peer-to-peer et décentralisée, fondée sur le protocole de communication Zenoh. L’enjeu est de permettre l’exécution d’algorithmes de commande distribuée dans des conditions réelles, sur une flotte hétérogène d’une dizaine de robots. Stage à dominante ingénierie logicielle et systèmes robotiques ; le code sera publié en open source.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/es_zenoh.jpeg" title="zenoh" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<hr>

**Equipe :** [Rainbow team](https://team.inria.fr/rainbow/) IRISA/Inria Rennes, France

**Encadrants :** [Esteban Restrepo](https://erestrep.github.io/), [Gianluca Corsini](https://team.inria.fr/rainbow/team/gianluca-corsini/)

**Contact :** [esteban.restrepo@irisa.fr](mailto:esteban.restrepo@irisa.fr) – [gianluca.corsini@irisa.fr](mailto:gianluca.corsini@irisa.fr)

**Comment candidater :** Les candidats intéressés sont priés de postuler via [ce formulaire](https://team.inria.fr/rainbow/appl-form-zenoh/).

<hr>

<br>

**Description and Objectifs :** L’équipe RAINBOW développe des stratégies de commande distribuées pour systèmes multi-robots, toutes fondées sur une même hypothèse : chaque robot ne calcule qu’à partir de l’information de ses voisins immédiats. Cependant, en pratique, ces algorithmes sont le plus souvent validés depuis un ordinateur central disposant de l’état global, ce qui ne dit rien de la robustesse aux latences, aux pertes de paquets et aux commutations de topologie réelles. Ce stage a pour but de supprimer cet écart.

L’équipe dispose de 10 robots terrestres (DJI RoboMaster modifiés, calculateur embarqué LattePanda Sigma), 10 Crazyflie 2.1, 10 Crazyflie 2.1 Brushless, de quadrotors plus grands, de deux salles de capture de mouvement (Vicon, Qualisys) et de divers équipements pour les Crazyflie (recharge sans fil, caméras embarquées, flow deck, AI deck).

Pour atteindre l’objectif du stage, le premier obstacle à surmonter est l’hétérogénéité. Les RoboMaster tournent sous Linux et peuvent exécuter un pair Zenoh nativement. Les Crazyflie reposent sur une architecture bi-microcontrôleur sans pile IP, dont toute communication transite par un dongle Crazyradio : leur pair Zenoh sera donc déporté au sol, sous forme de processus indépendant et sans état partagé, à raison d’un par drone. Un algorithme distribué devra pouvoir s’exécuter sans savoir sur quel type de robot il tourne.

Le deuxième obstacle concerne le voisinage des robots. Zenoh met par défaut tous les pairs en relation, ce qu’un algorithme distribué ne doit précisément pas avoir à disposition. Il s’agit donc de développer une couche restreignant dynamiquement les échanges au voisinage effectif de chaque robot (portée de communication, apparition et rupture de liens, topologie commutante), conçue autour d’une interface abstraite de « fournisseur de voisinage » alimentable aussi bien par la capture de mouvement que par la localisation relative décentralisée.


**Objectifs :** 

* Concevoir l’architecture de communication : espace de nommage, modèle de données (type de messages en fonction du type de robot), découverte, etc.

* Implémenter la bibliothèque : un pair Zenoh par robot, sans processus maître ; intégration à l’existant (ROS 2, Crazyswarm2 / cflib).

* Développer la couche de contrainte de voisinage et son interface de fournisseur de voisinage.

* Instrumenter la plateforme : mesure de latence, débit et pertes par lien, tests automatisés, lancement reproductible d’une expérience à N robots.

* Valider par la démonstration d’un algorithme distribué (consensus, estimation de connectivité) sur une flotte hétérogène d’une dizaine de robots, terrestres et aériens simultanément.

* Livrer une bibliothèque documentée, avec exemples et tutoriels destinés aux doctorants et chercheurs, publiée en open source.

<br>
<h3 class="subsection-title">Activités envisagées</h3>
<br>

1. Prise en main de la plateforme (ROS 2, Crazyswarm2 / cflib, capture de mouvement) et de Zenoh ; état des lieux de l’existant.

1. Conception de l’architecture et prototype.

1. Développement de la couche de contrainte de voisinage et des outils de mesure.

1. Mise en place et caractérisation des performances et des limites de dimensionnement.

1. Démonstration expérimentale, documentation, tests, publication du code.

Des activités optionnelles, abordées une fois les objectifs principaux atteints, peuvent inclure : appui aux expériences des doctorants ; mise en service des stations de recharge sans fil ; intégration de nouveaux capteurs embarqués ; étude de faisabilité de zenoh-pico sur le module WiFi de l’AI deck.

L’architecture retenue conditionnera les expérimentations de l’équipe pour plusieurs années. Le stage offre une réelle responsabilité technique, un travail au contact direct des doctorants, une pratique approfondie des systèmes distribués appliqués à la robotique, et une contribution open source visible dans l’écosystème ROS 2 / Zenoh.

<br>
<h3 class="subsection-title">Compétences requises</h3>
<br>

**Indispensables**

* Bonne maîtrise du C++ et/ou de Python sous Linux, avec Git ;

* Notions solides de réseaux et de systèmes distribués (publication/souscription, découverte, UDP/TCP, multicast) ;

* Connaissances de base de ROS 2 ;

* Goût pour le travail expérimental sur robots réels ;

* Autonomie et capacité à produire du code documenté et testé, destiné à être repris par d’autres ;

* Capacité à travailler en anglais.

**Appréciées**

* Connaissance de Zenoh, de DDS ou d’un autre protocole de communication en robotique ;

* Expérience des systèmes embarqués et des microcontrôleurs ;

* Expérience de l’écosystème Crazyflie (Crazyswarm2, cflib) ou de PX4 ;

<br>
<hr>
<br>

<h3 class="subsection-title">Conditions</h3>
<br>

Stage de fin d’études, parcours ingénieur (Bac+5)

Durée prévue du stage: **5-6 mois**

Les travaux se dérouleront en anglais/français au Centre de recherche Inria de l’Université de Rennes, France.

Gratification de stage : 4,50 €/h

<br>
<h3 class="subsection-title">Comment candidater</h3>
<br>

Les candidats intéressés sont priés de postuler via [ce formulaire](https://team.inria.fr/rainbow/appl-form-zenoh/).

Le poste restera vacant jusqu’à ce qu’un candidat retenu soit trouvé. Si votre candidature est retenue, vous serez contacté(e). Dans le cas contraire, vous ne recevrez pas de réponse.

**Encadrants :** Dr. Esteban Restrepo, Dr. Gianluca Corsini


