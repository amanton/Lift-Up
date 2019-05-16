Projet Ul - Lift up
====================

[Presentations slide](https://docs.google.com/presentation/d/1F90I4jqLM0xJeXBUU_vE5x2pX4bnX4WyPgPFGB-84LE/edit?usp=sharing)

Lift up

__Lift up__ a été imaginée et conçue pour les personnes avec _un léger handicap moteur_. Beaucoup de personne ne peuvent pas ou ont du mal à se relever lorsque qu'ils sont assis sur une chaise, et donc pour ces personnes là, on a voulu créer un prototype de chaise autonome et a l'aspect d'une chaise ordinaire __qui pourrait donc être placé dans les restaurants__ pour que ces personnes puissent manger au restaurant __sans aide pour se relever__.

Pourquoi somme nous aller vers ce projet ? __Ici je vais parler personnellement (Richard)__ je connais plusieurs personnes qui souffre au niveau des jambes, et ce qui m'a le plus marqué c'est mon grand-père qui aime beaucoup sortir aux restaurents mais depuis quelques années il ne veut plus y aller car il se __sent gênez de demander de l'aide pour le relever d'une chaise__, comme il existe déjà des siège et fauteuils qui aide à se relever, pourquoi des chaises fine ne peuvent pas le faire aussi ? En partant de cette question, le projet est né et les schémas ont commencé à être imaginé.

Il y avait plusieurs styles de chaise possible, la première aurais étais de faire __une chaise totalement automatisée avec des rails__ pour que les personnes n'aient pas grand chose à faire et surtout qu'il n'est pas à forcer, sauf que ce type avait des défauts, elle aurait étais __très peu maniable__ pour les restaurateurs et donc aucun l'aurais acheter.

Un version similaire vu le jour dans nos tête juste après, __remplacer les rails par des roues__, sauf que comme l'exemple du grand-père de richard, il a honte qu'on le voit avoir besoin d'aide, donc voir des roue sous une chaise serais la preuve qu'il a besoin d'aide, on est donc partie sur le troisième modèle qui est qu'on __garde l'architecture basique d'une chaise__, on rajoute un moteur ou des piston en dessous les plus discrets possibles, la personne devras certes faire un peu plus d'effort que les 2 autres chaises citez au-dessus, mais __la chaise sera pratiquement la même que les autres dans le restaurant__, et c'est vraiment le __but du projet__.

Comme on n'est pas des ingénieur et qu'on n'a pas les outils ni même les matériaux notre chaise donc l'aspect shoutaiter ne sera donc pas présent

Bon, partant de cette idée, on avait deux choix qui s'ouvrait a nous.
Faire une maquette puis essayer de faire une chaise grandeur nature, ou faire un prototype fonctionnel pour sa taille
On est partie pour un prototype fonctionnelle, car on a vu les prix des coûts pour une grandeur nature. 
Le projet étais donc lancer, nous avons quand même regarder sur le net si des chaise de ce style exister dans le marché. Mais sans grande trouvaille, sauf un produit nous reste en tête 


[Coussin d'aide à la levée](https://www.tousergo.com/aide-au-transfert/28-coussin-d-aide-a-la-levee-3574590140219.html)


Comme prévue pratiquement, aucune société ne fait de chaise de ce style, les sociétés préfèrent viser le marché des fauteuils par rapport aux chaises.
La première fut les pistons, simples, très robuste, mais chère.
La deuxième était de passer via un moteur et une crémaillère, moins robuste, mais efficace.

Après avoir choisi de passer par une crémaillère et un moteur.

![](https://zupimages.net/up/19/20/yr36.png) ![](https://zupimages.net/up/19/20/filr.png) ![](https://zupimages.net/up/19/20/6vpy.png)

voici la [chaise](https://www.ikea.com/fr/fr/p/kritter-chaise-enfant-rouge-80153697/)


nous vont aussi du modeliser des pièces en 3d pour faire la cremaillière et un support moteur
nous avons eu plusieurs idée lors de la modélisation


voici les [pièces modelisées pour le premier test](https://www.tinkercad.com/things/dY0HXlwu65n)


voici les [pièces modelisées](https://www.tinkercad.com/things/2Bs0kqwbqwV)

Lors de l'avancement une partie programmation étais présente. Nous avons dû programmer de l'Arduino (qui est proche du C et du C++), comme nous ne sommes pas expert en Arduino, nous avons commencé à regarder les librairies disponibles pour le fonctionnement d'un servomoteur, et surtout du Bluetooth.

Suite à plusieurs dizaines d'heures à essayer de faire fonctionner le Bluetooth sur la carte Arduino, même avec l'aide d'un professeur, la carte ne voulais rien savoir. Nous avons mis en place une application Android qui n'a pas abouti, car au début, on croyait que le fait que l'Arduino ne recevait pas les données venais de notre application, vous pouvez accéder au code [ici](https://github.com/DeadMeon/Lift-Up/blob/master/1erCodeArduino.ino).

Nous avons donc décider d'abandonner le Bluetooth via l'Arduino pour nous consacrer sur le Raspberry, nous avons donc commencer de la programmation python, nous sommes déjà un plus apte à être sur ce langage ayant appris les bases lors de notre année au début le Raspberry servais juste de relais pour envoyer des donner a l'Arduino, voici le code de [l'Arduino](https://github.com/DeadMeon/Lift-Up/blob/master/1erCodeArduino.ino).

Pendant le développement du programme en python pour la chaise, nous avons reçu la chaise et nous avons commencer les modifications dessus, pour la rendre "compatible" avec notre système, nous avons troué certain partie, retirer quelques parties aussi, mais nous avons surtout poncer beaucoup de partie que se soit de la chaise ou des pièces imprimé en 3d, rien de très compliquer, ça prend juste un peu de temps et de patience, la chaise avancer donc très bien pendant le temps du développement.

Une première version du code python vu le jour, la chaise se levais et redescendais tout été parfait ! Mais un jour plus rien n'était parfait nous avons donc décider de passer le projet que sur un unique Raspberry et nous avons fait nos adieux à l'Arduino qui nous a poser beaucoup de soucis, mais le Raspberry nous posa aussi beaucoup de soucis, du moins une libraire python nous causa beaucoup de soucis, Même en regardant des tutoriel, des vidéo, la documentation la première libraire que nous avions utilisé été incompréhensible, le moteur ne réagissais pas logiquement. Suite a ça nous avons trouver une nouvelle librairie qui réagissait correctement avec le moteur que nous avions et la chaise été donc enfin fonctionnelle. Voici le code [Python](https://github.com/DeadMeon/Lift-Up/blob/master/bluetoothGPIO.py), et le fait de passer que par le Raspberry nous fait donc avoir une chaise totalement libre niveau énergie, une simple batterie externe de téléphone suffit pour que la chaise fonctionne.

Les plus grosses difficultés rencontrées dans ce projet ont été le caprice que nous a fait l'Arduino, la librairie pas compatible avec notre moteur sur Python, et la modélisation des pièce 3d , pas de grosse difficulté nous on retarder juste des imprévue de temps en temps, mais rien de bien méchant;

La chaise est fonctionelle, mais elle n'est pas parfaite, des améliorations, peuvent etre envisager, que se soit materielle ou même application. Un des premiers ajouts qu'on pourrait faire, c'est un bouton sur la chaise pour donner plus de choix d'utilisation, car les personne agées n'ont pas tous un téléphone, ou même certaine ne savent pas utilisé le Bluetooth, on pourrait aussi créer une télécommande pour simplifier l'utilisation à distance. 

Notre moyen, de faire monter le siège de la chaise n'est pas parfait, il est utile pour les personnes ayant un léger handicap moteur, car la chaise va les aider et ils pourront prendre appuie dès qu'ils le veulent, mais pour les personnes ayant un handicap moteur assez élevé, notre système n'est pas du tout conseillée, car il y a des risques que la personne glisse si ses appuis ne sont pas pris.

Comme prévu n'étant pas des ingénieurs, nous n'avions pas toutes les compétences pour réaliser le projet avec un modèle réel et surtout nous avions pas le budget, la chaise a donc de petit défaut, comme le support moteur qui empêche la fermeture complète de la chaise, car la chaise est trop petite, mais ce souci devrait être réglé si nous passons sur une tailles grandeur nature.

Pour conclure, nous sommes fiers de présenter ce projet, c'est un projet qui nous tient a Coeur, essayer de donner une autonomie aux personnes qui la perde suite aux faiblesses de leur corps. C'est un monde qui n'est pas exploiter par les sociétés et nous ne comprenons pas, c'est certes peut être très complexe si on veut associer la puissance des moteur avec l'esthétique d'une chaise et le confort aussi, car il est vrai que nous n'avons pas du tout prêter attention au confort, car nous avions qu'une chaise en bois pour enfant on pouvais pas trop comparais, ce projet prouve que ce n'est pas impossible comme idée et que de nombreuses sociétés pourrais démocratiser ce domaine pour le bien des personnes dans le besoin.
