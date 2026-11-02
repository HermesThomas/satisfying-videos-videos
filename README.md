# satisfying-videos-videos

Repository public pour les vidéos générées par l'algorithme **bouncing_balls_v4**.

## Algorithme

**bouncing_balls_v4.py** — Une seule balle dans un cercle, physique réaliste :
- Gravité + coefficient de restitution (>1 pour récupérer de l'énergie à chaque rebond)
- La balle rebondit sur le BORD du cercle (contact boule-cercle) sans jamais le traverser
- Fond noir, générations satisfaisantes et addictives

## Génération

Voir le repo [satisfying-videos](https://github.com/HermesThomas/satisfying-videos) pour le code source et les instructions de génération.

### Commande

```bash
python generate.py --config config/bouncing_ball_v4_seed_101.json --output videos/bouncing_ball_v4_seed_101.mp4
```

### Vidéos disponibles

- `bouncing_ball_v4_seed_101.mp4` — Cercle bleu `#3b82f6`, balle rouge `#ef4444`
- `bouncing_ball_v4_seed_202.mp4` — Cercle vert `#22c55e`, balle bleue `#3b82f6`
- `bouncing_ball_v4_seed_303.mp4` — Cercle jaune `#f59e0b`, balle pourpre `#a855f7`

## Validation

La trace de la balle (positions à chaque frame) est enregistrée dans `logs/coord_log.json`. Le fichier `test_v4_physics.py` vérifie que la balle ne traverse pas le cercle.

## Licence

Code source dans le repo [satisfying-videos](https://github.com/HermesThomas/satisfying-videos) (private), vidéos dans ce repo (public).
