# You'll never code alone
Depuis un an, je travaille quotidiennement en pair ou mob programming avec une équipe à distance. 

Le Mob Programing consiste à faire travailler toute une équipe sur une seule tâche en codant à tour de rôle, c'est une forme d'extension du pair programming. 
Cette approche permet à une équipe de travailler sur presque toutes les activités de développement logiciel, comme la conception, le développement ou les tests. 

Durant ma carrière, j’ai souvent eu l'occasion de travailler en mob programming. 
Mais c’est cette dernière année que j’ai le plus perfectionné ma méthode en la pratiquant quotidiennement 
et notamment en remote.

Aujourd’hui, à niveau de qualité égale, 
nous sommes au moins aussi véloces en mob qu'en pair ou en développant seuls.

C’est pourquoi, par les temps qui courent, 
j’ai eu envie de partager avec vous mes conseils de mob programming à distance. 
J’espère qu’après ça, You’ll never Code alone ! 

![Image of Cartman](https://i.ytimg.com/vi/2aDgH-_G4h0/maxresdefault.jpg)

### Contexte
Nous sommes une équipe de 5 avec une personne qui habite à Bordeaux et le reste à Paris. 
L'équipe est composée de profils assez différents :
- 2 profils séniors plutôt orientés craft
- 1 profil junior
- 1 scrum master
- 1 product owner

Les développeurs de l'équipe travaillaient initialement seuls et organisaient des séances communes de relecture de code. Lors de ces séances, il arrivait que les développeurs réécrivent toute une user story ensemble.
C'est à partir de là que l'équipe a décidé de commencer à travailler en mob.

### Prérequis
Quel que soit votre langage de programmation, la méthode avec laquelle nous travaillons peut s'adapter à vos besoins si vous disposez a minima des outils suivants:

- Un outil de gestion de version (git, svn, etc.),
- Un outil de visio / partage d'écran,
- Votre IDE préféré,
- Un chronomètre pour aider à partager le temps de clavier,
- Une connexion internet décente.

Nous avons considéré la possibilité de travailler avec des outils de partage de code 
style Sandbox pour Visual Studio, Floobits pour IntelliJ. 
Pour des raisons de sécurité, le code transitant par des serveurs tiers, nous n'avons pas pu. 
Et la technique alternative que nous avons trouvée me paraît avoir des effets plus intéressants : 
chacun peut utiliser son OS, son IDE, ses raccourcis, son type de clavier, etc. 
Cette méthode force également les participants du mob à faire des babys step et à committer très régulièrement sur git.

Pour augmenter la vitesse de partage du code et la fréquence d'intégration continue, nous utilisons un [script](https://github.com/HadrienMP/limbo) pour faire du push/pull automatique sur git.

### Rythme 
[XP](https://blog.engineering.publicissapient.fr/2008/01/10/scrum-ou-xp-scrum-et-xp/) prône un rythme soutenable, on essaye de travailler un maximum tous ensemble, sans avoir à respecter les mêmes horaires.  
En général l'équipe arrive entre 8h00 et 9h30. 
Le premier arrivé commence à bosser puis il est progressivement rejoint par le reste de l'équipe, mob. 
On n'attend pas que tout le monde soit là pour commencer, 
ce qui nous donne une plus grande amplitude horaire. 
Lorsqu'un nouveau membre rejoint le groupe, il suffit de lui montrer ce qui a pu être réalisé en son absence. 

De mon côté, j'essaie de respecter les horaires de travail que j'aurai en étant sur site.
j'ai aussi un rituel très simple qui consiste à me préparer ainsi qu'à m'habiller 
comme si j'allais au travail, ça m'aide à lancer ma journée. 

![](https://i.pinimg.com/736x/29/5b/94/295b9419b80fc1c2b8abc758dbcd9df2--work-shirts-funny-videos.jpg)

N'oubliez pas non plus de prendre des pauses régulières. 
On a facilement tendance à travailler sans relâche. 
Le mob peut continuer sans vous le temps d'une pause personnelle 
ou alors il peut être intéressant de convenir de pauses régulières tous ensemble. 
Vous pouvez par exemple utiliser la technique du [pomodorro](https://fr.wikipedia.org/wiki/Technique_Pomodoro). 

### Communication
L'un des points importants de la communication à distance c'est d'activer sa webcam.
La communication non verbale est un élément important lorsque l'on travaille en mob ou en pair programming.
En effet c'est plus compliqué de prendre la parole à distance, la webcam aide à la prise de parole et permet de faire passer plus d'informations que la voix seule. 

Ça permet également de voir plus facilement si un des participants est en désaccord. Quelques signes peuvent en effet être facilement détectés : des soupirs, le silence, un regard fuyant, une mine déconfite, etc. 

![homer](https://bigbiggityben1.files.wordpress.com/2015/09/cartoon-homer-looking-right-two.png)

N'hésitez pas à demander du feedback au reste de l'équipe ou à donner, ça permet de clarifier la situation sur ce qu'on est en train de produire. 
Vous pouvez facilement demander si tout le monde est ok avec ce que vous êtes en train de faire, demander l'avis de ceux qui s'expriment peu pour faciliter le dialogue.
À l'inverse, n'hésitez pas à exprimer votre accord/désaccord avec une décision même si on ne vous demande pas explicitement votre avis. 

En plus, on est facilement isolé quand on bosse à la maison, 
la caméra nous permet plus facilement d'entretenir de bonnes interactions sociales. 

(TODO : Photo meet up ou katas en ligne shodo)

### Itération
Nous fonctionnons par itérations à durées fixes,chacun prend le clavier à tour de rôle en commitant de manière très régulière sur git.
En mob, nos tours durent de 8 à 12 minutes mais il nous arrive de diminuer le temps de clavier à 4 voire 2 minutes pour s'obliger à faire des baby steps.
Cela evite d'avoir une personne qui monopolise le clavier pendant que les autres regardent et ne se sentent plus concerné.e.s.
A la fin de chaque tour, on essaye d'avoir un build vert. 

On utilise un timer synchronisé, [mob time](https://github.com/HadrienMP/mob-time), qui joue de sympathique musique ;)

![](https://tse1.mm.bing.net/th?id=OIP.LsY1UAITtdneG7m-Z6RfOgEgDY&pid=Api) 

On essaie d'être fluide, rapide, de ne pas dépasser notre temps quitte à revenir en arrière sur nos modifications au lieu de dépasser ou de casser le build, et ça force les petits incréments. 

### Méthodologies

En pair programming, on travaille plutôt en utilisant 2 rôles, driver et navigator, un peu à l'image du strong style pair programming :
- Le driver, ou conducteur :  est celui qui partage
C'est la personne qui code et partage son écran. 
Elle ne prend presque pas d'initiative et obéit aux instructions du navigateur.
- Le navigateur :
C'est la personne qui donne des instructions au driver, avec un niveau d'abstraction assez elevé pour lui donner la direction dans laquelle aller.

Les méthodologies ne sont pas figées, n'hésitez pas à faire des micro rétrospectives régulières dédiées uniquement au mob ou au pair pour améliorer votre fonctionnement.
Essayez d'expérimenter de nouvelles façons de travailler, en journée ou en dojo, même si elles peuvent sembler un peu extrème :
- Tour de mob d'1 à 2 minutes,
- Driver muet,
- [Limited WIP](https://plugins.jetbrains.com/plugin/7655-limited-wip),
- [TCR](https://medium.com/@kentbeck_7670/test-commit-revert-870bbd756864)

Ces expérimentations vous permettrons de mieux trouver un consensus sur votre manière de travailler.

Pour la relecture ou l'exploration de code, il peut être pertinent de donner la main à un membre de l'équipe découvrant du code, plutôt qu'à celui ou celle qui le connait déjà.
Cela permet d'éviter de montrer du code à une personne qui ne comprend pas et n'ose pas le dire, en tout cas, ça limite cet effet.

### Mise en pratique :
N'hésitez pas à tester en faisant un [coding dojo](http://codingdojo.org/) ;
- Katas 
- Entre 2 et X participants
- Un driver 
- un navigateur
- un timekeeper

Nous avons créé un [meetup](https://www.meetup.com/fr-FR/paris-mob-programming/) avec [@HadrienMP](https://twitter.com/HadrienMP) où on va faire des sessions de mob en remote régulière afin de partager et d'améliorer nos pratiques tous ensemble, qu'on soit novice ou expérimenté.

Je suis également disponible pour faire un BBL ou animer un kata à distance si ça vous intéresse.

#### Source :
https://www.remotemobprogramming.org/
https://github.com/willemlarsen/mobprogrammingrpg
https://twitter.com/GuLhe_le_GuJ/status/1240067198946881540
https://github.com/HadrienMP/limbo
https://github.com/HadrienMP/mob-time