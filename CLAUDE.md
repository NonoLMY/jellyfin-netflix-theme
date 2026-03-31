# Regles du projet — LamyN Theme

## Methode de travail
- Toujours utiliser le mode plan avant de modifier le CSS de maniere significative
- L'utilisateur n'est pas developpeur : explications claires, pas de jargon
- Ne jamais modifier le CSS sans validation prealable

## Qualite
- Fichier CSS formate et lisible (pas de minification en dev)
- Commentaires de section pour organiser le code
- Variables CSS centralisees dans :root
- Compatibilite Jellyfin 10.11.x

## Documentation
- Mettre a jour TOUS les docs a chaque session (README, cahier des charges, TODO, CHANGELOG, RESUME_PROMPT, MEMORY)
- Versionner avec des releases (semver)

## Headers de fichiers
- Le fichier CSS principal doit avoir le header standard du projet
- Mettre a jour @updated a chaque modification
- Mettre a jour @version quand la version du projet change

## ASCII Art du projet (reference)
```
   _                        _   _   _____ _
  | |    __ _ _ __ ___  _  | \ | | |_   _| |__   ___ _ __ ___   ___
  | |   / _` | '_ ` _ \| | |  \| |   | | | '_ \ / _ \ '_ ` _ \ / _ \
  | |__| (_| | | | | | | |_| |\  |   | | | | | |  __/ | | | | |  __/
  |_____\__,_|_| |_| |_|\__, |_| \_|   |_| |_| |_|\___|_| |_| |_|\___|
                         |___/
```

## Sessions de travail
- En fin de session, mettre a jour RESUME_PROMPT.md
- "save" / "sauvegarde" = mettre a jour TOUS les docs + commit + push

## Deploiement
- Le CSS est servi via jsDelivr depuis GitHub
- TOUJOURS utiliser une URL avec commit specifique (@hash) et non @main (cache agressif de jsDelivr)
- Apres chaque push, purger le cache : https://purge.jsdelivr.net/gh/NonoLMY/jellyfin-netflix-theme@main/theme-netflix.css
- Verifier avec WebFetch que la bonne version est servie avant de donner l'URL a l'utilisateur
