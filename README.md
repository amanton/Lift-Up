# Projet - Lift up

_Lift-Up has been created and designed for people who can't stand up by themselves as persons with mild motor disabilities. With his simplistic design, he can be placed everywhere without attracting attention. It is commanded with Bluetooth, allowing an easier control. Warning, Lift-Up is not made for (general) public with average motor impairment or more.
All the system is run by a Raspberry Pi 3._

[Presentations slide](https://docs.google.com/presentation/d/1F90I4jqLM0xJeXBUU_vE5x2pX4bnX4WyPgPFGB-84LE/edit?usp=sharing)


## Présentation


__Lift up__ a été imaginée et conçue pour les personnes avec _un léger handicap moteur_. Beaucoup de personnes ne peuvent pas ou ont du mal à se relever lorsqu'elles sont assises sur une chaise, et donc pour ces personnes là, on a voulu créer un prototype de chaise autonome et ayantl'aspect d'une chaise ordinaire __qui pourrait donc être placée dans les restaurants__ pour que ces personnes puissent manger au restaurant __sans aide pour se relever__.

Le projet ne peut malheureusement pas être adapté pour les personnes ayant un gros handicap moteur.

Pourquoi sommes-nous allés vers ce projet ? 

>je connais plusieurs personnes qui souffrent au niveau des jambes, et ce qui m'a le plus marqué c'est mon grand-père qui aime beaucoup aller au restaurant, mais depuis quelques années il ne veut plus y aller car il se __sent gêné pour demander de l'aide pour le relever d'une chaise__, comme il existe déjà des sièges et fauteuils qui aident à se relever, pourquoi des chaises fines ne peuvent pas le faire aussi ? 
>>Richard

En partant de cette question, le projet est né et les schémas ont commencé à être imaginés.


## Choix du Projet


Il y avait plusieurs styles de chaise possible, la première aurait été de faire __une chaise totalement automatisée avec des rails__ pour qu'elles n'aient pas à forcer, sauf que ce type avait des défauts, elle aurait été __très peu maniable__ pour les restaurateurs et les rails auraient pu fait tomber une personne. Donc personnes ne l'aurait achetée.

Une version similaire a vu le jour dans nos têtes juste après, __remplacer les rails par des roues__, sauf que comme l'exemple du grand-père de richard, il a honte qu'on le voit avoir besoin d'aide, donc voir des roues sous une chaise serait la preuve qu'il a besoin d'aide. Mais aussi des problèmes techniques, car il faudrait gérer les roues pour éviter que la chaise glisse ou se retourne due à un centre de gravité mal géré. Et si les roues étaient motorisées, il faudrait vérifier s'il y a un obstacle derrière la chaise et si oui, ne pas reculer. On est donc partis sur le troisième modèle qui est qu'on __garde l'architecture basique d'une chaise__, on rajoute un moteur ou des piston en dessous les plus discrets possible, la personne devra certes faire un peu plus d'effort que les 2 autres chaises citées au-dessus, mais __la chaise sera pratiquement la même que les autres dans le restaurant__, et c'est vraiment le __but du projet__.

Bon, partant de cette idée, on avait deux choix qui s'ouvraient à nous :
* Faire une maquette puis essayer de faire une chaise grandeur nature. 
* Faire un prototype fonctionnel pour sa taille.

On est partis pour un prototype fonctionnelle, car nous n'avions ni le temps, ni les moyens financiers pour un tel projet. 


## Brainstorm


Le projet était donc lancé, nous avons quand même regardé sur le net si des chaises de ce style existaient dans le marchés, mais sans grande trouvaille, un seul produit nous reste en tête 
[Coussin d'aide à la levée](https://www.tousergo.com/aide-au-transfert/28-coussin-d-aide-a-la-levee-3574590140219.html).
Comme prévu pratiquement aucune société ne fait de chaise de ce style, les sociétés préfèrent viser le marché des fauteuils par rapport aux chaises.

Nous avons réfléchi à plusieurs idées permettant de faire monter le siège d'une chaise :

1. La première idée fut les pistons, simples.
2. La deuxième était de passer par une [vis sans fin](https://upload.wikimedia.org/wikipedia/commons/b/b8/Vis100f1.png) qui est un engrenage et une vis.  
3. La troisième était de passer via un engrenage et une crémaillère, moins robuste, mais efficace.

La première est très efficace, mais chère et dangereuse si elle est mal programmée (_elle pourrait éjecter la personne contre la table ou son voisin d'en face_). La deuxième peut soulever une importante charge et de manière précise, mais est impossible due à l'irréversibilité de la vis sans fin, car on ne pouvait pas placer la vis de la manière voulue due a la présence du moteur qui bloquait la crémaillère. La troisième est fonctionnelle et efficace, mais dépendante de la matière dont est constituée la crémaillère ainsi qu'à la fixation entre la crémaillère et le siège de la chaise, car si le poids et trop important, soit la crémaillère cède sous le poids ou bien la crémaillère perfore le siège si la force est trop importante.  

Nous avons donc choisit de passer par la troisième méthode.

![](https://zupimages.net/up/19/20/yr36.png) ![](https://zupimages.net/up/19/20/filr.png) ![](https://zupimages.net/up/19/20/6vpy.png)

## Fabrication

### Construction

Notre première question pour la construction du projet était de savoir si on allait construire la chaise entièrement ou si nous prendrions un kit d'une chaise chez un fabricant. Comme le temps nous manquait un peu, nous avons opté pour choisir une petite [chaise](https://www.ikea.com/fr/fr/p/kritter-chaise-enfant-rouge-80153697/)
 chez le leader IKEA, ceci fait nous a beaucoup facilité la tâche, car il nous rester qu'a ajuster la chaise pour qu'elle soit fonctionnelle avec notre projet.


Une chaise est complexe à créer, plusieurs critères liés à la conception pour le confort sont très précis : 
1.  __La hauteur d'assise__
	>C'est la mesure qui sépare le sol de la surface sur laquelle nous sommes assis. Elle correspond à la longueur moyenne de l'arrière d'une jambe, depuis le pli du genou jusqu'au talon, chaussure comprise. Pour les chaises devant servir à prendre des repas autour d'une table ou à travailler à un bureau, elle est de nos jours de 450 mm. Il est éventuellement possible de porter cette mesure à 460, voire 470 mm et rien n'interdit de la baisser jusqu'à 440 mm.
	>>Fabrication d'une chaise: le confort d'une assise
2. __Les dimensions de l'assise__
	>Une assise profonde et large offre un plus grand confort qu'une même assise aux dimensions réduites. Il est cependant inutile d'en exagérer les mesures, car l'encombrement de la chaise deviendra une gêne plus qu'un élément de confort. Sa largeur peut ainsi varier de 400 à 480 mm et sa profondeur de 360 à 410 mm. Des mesures inférieures vont au détriment du confort.
	>>Fabrication d'une chaise: le confort d'une assise
3. __La nature de l'assise__
	>Nous avons tous ressenti un jour la sensation désagréable d'être assis sur une chaise trop dure, mal paillée ou mal rembourrée. Il est alors impossible de rester immobile et de se détendre. C'est donc un point qu'il faut aborder avec attention. Une assise peut être en bois nu et offrir une assise confortable à condition de lui donner une forme en creux bien particulière. Celle en bois massif d'une chaise de style Windsor en est un exemple.
	>>Fabrication d'une chaise: le confort d'une assise


![](https://zupimages.net/up/19/20/uzdp.jpg "Schéma d'une chaise")
>[Schéma d'une chaise](http://www.ikonet.com/fr/ledictionnairevisuel/maison/ameublement-de-la-maison/chaise/parties.php)

Comme c'est un prototype, il se doit d'être peu coûteux. Donc nous avons choisi de fabriquer la crémaillère en plastique imprimer avec une imprimante 3D. L'engrenage a aussi été imprimé en 3D pour qu'il s'emboîte parfaitement ainsi qu'un bloc pour les contenir et qu'il reste assemblés.Les pièces étant uniques nous avons due les modéliser en 3D. 

Nous avons utilisé le site [Tinkercad](https://www.tinkercad.com) pour la modélisation qui est aussi une application disponible sur Windows via le store. Cette application est produite par la société [Autodesk](https://fr.wikipedia.org/wiki/Autodesk).

>Tinkercad est un outil gratuit et convivial pour la conception 3D, l'électronique et le codage. Il permet aux enseignants, aux enfants, aux amateurs et aux concepteurs d'imaginer, de concevoir et de fabriquer sans limites.

Vous pouvez voir [ici](https://www.tinkercad.com/things/dY0HXlwu65n) les pièces modélisées pour le premier test et [ici](https://www.tinkercad.com/things/2Bs0kqwbqwV) les pièces utilisées pour le montage final. Seules ces dernières on été imprimées.

Les pièces modélisaient sont :
* Crémaillère
* Un engrenage
* Un support moteur

La crémaillère servira à soulever le siège, elle sera propulsée via l'engrenage qui sera dans son support permettant à l'engrenage et la crémaillère d'être en contact, le servomoteur se rajoute au support pour actionner le tout, ils sont enveloppés par un boîtier pour protéger le tout, le boîtier inclus des trous sur 2 extrémités pour insérer un support (bâton en bois) pour avoir une liberté d'axe.


Quand nous avons reçu la chaise, nous avons commencer les modifications dessus, pour la rendre "compatible" avec notre système, nous avons troué certain partie, retirer quelques parties aussi, mais nous avons surtout poncer beaucoup de partie que se soit de la chaise ou des pièces imprimé en 3d, rien de très compliquer, ça prend juste un peu de temps et de patience, la chaise avancer donc très bien pendant le temps du développement.

### Programmation

Lors de l'avancement une partie programmation étais présente. Nous avons dû programmer de l'Arduino (qui est proche du C et du C++), comme nous ne sommes pas expert en Arduino, nous avons commencé à regarder les librairies disponibles pour le fonctionnement d'un servomoteur, et surtout du Bluetooth.

>Une carte Arduino est une petite carte électronique équipée d'un micro-contrôleur. Le micro-contrôleur permet, à partir d'événements détectés par des capteurs, de programmer et commander des actionneurs ; la carte Arduino est donc une interface programmable. La carte Arduino la plus utilisée est la carte Arduino Uno.
>>Découverte des cartes Arduino

On a donc appris ou du moins essayer de programmer en Arduino, après plusieurs séances a tester les fonctionnalités que nous offre les librairies, on a commencé à s'intéresser au fonctionnement des Connecteurs pour gérer les entrées et les sorties numériques. Les signaux transmirent par ces connecteurs sont des signaux logiques, c'est-à-dire qu'ils ne peuvent prendre que deux états : HAUT (5 Volts) ou BAS (0 Volt), par rapport au connecteur de masse GND, qui lui est toujours, par définition, à 0 Volt. Il existe aussi des entrées analogique qui peuvent aussi prendre que 2 état , mais peuvent admettre 1024 valeurs comprises entre 0 et 5 Volts, ces entrées servent à faire varier la luminosité d'une del par exemple.

L'IDE (_Integrated Development Environment ou Environnement de développement_) Blockly Arduino est bien pour une introduction à l'Arduino pour les personnes qui apprennent l'informatique comme Scratch. Mais pour des personnes qui on l'habitude de coder, c'est contre-intuitif, car on passe son temps à vouloir ajouter des lignes de code simple, or, c'est impossible. Donc on passe notre temps à faire du copier-coller des blocks dans l'IDE d'Arduino. Mais vous allez nous dire de directement coder sur l'IDE d'Arduino sauf que pour utiliser les servomoteurs, ils faut des importer des bibliothèques qui sont intégrer à IDE Blockly Arduino. Ainsi pour se simplifier la vie Aziz a copier la bibliothèque directement dans l'IDE d'Arduino.

Suite à plusieurs dizaines d'heures à essayer de faire fonctionner le Bluetooth sur la carte Arduino, même avec l'aide d'un professeur, la carte ne voulais rien savoir. Nous avons mis en place une application Android qui n'a pas abouti, car au début, on croyait que le fait que l'Arduino ne recevait pas les données venais de notre application, vous pouvez accéder au code [ici](https://github.com/DeadMeon/Lift-Up/blob/master/Test_Applcation_Android/main/java/com/example/devicelist/MainActivity.java).

>Le Raspberry pi est un nano ordinateur de la taille d'une carte de crédit que l'on peut brancher à un écran et utilisé comme un ordinateur standard. Sa petite taille, et son prix intéressant fait du Raspberry pi un produit idéal pour tester différentes choses
>>Qu'est ce qu'un Raspberry Pi ?

Une première version du code python vu le jour, la chaise se levais et redescendais tout été parfait ! Mais un jour plus rien n'était parfait nous avons donc décider de passer le projet que sur un unique Raspberry et nous avons fait nos adieux à l'Arduino qui nous a poser beaucoup de soucis, mais le Raspberry nous posa aussi beaucoup de soucis, du moins une libraire python nous causa beaucoup de soucis,

`import RPi.GPIO as GPIO`

>Un connecteur GPIO offre à une carte électronique la possibilité de communiquer avec d'autres circuits électroniques. Le GPIO est très présent dans les domaine de l'informatique, principalement embarquée, l'électronique, l'automatisme, la commande numérique, ou la robotique.
>>General Purpose Input/Output

Nous avons donc décider d'abandonner le Bluetooth via l'Arduino pour nous consacrer sur le Raspberry, nous avons donc commencer de la programmation python, nous sommes déjà un plus apte à être sur ce langage ayant appris les bases lors de notre année au début le Raspberry servais juste de relais pour envoyer des donner a l'Arduino, voici le code de [l'Arduino](https://github.com/DeadMeon/Lift-Up/blob/master/1erCodeArduino.ino).

Cette librairie nous a causé beaucoup de problème, nous ne comprenions pas la logique derrière certaines fonctions, même avec des tutoriels que se soit textuel ou même vidéo, le servomoteur réagissais de manière illogique, une fois, il tourner vers la droite, mais après il tourner à gauche alors qu'on avait rien changer dans le code, nous ne savons toujours pas pourquoi le servomoteur réagissait de cette manière, nous pensons peut-être à un problème de compatibilité avec notre servomoteur, mais nous ne pouvons pas l'affirmer.

`from gpiozero import AngularServo`

>Extends Servo and represents a rotational PWM-controlled servo motor which can be set to particular angles (assuming valid minimum and maximum angles are provided to the constructor). Connect a power source (e.g. a battery pack or the 5V pin) to the power cable of the servo (this is typically colored red); connect the ground cable of the servo (typically colored black or brown) to the negative of your battery pack, or a GND pin; connect the final cable (typically colored white or orange) to the GPIO pin you wish to use for controlling the servo.
>>14. API - Output Devices

gpiozero et donc la librairie que nous avons utiliser, mais nous avons surtout utilisé AngularServo, avec cette nouvelle librairie nous avons réussie à faire un prototype fonctionnel de notre chaise, vous pouvez voir le code python [ici](https://github.com/DeadMeon/Lift-Up/blob/master/bluetoothGPIO.py). Le fait de passer le projet que sur un Raspberry a un énorme avantage, on se limite qu'a un langage de programmation, l'alimentation est très simple, car juste une batterie externe suffit pour que le tout fonctionne, et surtout ça prend moins de place et donc beaucoup plus simple a cacher

## Les difficultés

Les plus grosses difficultés rencontrées dans ce projet ont été le caprice que nous a fait l'Arduino, la librairie pas compatible avec notre moteur sur Python, et la modélisation des pièce 3d , pas de grosse difficulté nous on retarder juste des imprévue de temps en temps, mais rien de bien méchant;

La chaise est fonctionelle, mais elle n'est pas parfaite, des améliorations, peuvent etre envisager, que se soit materielle ou même application. Un des premiers ajouts qu'on pourrait faire, c'est un bouton sur la chaise pour donner plus de choix d'utilisation, car les personne agées n'ont pas tous un téléphone, ou même certaine ne savent pas utilisé le Bluetooth, on pourrait aussi créer une télécommande pour simplifier l'utilisation à distance. 

Notre moyen, de faire monter le siège de la chaise n'est pas parfait, il est utile pour les personnes ayant un léger handicap moteur, car la chaise va les aider et ils pourront prendre appuie dès qu'ils le veulent, mais pour les personnes ayant un handicap moteur assez élevé, notre système n'est pas du tout conseillée, car il y a des risques que la personne glisse si ses appuis ne sont pas pris.

Comme prévu n'étant pas des ingénieurs, nous n'avions pas toutes les compétences pour réaliser le projet avec un modèle réel et surtout nous avions pas le budget, la chaise a donc de petit défaut, comme le support moteur qui empêche la fermeture complète de la chaise, car la chaise est trop petite, mais ce souci devrait être réglé si nous passons sur une tailles grandeur nature.

## En Conclusion

Pour conclure, nous sommes fiers de présenter ce projet, c'est un projet qui nous tient a Coeur, essayer de donner une autonomie aux personnes qui la perde suite aux faiblesses de leur corps. C'est un monde qui n'est pas exploité par les sociétés et nous ne comprenons pas, c'est certes peut être très complexe si on veut associer la puissance des moteurs avec l'esthétique d'une chaise et le confort aussi, car il est vrai que nous n'avons pas du tout prêter attention au confort. Nous n'avions qu'une chaise en bois pour enfant, nous ne pouvions pas trop comparer, ce projet prouve que ce n'est pas impossible comme idée et que de nombreuses sociétés pourraient démocratiser ce domaine pour le bien des personnes dans le besoin. 

Les sociétés trouvent que ce marché est de niche ainsi, ils ne chercheront jamais à cibler cette problématique qui ne leur rapportera pas assez d'argent. Donc les recherches sur ce sujet ne sont pas en évolution, et même si une marque décide d'en sortir une, il y a fort à parier que le produit soit trop cher pour les personnes dans le besoin, vu le manque de concurrence. 

Le projet ne peut malheureusement pas être adapté pour les personnes ayant un gros handicap moteur, car la chaise aide juste la personne à se relever, donc il faut que la personne ait un minimum de force dans les jambes.

## Bibliographie

* Ben Nuttall*.14. API - Output Devices, 03/04/2017, [https://gpiozero.readthedocs.io/en/stable/api_output.html], (05/04/2019).

* GRAFIKART*. Qu'est ce qu'un Raspberry Pi ?, 23/10/2015, [https://www.grafikart.fr/blog/raspberry-pi-utilisation], (15, 02, 2019).

* C. Fréou et A. Grimault*. Découverte des cartes Arduino, 08/04/2016, [http://www.techmania.fr/arduino/Decouverte_arduino.pdf], (15, 02, 2019).

* Wikipédia, General Purpose Input/Output, 31/03/2019, [https://fr.wikipedia.org/wiki/General_Purpose_Input/Output], (20/04/2019).

* Claude Gomi, Le Bouvet*, Fabrication d'une chaise: le confort d'une assise, 03/05/2009, [http://www.ideesmaison.com/Bricolage/Fiches-bricos/Bois/Fabriquer-du-mobilier/Fabrication-de-chaises/Les-elements-de-confort.html], (01/05/2019).

* Mathieu Nebra*, Rédigez en Markdown !, 29/11/2017, [https://openclassrooms.com/fr/courses/1304236-redigez-en-markdown], (29/04/2019).

