1. Introduction
Ce projet présente un système SQL permettant de piloter une activité de location de véhicules. L'objectif est de gérer la flotte en temps réel, de suivre les clients et d'analyser les performances commerciales.

2. Structure des données
Le système s'appuie sur quatre tables interconnectées :

Vehicule : Contient les informations techniques (marque, modèle, autonomie), l'état (disponible ou non) et la localisation.

Client : Regroupe l'identité et les contacts des utilisateurs.

Location : Enregistre les transactions, les dates et lie les clients aux véhicules.

Station : Définit les points de départ et d'arrivée.

3. Les axes d'analyse du script

A. Gestion opérationnelle (Filtres)
Les requêtes permettent de répondre aux besoins immédiats du terrain :

Lister les véhicules par ville (exemple : Paris).

Isoler les véhicules immédiatement disponibles.

Identifier les véhicules ayant une forte autonomie (plus de 400 km).

B. Relations et Logistique (Jointures)
L'utilisation des JOIN permet de croiser les informations :

Associer un nom de client à un numéro de contrat.

Identifier précisément le modèle de véhicule loué.

Suivre le trajet d'une location entre la station de départ et la station d'arrivée.

C. Pilotage et Statistiques (Agrégations)
Ces requêtes servent à la prise de décision :

Calculer l'autonomie moyenne de l'ensemble du parc.

Identifier les meilleurs clients (ceux ayant effectué au moins 2 locations).

Repérer les véhicules qui n'ont jamais été loués (audit de rentabilité).

Déterminer les zones géographiques les plus actives.

4. Conclusion
Ce script offre une vision complète de l'activité. Il permet de passer d'une simple liste de données à un véritable outil d'aide à la décision pour optimiser la gestion de la flotte.
