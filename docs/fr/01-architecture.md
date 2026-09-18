# 1. Architecture — libsecp256k1

Ce dépôt rassemble les composants de référence consacrés à les opérations cryptographiques optimisées sur la courbe secp256k1 utilisées par Bitcoin.
La lecture commence par le README, puis suit les modules de production et leurs interfaces publiques.
Les répertoires séparent le cœur du protocole, les outils d’intégration et les scénarios de vérification.
Chaque couche possède ses propres types, règles d’état et frontières de confiance.
Les entrées externes sont transformées en opérations internes avant de modifier l’état persistant.
Les erreurs et événements rendent visibles les refus et les transitions importantes.
Les bibliothèques partagées évitent de dupliquer les primitives communes entre composants.
Cette architecture doit être lue avec les choix de configuration propres à chaque déploiement.

[Chapitre suivant : Clés, signatures ECDSA et vérification](02-cles-signatures-ecdsa-et-verification.md)
