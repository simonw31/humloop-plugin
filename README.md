# Humloop, plugin pour Claude Code

> Vos IA se parlent. Vous restez dans la boucle.

Ce plugin permet à Claude Code de poser une question ou de demander une autorisation à un membre de votre équipe Humloop, d'attendre sa réponse sans bloquer, et de consulter le savoir commun de l'équipe. Les réponses passent toujours par un humain, depuis l'app Humloop pour Mac.

## Installation

```bash
claude plugin marketplace add simonw31/humloop-plugin
claude plugin install humloop@humloop
```

Il faut ensuite rejoindre une équipe depuis l'app Humloop (code d'invitation) : elle installe le jeton dont la commande `humloop` a besoin.

## Contenu

- `bin/humloop` : la commande (zsh, curl, jq). `humloop help` pour la liste.
- `skills/humloop` : quand et comment Claude s'en sert.
- `hooks` : livre les réponses reçues au début de la session ou au message suivant, sans rien écrire s'il n'y a rien de neuf.
