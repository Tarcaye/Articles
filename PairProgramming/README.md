``# You'll never code alone

_Note sur l'inclusivité, on parle de développeurs mais n'hésitez pas à remplacer développeurs par développeur·e·s dans votre cerveau._

<!-- https://media.giphy.com/media/3o6UBbsOZ3co6fJHLG/giphy.gif -->

Être développeur au sein d'une équipe ne se limite pas à dépiler des tâches les unes après les autres. 
Dans l'imaginaire collectif, les développeurs sont souvent associés à des êtres associaux travaillants seuls toute la journée sur un poste, surement dans une cave.

![Image of Cartman](https://i.ytimg.com/vi/2aDgH-_G4h0/maxresdefault.jpg)
<!-- _une des 2 images au choix_ https://i.ytimg.com/vi/2aDgH-_G4h0/maxresdefault.jpg -->
<!-- http://comedycentral.mtvnimages.com/images/shows/south-park/clip-thumbnails/season-10/1008/south-park-s10e08c05-the-slaughter-16x9.jpg -->
<!-- https://i.ytimg.com/vi/2aDgH-_G4h0/maxresdefault.jpg -->

D'après notre expérience, la réalité est souvent toute autre : Vous ne travaillerez quasiment jamais seuls dans votre coin, vous ferez surement partie de ce qu'on appelle... une équipe !
En plus de la collaboration avec les autres membres de l'équipe, une partie de notre travail consiste à relire du code, guider les autres développeurs, etc.
**_````_**
## Pair 101 // Définition

La collaboration, le mentoring et les revues de code peuvent prendre différentes formes selon les projets. L'une des solutions que nous avons choisi d'adopter, notamment en action de rétrospective, et qui semble connue et reconnue de nombreux développeurs est le binomage.

![Image of Pair](https://developer.atlassian.com/blog/2015/05/try-pair-programming/images/the-noob.jpg)

Pourtant bien que la plupart d'entre nous semble ouvert à la mise en place de cette pratique, elle n'est souvent pas utilisée. Mais quels sont les freins au pair programming ?

### Notes
J’ai jamais binomé...
Je n'ai jamais binômé... je ne suis pas contre mais avec qui commencer... en attendant je reste comme ça. 
Charge aux développeurs ayant déjà cette expérience de faire découvrir aux aspirants, et de leur laisser le temps 
de se l'approprier... bien binomer ça se travaille. Privilégier un binomage progressif, d'abord sous forme de test... puis on verra.

J’arrive à trouver tout seul, je comprend pas le besoin que toi tu as de binômer 
Le travail en équipe nécessite du partage et de la communication... bien communiquer n'est pas chose aisée. Une équipe
est souvent composée de caractères différents, de certitudes, de forces/faiblesses, parfois d'un brin de manipulation.
Un des buts qui pourrait être atteint est la fiertée du travail accompli en communauté et l'envie de le partager.

Et si moi j’arrive pas à trouver tout seul ...// entre aide // Y toujours des choses à
apprendre // moins de risuqe d’erreur // Qulité / Vitesse #mindset

J’ai peur du jugement de mon pair... mise à nu/ego (// pas plus de jugement // sentiment réciproque // C’est pas du jugement) #mindset
Peur du jugement et envie d'apprendre... nous sommes pleins de contradictions. L'ouverture aux connaissances de son 
binôme et l'humilité sur nos connaissances, deux réactions qui doivent nous permettre de bien vivre le travail à deux. 

On fait des tâches machinales où le binomage n’apporte rien à mon sens. // pénibilité de ta
tache diminuée par ton binome // Quel est la frontière entre une tache facile //
Potentiellement refactorer// trouver des bugs autour // Potentiellemnt plus d’erreurs
d’inattention // automatisation 
=> Quand binomer


## This is not pair programming ! // Anti pattern
(peut être mettre cette partie après)

Le but de cet article n'est pas de vanter les mérites du travail en binôme mais plutôt de voir quels sont les contraintes et les blocages que l'ont peut rencontrer avec cette pratique et comment les contourner. // J'aime moyennement cette phrase, trouver comment reformuler

<Une image avec 2 personnes devant un PC donc un qui fait autre chose genre dort>

Soyons clairs, binomer ce n'est pas juste se poser à 2 devant un poste, c'est une pratique qui s'apprend et qui nécessite du travail et des essais.

### Notes
En plus tu n'as pas le même rythme de dev que moi // différence de connaissance, aisance,
// Pour le plus expérimenté c’est le next step de savoir expliquer/faire comprendre/faire
apprendre ; c’est le role des plus expérimenté des former acompagner // montée en
compétences accompagnement
// Blocage certains n’ont pas encore la pas la patience // la compétence pour faire de
l’accompagnement #mindset

Je vais plus vite tout seul // cf plus haut

On ira plus vite chacun de notre côté // idée reçu ? expérience Sopra #performance


Je dois tjrs me battre pour récupérer le clavier/je lâcherai pas le clavier // Timebox // ping
pong // strong #outils #technique

Dès que j'ai le clavier tu en profites pour dormir et tu déconnectés complètement // echanges
de clavier rapides -> moins le temps de déconnecter // Ping pong // Strong autre solution
#outils #technique

## How To // Tricks

### Notes

C'est fatigant, je peux pas regarder mes mails, encore moins répondre aux whatsapp,
regarder twitter…. // Pomodorro ; difficile de trouver un rythme à plusieurs ; se caler des
pauses #outils #technique

En plus tu n'as pas le même rythme de dev que moi // différence de connaissance, aisance,
// Pour le plus expérimenté c’est le next step de savoir expliquer/faire comprendre/faire
apprendre ; c’est le role des plus expérimenté des former acompagner // montée en
compétences accompagnement
// Blocage certains n’ont pas encore la pas la patience // la compétence pour faire de
l’accompagnement #mindset

Je vais plus vite tout seul // cf plus haut

On ira plus vite chacun de notre côté // idée reçu ? expérience Sopra #performance

Dur d'appréhender du nouveau code à deux, tu veux aller voir cette classe alors que je
serais plutôt aller dans celle ci // Explrer les pistes à tour de role (ecriture puis binnome A
explore la piste de binome B et vice versa) // Se mettre d’accord sur la compréhension/
cartographie #technique

On s’entend pas du tout / c’est pas mon pote #connard #mindset

Je/il développe sur Mac avec un ide obscur // Strong // Change d’environnement // Tous le
même poste // Poste impersonnel #outils

J’ai jamais binomé, j’ai pas de méthodologie pour le binomage. // Toute chose a un début /
MeetUp / Articles #technique

Quand je binôme avec toi tu me donnes des ordres et je suis juste une machine qui fait ce
que tu me demandes // Changer de role -> pingpong / Strong
Si le pb c’est un noob + un expert alors ne pas donner la réponse mais plutôt le chemin pour
trouver la solution #technique #mindset

Pingpong / Strong

// Certains binome avec 2 PC en pushant pour etre multi OS/IDE

Donner du feedback, dans les 2 sens // encourageant

## Etat d'esprit // Mindset Quel est le bon mindset pour développer

![Mood](https://memegenerator.net/img/instances/500x/81131975/of-course-id-love-to-work-with-you-but-im-not-in-the-mood.jpg)

### Notes
Au cours de nos discussions, on s'est rendu compte que ...
On s’entend pas du tout / c’est pas mon pote #connard #mindset

// Il code avec un clavier mécanique en qwerty // prévoir un 2e clavier #outils

Je suis trop extrémiste craft et pas les autres du projet (genre le raise the bar dans le
mauvais sens) // Raise the bar progressivement #mindset

J’ai peur du jugement de mon pair // pas plus de jugement // sentiment réciproque // C’est
pas du jugement #mindset

J’aime travaillé en musique #mindset #connard

On n’a pas les mêmes horaires // travail en équipe #mindset

# Conclusion
Full time pair programming
