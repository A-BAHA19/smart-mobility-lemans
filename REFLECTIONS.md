# Réflexions — TD2 Smart Mobility Le Mans

## 1. Mes attentes avant de construire le projet

Je pense qu’afficher les retards actuels sera plus simple que déterminer quelles communes ont besoin de davantage de transports. Cette deuxième question me paraît la plus difficile, car la population seule ne permet pas de connaître les déplacements et les besoins réels des usagers.

## 2. Pourquoi ne pas actualiser les données statiques toutes les 15 minutes ?

Je suppose que les horaires prévus, les lignes et les arrêts changent beaucoup moins souvent que les retards. Télécharger ces données toutes les 15 minutes répéterait donc généralement le même traitement sans apporter de nouvelles informations.

## 3. Types des identifiants et jointure des fichiers

Si un même identifiant est interprété comme un nombre dans un fichier et comme du texte dans un autre, la jointure peut échouer ou ne pas retrouver certaines correspondances. Des zéros initiaux peuvent également être perdus si un identifiant est converti en nombre. Lire les identifiants avec dtype=str permet de conserver un type cohérent entre les fichiers.
