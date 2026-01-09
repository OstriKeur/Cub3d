# cub3d

Raycasting 3D avec la MLX - Projet 42 Paris

## À propos

Cub3D est un projet de raycasting 3D inspiré de Wolfenstein 3D. Il faut créer un moteur 3D basique en utilisant la technique du raycasting pour afficher une vue en première personne.

C'est un projet graphique avancé qui combine mathématiques et programmation graphique. J'ai appris à implémenter un moteur de rendu 3D basique, gérer les textures, et créer une expérience de jeu interactive.

## Compilation

```bash
make
```

Cela génère l'exécutable `cub3d`.

## Utilisation

```bash
./cub3d maps/good/map.cub
```

## Contrôles

- **WASD** : déplacer le joueur
- **Flèches gauche/droite** : tourner la caméra
- **ESC** : quitter le jeu
- **Souris** : rotation de la caméra (si activé)

## Fonctionnalités

- Raycasting pour le rendu 3D
- Textures sur les murs
- Gestion des sprites
- Parsing de fichiers de configuration (.cub)
- Validation de la map
- Gestion des collisions
- Mouvements fluides

## Structure du projet

```
cub3d/
├── src/              # Code source principal
│   ├── main.c
│   ├── rendering/    # Moteur de rendu et raycasting
│   ├── moves/        # Gestion des mouvements
│   ├── parsing/      # Parsing des fichiers .cub
│   ├── map/          # Validation et gestion de la map
│   └── config/       # Configuration du jeu
├── inc/              # Headers et bibliothèques
│   ├── libft/        # Bibliothèque C personnalisée
│   └── mlx/          # MiniLibX
├── maps/             # Fichiers de map d'exemple
└── textures/         # Textures pour les murs et sprites
```

## Ce que j'ai appris

- Raycasting et mathématiques 3D
- Calcul de distances et intersections
- Gestion de textures et sprites
- Parsing de fichiers de configuration complexes
- Validation de maps avec algorithmes de flood fill
- Optimisation du rendu pour de bonnes performances
- Gestion d'événements clavier et souris avec MLX

## Format de fichier .cub

Le fichier de configuration contient :
- Résolution de la fenêtre
- Chemins vers les textures (N, S, E, W)
- Couleurs du sol et du plafond
- La map avec les caractères : 0 (sol), 1 (mur), N/S/E/W (joueur), etc.

---

**Projet réalisé dans le cadre du cursus 42 Paris**
