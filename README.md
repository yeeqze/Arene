# Arène – Duels de réponses d'IA

Petite application web où l'on **compare deux réponses d'IA** à la même question et où l'on vote pour la meilleure. Un classement se met à jour après chaque vote.

🔗 **Démo** : https://yeeqze.github.io/NOM-DU-DEPOT/ *(à adapter après la mise en ligne)*

## Pourquoi ce projet ?

Comparer des réponses d'IA en aveugle est une méthode courante pour évaluer des modèles. J'ai voulu comprendre comment ça fonctionne : l'ordre est tiré au sort pour éviter un biais, les noms sont cachés avant le vote, et le classement est calculé à partir des résultats.

## Fonctionnalités

- Duels entre deux réponses, avec **ordre A/B aléatoire**
- Noms des modèles **révélés après le vote**
- Votes : A meilleure, B meilleure, égalité, aucune n'est bonne
- **Classement Elo** recalculé à partir de tous les votes
- Sauvegarde automatique dans le navigateur
- Export des votes et du classement en JSON

## Utilisation

Ouvrir `index.html` dans un navigateur : aucune installation nécessaire.

## Comment fonctionne le score Elo ?

Chaque modèle démarre à 1000 points. Après un duel, le gagnant prend des points et le perdant en perd. Battre un modèle mieux classé rapporte plus de points que battre un modèle plus faible. En cas d'égalité, les scores se rapprochent. Le vote « aucune n'est bonne » n'est pas compté dans le classement.

## Technologies

HTML, CSS et JavaScript (sans framework). Données stockées dans le navigateur (`localStorage`).

## Limites

Les modèles (Alpha, Bêta, Gamma) et leurs réponses sont **fictifs**, écrits pour la démonstration. Avec seulement 5 duels, le classement reste indicatif.

## Ce que j'ai appris

*(À remplir avec tes propres mots : ce que tu as compris du tirage au sort A/B, du score Elo, ce que tu changerais.)*

## Pistes d'amélioration

- Importer ses propres duels depuis un fichier JSON
- Afficher un intervalle de confiance sur le classement
- Ajouter une catégorie par duel (maths, langue, sécurité…)

## Outils utilisés

Projet réalisé avec l'aide d'une IA (Claude), puis relu et compris par mes soins.
