# Cahier des charges — LamyN Theme

## Presentation
Theme CSS personnalise pour Jellyfin, installe sur un NAS Synology DS420+ via Docker.
Le theme est utilise par la famille (acces partage via DDNS).

## Public cible
- Utilisateur principal (admin Jellyfin)
- Membres de la famille (acces invite)

## Objectifs
- Interface sombre avec fond noir pur
- Style cinematographique inspire de Netflix
- Lisibilite et confort visuel
- Compatible desktop, mobile et Chromecast (via app Jellyfin)

## Caracteristiques actuelles (v0.1.0)
- Fond noir pur (#000000)
- Police Inter
- Coins arrondis sur les cartes
- Header avec degradé transparent
- Sidebar avec blur
- Effets de survol sur les cartes
- Boutons stylises
- Barre de progression stylisee
- Scrollbar discrete
- Page de connexion personnalisee
- Compatible responsive (desktop/mobile)

## Evolutions prevues
- Personnalisation des couleurs d'accent (rouge Netflix)
- Zoom au survol des cartes style Netflix
- Header plus compact
- Animations supplementaires

## Contraintes techniques
- CSS pur uniquement (pas de JS)
- Compatible Jellyfin 10.11.x
- Servi via jsDelivr (CDN)
- Pas de dependance externe autre que Google Fonts (Inter)

## Historique des decisions

| Date | Decision | Raison |
|------|----------|--------|
| 2026-04-01 | Fond noir pur (#000) au lieu du bleu-gris | Style Netflix plus fidele |
| 2026-04-01 | Utiliser commit-specific jsDelivr URLs | Cache agressif de @main |
| 2026-04-01 | CSS formate (non minifie) | Maintenabilite et lisibilite |
