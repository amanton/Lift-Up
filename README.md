Projet Ul - Lift up
====================

[Presentations slide](https://docs.google.com/presentation/d/1F90I4jqLM0xJeXBUU_vE5x2pX4bnX4WyPgPFGB-84LE/edit?usp=sharing)

Lift up

__Lift up__ a été imaginée et conçue pour les personnes avec _un léger handicap moteur_. Beaucoup de personne ne peuvent pas ou ont du mal à se relever lorsque qu'ils sont assis sur une chaise, et donc pour ces personnes-là, on a voulu créer un prototype de chaise autonome et a l'aspect d'une chaise ordinaire __qui pourrait donc être placé dans les restaurants__ pour que ces personnes puissent manger au restaurant __sans aide pour se relever__.

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
Comme prévue pratiquement, aucune société ne fait de chaise de se styler, les sociétés préfèrent viser le marché des fauteuils par rapport aux chaises.
La première fut les pistons, simples, très robuste, mais chère.
La deuxième était de passer via un moteur et une crémaillère, moins robuste, mais efficace.

Après avoir choisi de passer par une crémaillère et un moteur.

![](https://zupimages.net/up/19/20/yr36.png) ![](https://zupimages.net/up/19/20/filr.png) ![](https://zupimages.net/up/19/20/6vpy.png)

voici la [chaise](https://www.ikea.com/fr/fr/p/kritter-chaise-enfant-rouge-80153697/)


nous vont aussi du modeliser des pièces en 3d pour faire la cremaillière et un support moteur
nous avons eu plusieurs idée lors de la modélisation


voici les [pièces modelisées pour le premier test](https://www.tinkercad.com/things/dY0HXlwu65n)


voici les [pièces modelisées](https://www.tinkercad.com/things/2Bs0kqwbqwV)

Lors de l'avancement une partie programmation étais présente.
nous avons dû programmer de l'arduino (qui est proche du C et du C++), comme nous ne somme pas expert en arduino, nous avons commencer a regarder les librairies disponible pour le fonctionnement d'un servo moteur, et surtout du bluetooth.
suite à plusieurs dizaine d'heure a essayer de faire fonctionner le bluetooth sur la carte arduino, même avec l'aide d'un proffeseur, la carte ne voulais rien savoir. Nous avons mis en place une application android qui n'a pas aboutie, car au debut on croyer que le fait que l'arduino ne recevez pas les donnée venais de notre application, vous pouvez acceder au code [ici](https://github.com/DeadMeon/Lift-Up/blob/master/Test_Applcation_Android/main/java/com/example/devicelist/MainActivity.java). 
nous avons donc decider d'abandonner le bluetooth via l'arduino pour nous consacrer sur le raspberry, nous avons donc commencer de la programmation python, nous sommes déjà un plus apte a être sur ce langage ayant apprit les bases lors de notre année au début le raspberry servais juste de relais pour envoyer des donner a l'arduino, voici le codes de [l'arduino](https://github.com/DeadMeon/Lift-Up/blob/master/1erCodeArduino.ino).
pendant le devellopement du programme en python pour la chaise, nous avons reçu la chaise et nous avons commencer les modifications dessus, pour la rendre "compatible" avec notre systeme, nous avons trouer certain partie, retirer quelque partie aussi mais nous avons surtout poncer beaucoup de partie que se soit de la chaise ou des pièces imprimé en 3d, rien de très compliquer, sa prend juste un peu de temps et de patience, la chaise avancer donc tres bien pendant le temps du devellopement. une première version du code python vu le jour, la chaise se lever et redéscender tout été parfait ! mais un jours plus rien n'était parfait nous avons donc décider de passez le projet que sur un unique raspberry et nous avons fait nos adieu a l'arduino qui nous a poser beaucoup de soucis, mais le raspberry nous posa aussi beaucoup de soucis, du moins une libraire python nous causa beaucoup de soucis, Même en regardant des tutoriel, des video, la documentaion la premiere libraire que nous avions utilisé été imcompréhensible, le moteur ne régaiser pas logiquement. suite a ça nous avons trouver une nouvelle librairie qui réagissait correctement avec le moteur que nous avions et la chaise été donc enfin fonctionelle. voici le code [Python](https://github.com/DeadMeon/Lift-Up/blob/master/bluetoothGPIO.py)



