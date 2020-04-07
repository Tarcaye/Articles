# You'll never code alone
_Travaillant depuis un an en [pair](https://en.wikipedia.org/wiki/Pair_programming "Pair programming") ou en [mob programming](https://en.wikipedia.org/wiki/Mob_programming "Mob programming") quotidiennement à distance, 
j'ai pensé partager avec vous notre façon de télétravailler._

![Image of Cartman](https://i.ytimg.com/vi/2aDgH-_G4h0/maxresdefault.jpg)

### Contexte
Nous sommes une équipe de 5 avec une personne vivant sur Bordeaux. 
L'équipe est composée de profils assez différents :
- 2 profils séniors plutôt orientés craft
- 1 profil junior
- 1 scrum master
- 1 product owner

### Prérequis
Quelque soit votre langage de programmation, la méthode avec laquelle nous travaillons peut s'adapter à vos besoins si vous disposez à minima des outils suivants:

- Un outils de gestion de version (git, svn, etc.),
- Un outils de visio / partage d'écran,
- Votre IDE préféré,
- Un chronomètre,
- Une connexion internet décente.

On ne fait pas de partage de code sur des serveurs privés (sandbox, floobits intelliJ, etc.) pour des raisons de sécurité.
L'avantage de notre méthode est que chacun peut utiliser son OS, son IDE, ses raccourcis, son type de clavier, etc.

On utlise également un [script](https://github.com/HadrienMP/limbo) pour faire du push/pull automatique sur git.

### Rythme 
[XP](https://blog.engineering.publicissapient.fr/2008/01/10/scrum-ou-xp-scrum-et-xp/) prône un rythme soutenable, on essaye de travailler un maximum tous ensemble, sans avoir à respecter les mêmes horaires.  
En général l'équipe arrive entre 8h00 et 9h30. 
Le premier arrivé commence à bosser puis il est progressivement rejoint par le reste de l'équipe, mob. 
On n'attend pas que tout le monde soit là pour commencer, 
ce qui nous donne une plus grande amplitude horaire. 
Lorsque qu'un nouveau membre rejoint le groupe, il suffit de lui montrer ce qui a pu être réalisé en son absence. 

De mon côté, j'essaie de respecter les horaires de travail que j'aurai en étant sur site.
j'ai aussi un rituel très simple qui consiste à me préparer ainsi qu'à m'habiller 
comme si j'allais au travail, ça m'aide à lancer ma journée. 

![](https://i.pinimg.com/736x/29/5b/94/295b9419b80fc1c2b8abc758dbcd9df2--work-shirts-funny-videos.jpg)

N'oubliez pas non plus de faire des pauses régulières. On a facilement tendance à travailler sans relache. Vous pouvez par exemple utiliser la technique du [pomodorro](https://fr.wikipedia.org/wiki/Technique_Pomodoro) pour faire des pauses régulières. 

### Communication
La communication non verbal est un élément important lorsque l'on travaille en mob en pair programming.
L'un des points importants de la communication à distance c'est d'activer sa webcam.
En effet c'est plus compliqué de prendre la parole à distance, la webcam aide à la prise de parole et permet de faire passer plus d'informations que la voix seule. 

Ça permet également de voir plus facilement si un des participants est en désaccord. 

![homer](https://bigbiggityben1.files.wordpress.com/2015/09/cartoon-homer-looking-right-two.png)

En plus, on est facilement isolé quand on bosse à la maison, 
la caméra nous permet plus facilement d'entretenir de bonnes interactions sociales. 

(TODO : Photo meet up ou katas en ligne shodo)

? Où mettre cette phrase ? developper un peu (c'est cool, pas cool, vous en pensez quoi les autres, etc.) ¿ Il est également très important de donner du feedback au reste de l'équipe ou d'en demander

### Itération
Nous fonctionnons par itérations à durées fixes,chacun prend le clavier à tour de rôle en commitant de manière très régulière sur git.
En mob, nos tours durent de 8 à 12 minutes mais il nous arrive de diminuer le temps de clavier à 4 voire 2 minutes pour s'obliger à faire des baby steps.
Cela evite d'avoir une personne qui monopolise le clavier pendant que les autres regardent et ne se sentent plus concerné.e.s.
A la fin de chaque tour, on essaye d'avoir un build vert quit à reverter nos modifs pour ne pas dépasser le temps qui nous est alloué. 

On utilise un timer synchronisé, [mob time](https://github.com/HadrienMP/mob-time), qui joue de sympathique musique ;)

![](https://tse1.mm.bing.net/th?id=OIP.LsY1UAITtdneG7m-Z6RfOgEgDY&pid=Api) 

On essaie d'être fluide, rapide de pas dépasser notre temps qui a revenir en arrière sur nos modifications au lieu de dépasser ou de casser le build, et ça force les petits incréments. 

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
- Limited WIP,
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

Nous avons créé un [meetup](https://www.meetup.com/fr-FR/paris-mob-programming/) où on va essayer de faire des sessions de mob en remote.

Je suis également disponible pour faire un BBL ou animer un kata à distance si ça vous intéresse.

#### Source :
https://www.remotemobprogramming.org/
https://github.com/willemlarsen/mobprogrammingrpg
https://twitter.com/GuLhe_le_GuJ/status/1240067198946881540
https://github.com/HadrienMP/limbo
https://github.com/HadrienMP/mob-time


# TODO ?
on travaille en remote par défaut / meme sur site pour inclure au maximum les personnes à distance
