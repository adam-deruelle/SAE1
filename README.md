# 🛠️ SAÉ 1 – Variateur de lumière sans contact

## 🎯 Objectif du projet

Concevoir et tester un variateur de lumière sans contact permettant de faire varier l’intensité lumineuse d’un ruban LED ou d’une lampe LED monochrome. Deux modes sont proposés :
- **Mode manuel** : commande par capteurs infrarouges (IR) "plus" et "moins"
- **Mode automatique** : réglage automatique en fonction de la luminosité ambiante

## 🧩 Contexte

Le projet s’inscrit dans un scénario fictif : après un incendie dans l’entreprise "France LED", les schémas de la nouvelle version du variateur ont été perdus. En tant qu’étudiant à l’IUT GEII, nous avons été sollicités pour recréer et tester un prototype fonctionnel à partir des rares documents récupérés.

## 🧠 Analyse de l’existant

À partir du boîtier d’un ancien variateur :
- Alimentation en 12V continue
- Éclairage supporté : jusqu’à 8A
- Utilisation d’un potentiomètre pour moduler la tension

## 📐 Conception de la carte

### Schéma structurel
La carte se compose de :
- Un **connecteur 12V**
- Un **convertisseur de tension 12V → 5V** (LM2576)
- Un **capteur de lumière** (TEMT6000)
- Deux **capteurs infrarouge TCRT5000**
- Un **microcontrôleur PIC16F18446**
- Un **MOSFET IRF520** pour la gestion de puissance
- Divers points de test (TP1 à TP11) pour la validation

### Logiciel utilisé
- [Proteus](https://www.labcenter.com/) pour la CAO (schéma + routage PCB)

## 🧪 Tests réalisés

### 🔍 Contrôle visuel
- Vérification de la présence, polarité, valeur et qualité de soudure des composants
- Évaluation du respect des contraintes de placement et de dimensions

### 📊 Tests fonctionnels
- Test de l'interrupteur général
- Vérification des tensions d’entrée (12V) et sortie régulée (5V)
- Mesures des signaux aux points de test TP1 à TP7
- Comportement des capteurs IR et de la LED témoin

> Résultat : tous les tests sont **conformes** aux attentes du cahier des charges.

## 📝 Conclusion

Ce projet nous a permis d’explorer l’ensemble du cycle de vie d’un produit électronique :
- Analyse et compréhension d’un produit existant
- Reconstitution du schéma et modélisation sous Proteus
- Fabrication manuelle de la carte
- Mise en place de tests rigoureux (visuels et fonctionnels)

Nous avons ainsi acquis des compétences solides en **CAO**, **montage électronique**, et **procédures de vérification**.

---

> 🧾 _Projet réalisé par Antoine Conty & Adam Deruelle – GEII – IUT de Rennes_
