# CLAUDE.md — bbl-ui
<!-- Working rules for Claude in this repository (French). Code and docs are in English. -->

`bbl-ui` : la crate d'interface commune des outils Blackberrylabs (Cleanator, MCProster,
Permitt, puis la tour de controle) — palette, briques iced, reglages d'interface, textes
traduits. Aucune logique metier.

## Regles de travail

- BRIEF valide avant le code ; PLAN et JOURNAL tenus ; `00_cadrage/` hors git.
- Un changement ici se verifie sur les trois apps (tests verts, captures a l'oeil) avant
  d'etre commite. iced fixe a `=0.13.1`.
- Rien d'ecrit hors `~/.config/<app>/settings.json` via `Prefs::save`.
- Commits locaux libres ; `git push`, suppression de fichiers, tags : accord explicite.
  Commandes completes, chemin absolu (`cd /home/nushoko/Bureau/Logiciels/Bbl_ui && …`).
- Anglais : code, commentaires, commits, README. Francais : pilotage.
- Seul nom cite : Alexandre Do.

## Identite git

Avant le **premier commit** : `git config user.name "Alexandre Do"` et
`git config user.email "277202463+Nimeria2026@users.noreply.github.com"` (config locale) ;
verifier `git log --format='%an <%ae>'` avant tout push.
