COMPTE RENDU

Hugo 
PELISSIER 
https://github.com/hugopelissier9-rgb/cc-ateliers-musees.git

Branches et modifications
main : branche principale avec toutes les étapes intégrées.
feat/theme-sombre : thème nocturne, avec le fond #17223b, le texte blanc et la couleur d’accent #e63946.
feat/confirmation-reservation : activation du message après une réservation.
hotfix/lisibilite-confirmation : ajout d’un panneau de confirmation contrasté.
feat/nom-atelier : ajout du nom "Fabriquez un objet inutile" au message.

Le depart-cc désigne le point de départ commun : 67aeb4f.

Tests réalisés

| Étape | Action | Résultat vérifié |
| Chargement | Ouvrir ou actualiser la page | Compteur à 0 et confirmation masquée |
| Première réservation | Cliquer sur « Réserver une place » | Compteur à 1 et confirmation avec le nom de l’atelier |
| Trois réservations | Réserver trois places | Compteur à 3 et confirmation indiquant 3 places |
| Remise à zéro | Cliquer sur « Recommencer » | Compteur à 0 et confirmation masquée |
| Réservation après remise à zéro | Réserver une place | Compteur à 1 et confirmation visible |
| Affichage mobile | Tester avec une largeur de 390 px | Pas de défilement horizontal ; largeur du contenu mesurée à 375 px |

Hotfix:
Après les évolutions A et B, le texte de confirmation avait encore la couleur sombre #17223b sur le fond sombre de la page. Le hotfix l’a remplacé par un panneau de fond #263859, avec un texte blanc et une bordure #e63946.

Réponses aux questions:
1. Base et branches
Les branches A et B partent toutes deux de depart-cc (67aeb4f). Le hotfix part de main après l’intégration de A et B (18411b7). La branche feat/nom-atelier part de main après l’intégration du hotfix (bfdf807). Ces étapes sont visibles avec git log, --graph, --oneline et --all.

2. Fusion et fonctionnement:
Une fusion sans conflit signifie que Git a pu combiner les modifications. Elle ne garantit pas que le résultat fonctionne ou reste lisible. Il faut aussi tester le site dans un navigateur. Ici, le hotfix corrige le contraste du message après l’évolution vers le thème sombre.

3. Commit et publication:
Un commit est enregistré dans le dépôt local. Il n’est pas automatiquement publié sur GitHub. Il faut configurer un dépôt distant, puis envoyer les commits avec git push. Aucun dépôt distant n’est configuré actuellement pour ce projet.

Aides utilisées:
IA utilisée pour la compréhension du tp, vérifier les codes et pour le css (pas tout).
Navigateur pour certains oublis.
