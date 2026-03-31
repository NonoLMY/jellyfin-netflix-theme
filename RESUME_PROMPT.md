# LamyN Theme — Prompt de reprise

> Pour reprendre le travail sur ce projet, dites a Claude Code :
>
> "Bonjour, je reprends le projet LamyN Theme. Lis RESUME_PROMPT.md et dis-moi ou on en est."

## Etat actuel
- **Version** : v0.1.0
- **Phase** : Personnalisation des couleurs (Phase 1)
- **Derniere session** : 1er avril 2026

## Ce qui a ete fait
- Theme CSS complet recupere, formate et nettoye (3350+ lignes)
- Fond noir pur (#000000) applique
- Commentaires de section ajoutes
- Toute reference a l'ancien theme supprimee
- Header standard du projet ajoute au CSS
- Projet initialise avec /init (docs, CHANGELOG, README, etc.)
- Repo GitHub : https://github.com/NonoLMY/jellyfin-netflix-theme

## Prochaines etapes
- [ ] Appliquer les couleurs d'accent rouge Netflix (#e50914)
- [ ] Ajouter les effets de survol style Netflix (zoom, ombre, overlay)
- [ ] Header compact et transparent
- [ ] Tester sur differents appareils

## Fichiers cles
- `theme-netflix.css` — Le theme CSS (fichier principal et unique livrable)
- `docs/cahier-des-charges.md` — Specifications du theme
- `docs/TODO.md` — Liste des taches
- `CHANGELOG.md` — Historique des versions
- `CLAUDE.md` — Regles de travail

## Points techniques importants
- Jellyfin 10.11.6 sur Synology DS420+ (Docker)
- Le CSS est servi via jsDelivr — TOUJOURS utiliser des URLs avec commit hash (@hash), pas @main
- Le champ CSS dans Jellyfin est dans : Tableau de bord > Slogan > Code CSS personnalise
- Les variables --jf-palette-* de Jellyfin ne sont pas overridables facilement depuis :root
- Les selecteurs directs (.backgroundContainer, .cardPadder, .countIndicator, etc.) fonctionnent bien

## Decisions en attente
- Choix definitif de la couleur d'accent (rouge Netflix #e50914 ou autre ?)
- Niveau de zoom au survol des cartes
