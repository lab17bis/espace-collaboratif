# espace-collaboratif

> **Espace Grist clé en main.** Un document Grist prêt à l'emploi pour **travailler ensemble** : les réunions de l'équipe, ses projets partagés et ses ressources communes, au Système de design de l'État (DSFR).

Un **espace** est un document Grist complet — tables, formules, pages, widgets et réglages — à importer en une fois. Il assemble des widgets de la famille `grist-…` autour d'une manière de travailler. Chaque widget reste utilisable seul.

## À quoi ça sert

- **Préparer et tenir les réunions** : chacun propose des points, les notes, décisions et actions sont prises en séance, le compte rendu se met en page tout seul.
- **Partager les projets** de l'équipe ou de plusieurs services, avec leurs porteurs, leur plan d'action et leur journal.
- **Mettre en commun des ressources** (outils, méthodes, conseils, modèles) dans un catalogue consultable et filtrable.
- **Décider ensemble** : une boîte à idées d'équipe avec soutiens et suites données, et des choix collectifs (créneau, outil, option) en choix unique ou en notation.
- Les actions décidées en réunion et les actions des projets restent chacune dans leur outil, sans double saisie.

## Ce que contient l'espace

| Page | Outil | Contenu |
| --- | --- | --- |
| **Réunions** | [grist-reunion](https://github.com/lab17bis/grist-reunion) | Ordre du jour, séance, compte rendu, suivi des actions. Tables `Reunions`, `Points`, `Decisions`, `Actions_reunion`. |
| **Projets** | [grist-projet](https://github.com/lab17bis/grist-projet) | Banque de projets, fiches projet, plans d'action, journal et règles d'accès. |
| **Décider ensemble** | [grist-decision](https://github.com/lab17bis/grist-decision) | Boîte à idées de l'équipe et choix collectifs, avec résultats et suites données. Tables `Consultations`, `Propositions`, `Criteres`, `Votes`, `Votants`. |
| **Ressources communes** | [grist-catalogue](https://github.com/lab17bis/grist-catalogue) | Catalogue des ressources de l'équipe. Page *Fiches* pour ajouter une ressource, page *Régler les ressources* pour le modifier. Table `Ressources`. |

## L'installer en 2 minutes

1. **Télécharger** le fichier de l'espace :
   - [`espace-collaboratif.grist`](https://github.com/lab17bis/espace-collaboratif/raw/main/espace-collaboratif.grist) : l'espace vide, prêt à l'usage ;
   - [`espace-collaboratif-exemple.grist`](https://github.com/lab17bis/espace-collaboratif/raw/main/espace-collaboratif-exemple.grist) : le même, rempli de données fictives, pour essayer.
2. **L'importer dans Grist** : depuis l'accueil de votre espace Grist, *Ajouter › Importer un document*, puis choisissez le fichier.
3. **L'ouvrir** : les pages et les widgets sont déjà en place. Si Grist le demande, confirmez l'accès complet des widgets au document.
4. **Inviter l'équipe** (*Partager*), en éditeur pour celles et ceux qui saisissent.

Vous êtes propriétaire du document importé. Rien n'est installé ailleurs : les widgets sont des pages web publiques, qui lisent et écrivent dans votre document avec les droits de la personne connectée.

Les widgets sont chargés depuis leur **adresse stable** (`…/v1/`) : une évolution d'un widget ne modifie pas votre espace sans que vous l'ayez décidé.

## Le régler

- **Réunions** : lien *Réglages* en bas du widget.
- **Projets** : lien *Réglages du suivi*.
- **Décider ensemble** : bouton *Nouvelle consultation*, puis onglet *Gérer* de chaque consultation.
- **Ressources communes** : page *Régler les ressources* (sections, filtres, étiquettes, contenu des fiches). Ajoutez ou renommez les colonnes de la table `Ressources` selon vos besoins.

Les réglages sont enregistrés dans le document. Ils partagent les mêmes réglages d'en-tête et de pied de page.

## Données et droits d'accès

Les votes de la page *Décider ensemble* portent l'adresse de leur auteur, visible des propriétaires dans la table `Votes`. L'espace contient aussi les **règles d'accès** de grist-projet, qui protègent les projets restreints. Elles ne concernent que les tables de projets. Vérifiez-les dans *Permissions avancées* avant d'inviter l'équipe.

Les tables `Personnes` et `Structures`, quand l'espace en contient, suivent la règle commune des widgets : un widget de la famille ajouté plus tard les reprend et les complète, au lieu d'en créer d'autres.

Les fichiers de ce dépôt ne contiennent aucune donnée réelle. L'exemple est entièrement fictif.

## Widgets utilisés

- [grist-catalogue](https://github.com/lab17bis/grist-catalogue) : catalogue de fiches au DSFR, avec recherche et filtres.
- [grist-projet](https://github.com/lab17bis/grist-projet) : banque de projets partagée et plans d'action.
- [grist-reunion](https://github.com/lab17bis/grist-reunion) : ordres du jour, notes, décisions, actions et comptes rendus.
- [grist-decision](https://github.com/lab17bis/grist-decision) : consultations : boîte à idées, valorisation des réalisations, votes et suites données.

## Autres espaces

- [espace-pilotage](https://github.com/lab17bis/espace-pilotage) : regarder et décider : un écran d'équipe qui rassemble indicateurs, réunions, projets, priorités et parties prenantes.
- [espace-accompagnement](https://github.com/lab17bis/espace-accompagnement) : suivre les personnes qui sollicitent un service : offre de service, sollicitations, fiches contact et satisfaction.
- [espace-sondage](https://github.com/lab17bis/espace-sondage) : concevoir un questionnaire, savoir qui a répondu et lire les résultats en indicateurs.
- [espace-communaute](https://github.com/lab17bis/espace-communaute) : animer une communauté de pratique ou un réseau : membres, groupes, rencontres, présences, ressources partagées, retours, carte et liens entre acteurs.
- [espace-contributions](https://github.com/lab17bis/espace-contributions) : faire participer : boîte à idées, valorisation des réalisations des équipes, votes et suites données.

## Écosystème

- **[Grist](https://grist.numerique.gouv.fr)** : tableur-base de données libre ([gristlabs/grist-core](https://github.com/gristlabs/grist-core)), proposé aux agents publics par la [DINUM](https://www.numerique.gouv.fr/) dans [La Suite numérique](https://lasuite.numerique.gouv.fr/). L'espace s'importe dans toute instance de Grist.
- **[Système de design de l'État (DSFR)](https://www.systeme-de-design.gouv.fr/)** ([GouvernementFR/dsfr](https://github.com/GouvernementFR/dsfr)). Son usage est réservé aux sites des services de l'État.

## Mots-clés

Grist, espace Grist, modèle Grist, document clé en main, travail collaboratif, équipe, réunion, ordre du jour, compte rendu, gestion de projet, ressources partagées, catalogue, boîte à idées, décision collective, DSFR, Système de design de l'État, La Suite numérique, service public, logiciel libre.

## Licence

Fichiers de l'espace et documentation sous licence Creative Commons [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.fr) : réutilisation et adaptation autorisées, en citant la source et en partageant sous la même licence. Le code des widgets est sous licence MIT, dans leurs dépôts.

Conçu par le Lab 17 bis, laboratoire d'innovation publique de l'académie de Reims. Contact : <lab17bis@ac-reims.fr>
