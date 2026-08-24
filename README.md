# Illustrations

Miroir des illustrations utilisées par
[pokemoncardsmosaic](https://github.com/ArielNora/pokemoncardsmosaic), une
application qui assemble des illustrations de cartes Pokémon en une mosaïque
dont les bords se raccordent, destinée à l'impression.

Ce dépôt ne contient pas de code. Il n'existe que pour héberger les archives,
publiées en *release* : une par extension.

## Contenu

441 illustrations en 22 archives, 56,4 Mo au total. Format 734x1024, WebP
qualité 80.

Ce sont les illustrations seules, telles que le jeu les affiche sous le cadre :
sans bordure, sans texte, sans logo.

## Utilisation

Rien à télécharger à la main, et un `git clone` ne suffit pas : les fichiers
d'une *release* ne sont pas dans git. L'application s'en charge.

```bash
git clone https://github.com/ArielNora/pokemoncardsmosaic.git
cd pokemoncardsmosaic
uv run python scripts/fetch_cards.py
```

Le manifeste `cards.json` du dépôt principal décrit les 441 illustrations, avec
leur chemin, leur taille et leur empreinte SHA-256. Le script vérifie chaque
archive, puis chaque image, avant de l'écrire.

Pour prendre les archives sans passer par l'application :

```bash
gh release download cards-v3 --repo ArielNora/pokemoncardsmosaic-images
```

## Droits

Les illustrations appartiennent à **The Pokémon Company International,
Nintendo, Creatures Inc.** et **GAME FREAK Inc.**, ainsi qu'aux illustrateurs
qui les ont réalisées.

Elles sont rassemblées ici pour un usage personnel et non commercial : un projet
d'impression sans but lucratif. Aucune revendication de propriété n'est faite
sur ces images.

Sur demande d'un ayant droit, ce dépôt sera retiré sans discussion. Ouvrez une
*issue* ou écrivez-moi.
