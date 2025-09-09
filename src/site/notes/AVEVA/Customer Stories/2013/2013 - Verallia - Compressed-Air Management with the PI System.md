---
{"Title":"2013 - Compressed-Air Management with the PI System","Year":2013,"Industry":"Glass","URL":"https://resources.osisoft.com/presentations/compressed-air-management-with-the-pi-system/","PDF":"https://cdn.osisoft.com/corp/en/media/presentations/2013/EMEA2013/PDF/EMEA13_Verallia_BaptistaTurck_DeploymentOfThePDHInfrastructureAtVerallia.pdf","Company":"Verallia","Keywords":["Furnace","France"],"dg-publish":true,"permalink":"/aveva/customer-stories/2013/2013-verallia-compressed-air-management-with-the-pi-system/","dgPassFrontmatter":true}
---

#### PRESENTATION

## 2013 - EMEA Users Conference - Paris

### Compressed-Air Management with the PI System

Saint-Gobain Verallia is a French glass manufacturer that produces glass bottles and pots. One of the Verallia plants' main energy costs comes from compressed air consumption. Using the PI System as the base for a pilot project, Saint-Gobain initiated the PDH project to monitor compressed air usage in an effort to reduce energy consumption costs. This presentation discusses the PDH project and how it enabled the company to fine tune their central infrastructure strategy and decide on the right PI System client tools for their users.

---
# Gestion de l’air comprimé chez Verallia avec le système PI

## Introduction
- Verallia est une filiale du groupe Saint-Gobain, spécialisée dans la fabrication de bouteilles et bocaux en verre
- Présence mondiale avec environ 40 usines, produisant 25 milliards d’unités par an.
- Processus industriel continu : les fours ne peuvent jamais s’arrêter, ce qui impose un suivi énergétique rigoureux.
    

## Projet PDH (Process Data Historian)
- Objectif principal : centraliser la collecte, le stockage et la publication des données industrielles.
- Un système PI unique global est déployé, remplaçant les multiples serveurs locaux par usine.
- Ce système fournit des données brutes en temps réel aux utilisateurs : opérateurs comme direction.

## Application pilote : surveillance des compresseurs d’air
- L’air comprimé est le 2ème ou 3ème poste de dépense énergétique dans les usines.
- Avant, la collecte de données était manuelle, dispersée sur plusieurs systèmes (ex : SAP, Seal, Excel).
- Installation de capteurs sur les compresseurs pour collecte automatique des données via PI Interface Nodes.
- Rapports générés automatiquement, avec une fréquence élevée (5 à 10 secondes), contre des rapports hebdo/mensuels auparavant.
- Visualisation en temps réel pour les opérateurs, une première dans ces usines.
    

## Résultats et apprentissages
- Identification de surconsommations d’air allant jusqu’à 2 à 3 fois le théorique sur certains compresseurs.
- Mauvaise configuration des systèmes de commande des compresseurs détectée, alors que la maintenance affirmait tout en ordre.
- Non-respect des procédures par les opérateurs, par exemple les compresseurs restent allumés plusieurs jours lors de changements de production.
- Ces observations ouvrent des possibilités d’économies substantielles.
- Importance capitale d’agir sur les données collectées : sans actions correctives, pas de retour sur investissement.
    

## Outils et déploiement applicatif

- Utilisation de ProcessBook pour la création d’écrans de supervision, et Data Link pour la génération de rapports Excel.
- Difficultés rencontrées :
    - Trop de développements en VB rendaient les applications lentes et difficiles à maintenir.
    - Difficile de standardiser à l’échelle globale à cause des différences locales (nombre de compresseurs etc.).
- Passage progressif vers des applications web, dynamiques et centrées sur une architecture modulaire avec PI AF SDK.
- But : faciliter la maintenance, la rapidité de déploiement, et permettre aux usines locales de créer leurs propres applications selon leurs besoins.
    

## Intégration business
- Utilisation de Business Objects pour croiser les données techniques avec les coûts financiers SAP.
- Permet aux responsables de visualiser directement le coût énergétique en euros par usine.
- Centralisation des rapports industriels et financiers dans un seul système global.
    

## Stratégie organisationnelle
- Approche hybride :
    - Centralisation des applications globales et standardisées.
    - Liberté laissée aux usines locales de développer des solutions spécifiques via ProcessBook pour besoins particuliers.
- Formation des équipes R&D et opérationnelles à l’utilisation de Data Link, pour qu’elles construisent elles-mêmes leurs rapports personnalisés.
- Pas de support centralisé pour les applications locales, donc priorité à la simplicité et l’autonomie.
    

## Conclusion
- Projet jeune (1 an et demi), déjà vecteur d’innovations dans la gestion énergétique.
- Collecte et analyse des données automatisées, ouvrant la voie à des économies d’énergie importantes.
- Prochain enjeu : transformer les analyses en actions concrètes pour maximiser le retour sur investissement.
- Renforcement continu de l’outil et évolution vers des solutions web modernes pour accompagner la croissance et la standardisation.