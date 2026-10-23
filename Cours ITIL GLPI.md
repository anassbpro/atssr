```markdown
# ITIL

L'ITIL (Information Technology Infrastructure Library), c'est un **référentiel de bonnes pratiques** pour gérer les services informatiques dans une entreprise. Ce n'est ni un logiciel ni une loi : c'est un ensemble de méthodes, créé au départ par le gouvernement britannique dans les années 80, pour que le service informatique fonctionne de façon organisée.

**L'idée centrale** : le service informatique n'est pas là juste pour réparer des PC, il **rend un service** aux utilisateurs, comme un prestataire envers ses clients. L'objectif est que ce service soit fiable, rapide et qu'il s'améliore en continu.

## Les notions clés

- **Le Service Desk** : le point de contact unique pour les utilisateurs. Tous les appels et tickets arrivent au même endroit.
- **Un incident** : quelque chose qui ne marche plus et qu'il faut rétablir vite. Exemple : l'imprimante d'un bureau ne répond plus. Le but est de **remettre en service** le plus rapidement possible, même avec une solution temporaire.
- **Un problème** : la **cause profonde** d'un ou plusieurs incidents. Si l'imprimante plante tous les lundis, on cherche pourquoi pour régler le souci définitivement.
- **Un changement** : toute modification du système (mise à jour, nouveau serveur…). ITIL demande de les préparer et de les valider pour ne pas tout casser.
- **Le SLA (Service Level Agreement)** : un accord sur le niveau de service promis, par exemple « un incident critique est traité en moins de 4 heures ».

## Exemple concret

Un utilisateur appelle car il n'a plus Internet. Le technicien du Service Desk crée un ticket (incident) et rétablit la connexion. Si dix personnes ont le même souci dans la semaine, on ouvre un problème pour trouver la vraie cause. Si la solution demande de remplacer un switch, ça devient un changement planifié.

## En résumé

ITIL, c'est une façon de structurer le travail d'un service informatique pour qu'il soit efficace, traçable et tourné vers les utilisateurs. La version actuelle est ITIL 4, qui met davantage l'accent sur la création de valeur et l'amélioration continue.

---

# GLPI

Le GLPI, c'est un **logiciel de gestion de parc informatique et de helpdesk**. Son nom veut dire **Gestionnaire Libre de Parc Informatique**. Il est gratuit, open source et d'origine française, ce qui explique qu'on le croise souvent en entreprise et en formation.

## À quoi il sert

- **L'inventaire du parc** : il recense tout le matériel et les logiciels de l'entreprise (PC, imprimantes, serveurs, licences…). On sait qui utilise quoi, où, et depuis quand. Avec un agent installé sur les postes, l'inventaire peut se remplir automatiquement.
- **La gestion des tickets** : quand un utilisateur a un souci, il crée un ticket dans GLPI. Le technicien le prend en charge, suit son avancement et le clôture une fois réglé. Tout est tracé.
- **Le lien entre les deux** : un ticket peut être rattaché directement à l'appareil concerné. Si un PC accumule les pannes, on le voit tout de suite dans son historique.
- **D'autres fonctions** : gestion des contrats, des fournisseurs, des garanties, une base de connaissances pour noter les solutions déjà trouvées, et des statistiques.

## Le lien avec ITIL

GLPI est l'outil qui permet d'**appliquer ITIL en pratique**. Il reprend les mêmes notions : incidents, problèmes, changements, demandes, SLA. ITIL te dit *comment* organiser le service informatique, GLPI te donne *l'outil* pour le faire au quotidien.

## Exemple concret

Un utilisateur signale que son PC ne démarre plus. Il ouvre un ticket dans GLPI. Le technicien voit dans la fiche du PC qu'il a déjà eu deux pannes ce mois-ci, règle l'incident, puis ouvre un problème pour comprendre la cause. Tout reste enregistré pour la suite.
```
