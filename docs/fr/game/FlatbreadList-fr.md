# Feuille de route de The Native Pond

![flatbreadlist_background](/background/fr/FBL-docs-bg-fr.png)

> [!WARNING]
> 1. Tout le contenu de cette liste est de la poudre aux yeux — il ne représente ni la présentation finale ni l'implémentation réelle.
> 2. Une partie du contenu de cette liste n'a pas été discutée en réunion d'équipe.
> 3. Une partie du contenu de cette liste n'a pas fait l'objet d'une étude de faisabilité.
> 4. Cette liste peut servir de source d'inspiration pour les créations dérivées et les œuvres secondaires.
> 5. L'équipe de développement se réserve tous les droits sur les évolutions futures de cette liste, ainsi que l'interprétation finale de son contenu.

---

## 🎮 Système de contrôle

Des déplacements fluides et une bonne caméra sont essentiels pour garantir le plaisir de jeu. **Le personnage doit absolument pouvoir se déplacer !**

### Déplacements

- Le joueur contrôle son personnage qui se déplace dans la **carte** ; à des emplacements spéciaux (comme la plateforme de pêche), il **déclenche** l'animation d'entrée dans cet **emplacement spécial** en appuyant sur une touche ou en atteignant une petite zone de coordonnées autour de celui-ci.
- Le joueur **interagit** avec le jeu via les boutons tactiles (mobile), le clavier (bureau) et la manette ; les touches sont entièrement personnalisables.

### Point de vue

- La **troisième personne** est utilisée dans les zones ordinaires de la carte.
- La **première personne** est utilisée dans les emplacements spéciaux (comme la plateforme de pêche), avec l'affichage de leur intérieur (s'il existe).
- La carte **suit** le mouvement de la caméra.

---

## 🗺️ Système de carte

Étale-toi sur la table pour travailler sur la **carte** : on y trouve vraiment de tout !

### Zoom et orientation

- La carte ne peut pas **pivoter** avec la caméra.
- La carte peut être **zoomée**.
- La carte respecte la logique « **nord en haut, sud en bas, ouest à gauche, est à droite** ».

### Frontières

- La carte du jeu possède des **frontières** : le joueur ne peut pas franchir les **bords de la carte**.
- Quand le joueur tente de franchir une frontière, le jeu le **ramène de force** et affiche le message « * Une sensation familière monte en toi — tu sembles entendre : « Explorons la zone devant nous plus tard ! » Même si tu sais que tu ne pourras jamais l'explorer plus tard, tu veux quand même essayer. »
- Les frontières peuvent être des **obstacles naturels** évidents (comme de hautes montagnes) ou des **clôtures artificielles** (comme les murs de l'architecture de style Huizhou).

### Météo

- Voici les **types** de météo :
	- Ensoleillé.
	- Pluie.
	- Orage.
	- Neige.
- Les **changements** de météo peuvent dépendre de :
	1. D'un réglage manuel par le joueur.
	2. D'une similitude avec le climat d'un lieu donné.
	3. D'une probabilité entièrement aléatoire.

### Saisons

- Les saisons changent toutes les **90 heures**.
- Voici les **types** de saisons :
	- Printemps.
	- Été.
	- Automne.
	- Hiver.

### Caméra

- Le joueur peut **prendre des photos** à n'importe quel endroit (sauf dans les interfaces GUI) en appuyant sur une touche du clavier, en cliquant sur un bouton ou en pressant une touche de la manette.
- Pendant la **prise de photo**, le jeu affiche un **flash blanc** plein écran pour la symboliser. Il faudra peut-être ajouter un écran d'avertissement sur l'**épilepsie photosensible** à l'écran de démarrage du jeu.
- Pendant la **prise de photo**, le jeu **capture** automatiquement tous les éléments à l'écran (sauf les éléments GUI) et ajoute un **cadre photo**.
- Le jeu **enregistre** les photos dans un **dossier dédié** afin de les partager.

### Étang de pêche

- L'étang de pêche est l'emplacement spécial le plus central du jeu : il comprend la **plateforme de pêche**, l'**étang** et le **petit bateau**.

#### Plateforme de pêche

- Située à l'extrémité la plus au **sud** de l'étang.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, le personnage s'assoit, et l'interface visuelle de l'emplacement s'affiche.
- La plateforme sert à **pêcher**.

#### Étang

- Situé à l'extrémité la plus au **nord** de la carte.
- Quand le joueur **entre** dans cet emplacement spécial, le personnage passe en mode **nage**.

#### Petit bateau

- Il peut se trouver à **n'importe quel endroit** de l'étang (selon l'endroit où le joueur l'a laissé la dernière fois).
- Quand le joueur **entre** dans cet emplacement spécial, le personnage passe en mode **pilotage**, et l'interface visuelle de l'emplacement s'affiche.
- Le joueur peut naviguer sur l'**étang** à bord du petit bateau.

### Tente

- Située au **sud-ouest** du centre de la carte.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, et l'interface visuelle de l'emplacement s'affiche.
- La tente est le cœur du **camp**.
- L'**intérieur** et la **taille** de la tente peuvent s'inspirer du design de la tente de « Robinson Crusoé ».

### Champ

- Le champ se trouve au **sud-est** de la tente.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, et l'interface visuelle de l'emplacement s'affiche.
- Le champ sert à **cultiver**.

### Marché

- Le marché se trouve à l'**est** de la carte.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, et l'interface visuelle de l'emplacement s'affiche.
- Le marché sert à **échanger**.

### Arbre

- Situé au **sud-est** de la tente.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, et le personnage s'assoit.
- Des **pommes** apparaissent parfois dans l'arbre (par exemple en automne). Le joueur peut les faire tomber avec une **longue perche en bois** puis les **ramasser**.
- Après que le joueur est resté un moment sous l'**arbre** (environ 1 minute), le jeu affiche un bouton flottant « Maintenez [W] pour méditer » ; en appuyant sur W, en cliquant sur le bouton ou en pressant une touche de la manette, le joueur entre en **méditation**. Pendant la **méditation**, le jeu affiche des **effets visuels** plein écran (diverses formules de physique), et le joueur peut être frappé par une **pomme**.

### Feu de camp

- Situé non loin à l'**est** de la tente.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, et l'interface visuelle de l'emplacement s'affiche.
- Le feu de camp peut être **allumé** et fournit de la lumière.
- Le feu de camp peut servir à **cuisiner**.

### Conque magique

- Le joueur peut ramasser la **conque magique** sur la **plage** au bord de l'eau.
- Quand le joueur **ramasse** la conque magique, le personnage passe en position de souffle et la caméra zoome automatiquement. Le joueur ne peut plus se déplacer, et l'interface visuelle de cet objet spécial s'affiche.
- La conque magique offre **7 notes** au joueur.
- La conque magique possède plusieurs **variantes**, chacune avec un **timbre** différent.

### Boîte aux lettres

- Située au **sud** de la tente.
- Quand le joueur **entre** dans cet emplacement spécial, la caméra zoome automatiquement et passe en première personne, et l'interface visuelle de l'emplacement s'affiche.
- La boîte aux lettres sert à **recevoir et envoyer des courriers**.

---

## 🎣 Système de pêche

Sur la **plateforme de pêche**, le joueur peut utiliser une **canne à pêche**.

### Espèces

- L'**étang de pêche** du jeu permet d'attraper aussi bien des **espèces marines** que des **espèces d'eau douce**. Outre les poissons, il est aussi possible d'attraper des **objets de collection**.
	1. Cela pourrait dépendre de la **plateforme de pêche** choisie par le joueur (par exemple, une plateforme en bord de mer ne permet d'attraper que des espèces marines, et une plateforme au bord d'un lac, uniquement des espèces d'eau douce).
	2. Cela pourrait dépendre des **probabilités** propres à chaque espèce (sur une même plateforme en bord de mer, il serait ainsi possible d'attraper à la fois des espèces marines et d'eau douce selon les probabilités).
- La **probabilité** d'attraper chaque espèce dépend de :
	1. La probabilité réelle d'attraper chaque espèce **dans la vraie vie**. Il peut s'agir d'une fourchette de valeurs, ajustée selon divers facteurs (comme la météo ou la saison) plutôt que fixe.
	2. Une probabilité entièrement **aléatoire**.
- La **probabilité** d'attraper des objets de collection dépend de :
	1. L'historique du **taux de morsure** du joueur.
	2. Une probabilité **aléatoire** dans une fourchette fixe.
	3. Une probabilité entièrement **aléatoire**.

### Taux de morsure

À noter : le taux de morsure désigne la probabilité que le poisson **morde à l'hameçon**, et non la probabilité finale de l'attraper.

- Le **taux de morsure** du jeu est déterminé par l'ensemble des facteurs suivants :
	- La présence ou non d'appât sur l'hameçon du joueur.
	- Que le joueur ait amorcé ou non (jeté une amorce).
	- Le type d'appât sur l'hameçon.
	- L'heure du jeu (jour, nuit).
	- Que la lampe frontale soit allumée ou non la nuit.
	- La météo du jeu.
	- La saison du jeu.
- Le taux de morsure peut aussi dépendre de :
	1. L'historique du taux de morsure du joueur.
	2. Une probabilité entièrement aléatoire.

### Taux de capture

Comme son nom l'indique, le taux de capture désigne la probabilité finale d'attraper le poisson.

- Le **taux de capture** du jeu est déterminé par l'ensemble des facteurs suivants :
	- Que le poisson ait mordu à l'hameçon.
	- Le moment où le joueur ferre (ni trop tôt, ni trop tard).
	- Le taux de rupture du fil de pêche.
	- La taille de l'hameçon.

### La canne

- La canne se compose de la **hampe**, du **flotteur**, de l'**hameçon** et du **fil de pêche**.
- Chaque partie de la canne possède une **durabilité** : plus elle est basse, plus le risque de casse est élevé. Quand une partie casse, il faut la **remplacer**.

#### Hampe

- La **hampe** est un composant de la **canne**.
- Le joueur peut acheter des hampes via le **système de commerce**, par exemple une canne de 2,7 mètres ou une canne de 3,6 mètres.
- Les cannes de longueurs différentes ont des temps de lancer et de ferrage différents.

#### Flotteur

- Le **flotteur** est un composant de la **canne** ; le joueur décide de ferrer ou non selon le **mouvement du flotteur**.
- Le joueur peut acheter des flotteurs via le **système de commerce**, par exemple un flotteur ordinaire ou un flotteur lumineux.
- Chaque espèce de poisson provoque un mouvement de flotteur différent au moment de la morsure, en référence aux mouvements réels des flotteurs.
- Le flotteur peut être réglé sur différentes **hauteurs de ligne** (en ajustant le poids du plomb) pour faciliter l'observation.

#### Hameçon

- L'**hameçon** est un composant de la **canne** et la base de toute prise.
- Le joueur peut acheter des hameçons via le **système de commerce**, par exemple des hameçons de petite ou de grande taille.
- La taille de l'hameçon est déterminante pour attraper de gros ou de petits poissons.
- L'hameçon peut recevoir un **appât**.

#### Fil de pêche

- Le **fil de pêche** est un composant de la **canne**.
- Le joueur peut acheter des fils via le **système de commerce**, par exemple un fil ordinaire n° 0,8 ou un fil premium n° 2,0.
- Les fils ont des **taux de rupture** différents, déterminés par l'ensemble des facteurs suivants :
	- La qualité du fil.
	- La durée d'utilisation ou la durabilité du fil.

### Appâts

- Le joueur peut acheter des appâts via le **système de commerce**, par exemple un appât ordinaire ou des vers rouges.
- Si l'appât acheté est en poudre, il faut encore le transformer en appât en y ajoutant de l'eau et en le pétrissant.
- Chaque appât offre un **taux de morsure** différent.
- En tant que consommable, si le joueur n'a plus d'appât et que ses coquillages (y compris ceux gagnés en vendant ses prises) ne suffisent pas à acheter un paquet d'appâts, le jeu fournira gratuitement un réapprovisionnement le lendemain dans la **boîte aux lettres**.

### Amorces

- Le joueur peut acheter des amorces via le **système de commerce**, par exemple du marc de tofu fermenté ou du vieux maïs trempé dans l'alcool.
- Chaque amorce offre un **taux de morsure** différent.
- L'amorce peut considérablement augmenter le taux de morsure.

### Lampe frontale

- Le joueur peut acheter des lampes frontales via le **système de commerce**, par exemple une lampe ordinaire ou une lampe de nuit à lumière bleue.
- Chaque lampe offre un **taux de morsure** et un rendu visuel différents.
- La nuit, la lampe frontale permet de voir la surface de l'eau et le flotteur.
- La nuit, la lampe peut effrayer les poissons et faire baisser le taux de morsure.

### Objets de collection

- Les objets de collection se répartissent principalement entre **bouteilles à la dérive**, **souvenirs** et **fragments d'histoire**.
- Le joueur peut **obtenir** des objets de collection par les moyens suivants :
	- La pêche.
	- Les cadeaux de Cat.

#### Bouteilles à la dérive

- Les bouteilles à la dérive contiennent des **lettres**.
- La plupart de ces lettres sont des **messages réconfortants** destinés à encourager le joueur.

#### Souvenirs

- Certains souvenirs peuvent être **exposés** dans la **tente**.

#### Fragments d'histoire

- Les fragments d'histoire guident le joueur dans la découverte des récits des **villageois**.
- Une fois tous les fragments collectés, le joueur débloque une longue séquence narrative pour découvrir de manière complète et détaillée les histoires des **villageois**.

---

## 🍳 Système de cuisine

Prépare des **plats** et essaie de les manger !

### Ustensiles de cuisine

- Les ustensiles de cuisine se composent de trois parties : le **fourneau**, la **planche à découper** et les **outils de cuisine**.

#### Fourneau

- Le fourneau sert à **chauffer** les aliments.
- Le fourneau peut se **trouver** :
	1. À l'intérieur de la tente.
	2. À l'extérieur de la tente, mais à proximité.
- Le fourneau permet de poser certains **outils de cuisine** (comme une poêle).
- Avant d'utiliser le fourneau, il faut y ajouter du **combustible**.
- Le joueur doit **contrôler la cuisson** pour s'assurer que les plats soient comestibles.

#### Planche à découper

- La planche sert à **hacher** les aliments.
- Le joueur peut y poser certains **ingrédients** (comme le chou chinois) et des **préparations intermédiaires**.
- Le joueur peut découper sur la planche avec certains **outils** (comme un couteau de cuisine).

#### Outils de cuisine

- Les outils permettent au joueur de **traiter** facilement les ingrédients.
- Les outils comprennent :
	- La grande marmite.
	- La poêle.
	- Le panier vapeur.
	- Le bol en porcelaine.
	- Le couteau de cuisine.
	- Le rouleau à pâtisserie.

### Recettes

- Le joueur peut préparer des plats en suivant les **recettes**. En général, en respectant la recette, le plat réussit.
- Le joueur peut aussi **ne pas suivre** la recette et improviser.

### Plats

- Quand le joueur a accompli tout le **processus de préparation**, il obtient un **plat**.
- Le joueur peut préparer les plats suivants :
	- Les nouilles simples (obtenues après tout le processus, de la farine au pétrissage, en passant par la découpe des lanières et la cuisson).
	- Les petits pains farcis vapeur (obtenus après tout le processus : farine, pétrissage, étalage de la pâte, préparation de la garniture, façonnage et cuisson à la vapeur).
	- L'œuf au plat (obtenu après tout le processus : casser l'œuf, allumer le feu, retourner).
	- Le poisson grillé (obtenu en grillant le poisson au feu de camp).
	- L'objet indescriptible (obtenu quand la préparation échoue).
	- Le charbon (obtenu quand on ne suit pas la recette et que la préparation échoue).

### Dégustation

- Une fois le **plat** préparé, le joueur peut essayer de le manger.
- Pour manger, le joueur peut cliquer sur le **plat** concerné ou sur l'une de ses **parties**.
- Quand le joueur mange un **plat**, des **effets sonores** agréables, des **textes** réconfortants accompagnent la **disparition** animée du plat ou de ses parties.
- En particulier, manger un **objet indescriptible** peut déclencher l'une des situations suivantes :
	1. Le personnage s'évanouit, puis se réveille après un moment.
	2. Le personnage subit un effet visuel de nausée pendant un moment.
	3. Il ne se passe rien.

---

## ⛺️ Système de camp

Seule la **tente** apporte un vrai sentiment de sécurité !

### Stockage

- Dans la **tente**, le joueur peut consulter les **objets** qu'il possède.
- Les objets **possédés** par le joueur comprennent :
	- Les poissons.
	- Les objets de collection.
	- L'équipement de pêche.
	- Les cultures.
- Certains objets (comme certains objets de collection) peuvent être **exposés**.

### Succès

- Dans la **tente**, le joueur peut consulter les **succès** débloqués.

### Lit

- Au **coucher du soleil** et **la nuit**, le joueur peut **dormir** en cliquant sur le lit pour passer la nuit.
- Le joueur se réveille au **lever du soleil** ou dans la **matinée** du lendemain ; il peut aussi choisir de **dormir un peu plus**.

### Bac de recyclage des émotions

- Ce bac, semblable à une poubelle de recyclage, permet au joueur d'écrire les choses désagréables rencontrées dans sa **vie réelle**, de les froisser en boule et de les jeter dans le bac de recyclage des émotions !

### Journal

- Le joueur peut écrire dans le **journal** ce qu'il a vécu chaque jour (que ce soit dans le jeu ou dans la réalité).
- Le jeu permet d'exporter certaines pages du **journal** vers un **dossier dédié** pour les partager.

### Album

- L'album présente toutes les **œuvres** dessinées par le joueur sur du **papier à dessin**.
- L'album peut être exporté en entier dans un fichier unique vers un **dossier dédié** pour le partager.

---

## 🐚 Système de commerce

Ce melon est-il mûr ?

### Achat

- Le joueur peut acheter des marchandises au **marché**.
- Au marché, le joueur peut discuter avec des **villageois** de diverses professions.
- En **discutant** avec un villageois, une **scène spéciale** peut se déclencher ; la terminer permet d'obtenir une **réduction**.
- Le joueur peut acheter au marché les **types** de marchandises suivants :
	- L'équipement de pêche (comme les cannes).
	- Les graines de cultures (comme les graines de blé).
	- Les cultures transformées (comme la farine).
	- Les légumes (comme le chou chinois).
	- Le combustible (comme le charbon).
	- Les assaisonnements (comme le sel).
	- Le papier à dessin (comme le papier 1:1).
	- Les timbres.

### Vente

- Le joueur peut vendre des marchandises au **marché**.
- Le joueur peut vendre au marché les **types** de marchandises suivants :
	- Les poissons.
	- Certains objets de collection.
- Pour vendre des poissons, le prix est fixé selon le **prix du jour**.
- Le **prix du jour** se divise en deux tarifs — **poisson frais** et **poisson en stock** — et aucun des deux n'est figé. Il peut être déterminé par l'ensemble des facteurs suivants :
	- La météo du jeu.
	- La saison du jeu.
	- Une valeur aléatoire dans une fourchette fixe.

### Monnaie

- Le jeu utilise les **coquillages** comme monnaie.
- Le joueur peut **obtenir** des coquillages par les moyens suivants :
	- Le commerce.
	- La pêche.
	- Les cadeaux de Cat.

---

## 🌽 Système de cultures

**Cultive** tes cultures, **arrose-les et fume-les**, puis **récolte**.

### Plantation

- Pour cultiver, il faut posséder des **graines**.
- Le **processus** de plantation est le suivant : aplanir le sol, semer les graines, recouvrir de terre, arroser, fertiliser.
- Les conditions de germination : une **humidité adéquate**, une **température adaptée** et un **apport d'oxygène suffisant**.
- En plantant, le joueur doit **tenir compte** de :
	- La météo du jeu.
	- La saison du jeu.

### Croissance

- Pendant la croissance des cultures, le joueur doit **arroser** et **fertiliser** sans interruption.
- Toutes les quelques heures (environ 90 heures), les cultures **changent** de **stade de croissance**.

### Récolte

- Quand les cultures sont **totalement mûres**, le joueur peut récolter les **cultures** et les **graines**.

---

## 🐱 CatGPT

**Bavarde** avec le petit chat ou **caresse-le** ฅ՞•ﻌ•՞ฅ.

### Discussion

- Le joueur peut **envoyer des messages** à Cat.
- Cat **répond** selon certains critères de pondération, qui peuvent dépendre de :
	1. Le nombre de caractères envoyés par le joueur.
	2. Une probabilité entièrement aléatoire.
- Cat répond par des « **Meow** » de tons et de timbres variés, pour apporter une valeur émotionnelle au joueur.

### Caresses

- Le joueur peut caresser Cat en touchant doucement sa **tête**.
- En caressant Cat, des bulles « **Meow** » s'envolent de son corps, accompagnées de « **Meow** » de tons et de timbres variés pour apporter une valeur émotionnelle au joueur.

### Cadeaux

- Cat peut offrir un **cadeau** au joueur au petit matin du lendemain, à son réveil.
- Que Cat offre un **cadeau** ou non peut dépendre de :
	1. Le nombre de discussions ou de caresses avec Cat la veille.
	2. L'historique des discussions et des caresses avec Cat.
	3. Une probabilité entièrement aléatoire.
- Les **types** de cadeaux peuvent comprendre :
	- Des poissons.
	- Des coquillages.
	- Certains objets de collection (probabilité infime).

### Et aussi…

- Outre Cat, le joueur peut choisir d'autres **interlocuteurs** pour discuter ou caresser. Ces **autres interlocuteurs** pourraient être des **membres de l'équipe de développement** apparaissant dans les **scènes d'introduction**.

---

## 🖌️ Système de dessin

**Dessine** sur un papier et avec des peintures d'un réalisme saisissant, puis enregistre ton œuvre.

### Papier à dessin

- Le papier à dessin se comporte comme un vrai papier : il permet l'**estompage**, la **superposition de couches** et le **mélange des couleurs**.
- Le joueur peut acheter du papier via le **système de commerce**, par exemple du papier 1:1 ou du papier 3:4.

### Palette

- Huit couleurs de base sont proposées par défaut ; le joueur peut tremper le **pinceau** dans la peinture et mélanger les teintes sur la **palette**.
- La palette peut être à l'**aquarelle** ou à la **gouache**.
- En mélangeant, les deux couleurs se combinent via le **pinceau** ; les pigments non mélangés conservent leur teinte d'origine, et la teinte obtenue dépend du degré de mélange du joueur.

### Pinceau

- Le pinceau permet d'**appliquer** de la peinture ou de l'eau sur le papier.

### Enregistrement

- Les œuvres du joueur sont **enregistrées** dans l'**album**.
- Le joueur peut **exporter** ses œuvres vers un **dossier dédié** pour les partager.

---

## 📬 Système de boîte aux lettres

Recevoir et envoyer des **courriers**.

### Réception

- Le joueur peut **recevoir** les courriers suivants :
	- Des lettres que le joueur s'est envoyées à lui-même.
	- Un réapprovisionnement gratuit d'appâts.
	- Des vœux de fête.
	- Des vœux d'anniversaire.

### Envoi

- Le joueur peut **envoyer** les courriers suivants :
	- Des lettres adressées à son futur soi.
- Pour envoyer un courrier, il faut y apposer un **timbre**.

---

## 📺 Interface visuelle

Des **animations non linéaires** fluides offrent toujours une belle expérience visuelle au joueur.

### Contrôles

- Les contrôles permettent de **déclencher** des comportements d'interaction et des événements.
- Les contrôles doivent conserver le même style de design que « Today@PolarBay ».
- Quand on **appuie** sur un contrôle, il doit rétrécir instantanément, puis rebondir de manière non linéaire.
- La **position** et la **taille** des contrôles sont personnalisables.

### Cartes

- Les cartes ne sont pas **interactives**.
- Les cartes doivent conserver le même style de design que « Today@PolarBay ».
- Les cartes servent à afficher des arrière-plans relativement **épurés**, comme l'interface de l'inventaire.

### Écran vert protecteur des yeux

- Comme le joueur doit **fixer longtemps** le **flotteur** pendant la **pêche**, un **écran vert protecteur des yeux** a été spécialement conçu.
- L'écran vert **recouvre tout l'écran** à intervalles réguliers pour **imposer une pause** au joueur.
- L'**intervalle** et la **durée d'affichage** de l'écran vert sont réglables ou désactivables dans les paramètres.
- L'écran vert affiche le contenu des **lettres** des **bouteilles à la dérive** déjà collectées par le joueur.

### Thèmes de couleurs

- Le jeu pourrait intégrer **deux thèmes** de couleurs : un thème blanc et un thème noir.
- Le **passage** de l'un à l'autre peut se faire selon les conditions suivantes :
	1. Le jour et la nuit dans la réalité.
	2. Le jour et la nuit dans le jeu.
	3. Un réglage manuel par le joueur dans les paramètres.

### Effets de particules

- Les effets de particules naissent d'**événements spéciaux**, comme la navigation du bateau sur l'eau.
- Leur quantité et leur activation peuvent être réglées dans les **paramètres**, pour éviter tout problème de performance.

### Matériaux avancés

- Les matériaux avancés, c'est-à-dire les matériaux en **acrylique**.
- Le joueur peut activer ou désactiver les matériaux avancés dans les **paramètres**.
- Une fois activés, les **espaces vides** des GUI (contrôles, cartes, etc.) deviennent des matériaux translucides et flous.

---

## 🕒 Système de temps

Le **temps** passe toujours si vite que nous manquons bien des choses.

### Conversion du temps

- Un **jour** dans le jeu équivaut à **une heure** dans la réalité.
- Le rapport de conversion entre le temps du jeu et le temps réel est de **1:24**.

### Tranches horaires

- Le **jour** et la **nuit** durent chacun **30 minutes** dans le jeu.
- Au cours d'une **journée** (60 minutes), les tranches horaires du jeu sont réparties comme suit :
	- Lever du soleil : minutes 1-2.
	- Matin : minutes 2-10.
	- Midi : minutes 11-20.
	- Après-midi : minutes 21-28.
	- Coucher du soleil : minutes 29-30.
	- Nuit : minutes 31-60.

---

## 💾 Système de sauvegarde

**Sauvegarde** ta **progression** actuelle pour que nos poissons et notre sel soient en sécurité.

### Sauvegarde

- Sur la page **Sauvegarde**, le joueur peut cliquer sur le bouton **Obtenir une sauvegarde** pour **enregistrer** sa progression actuelle.
- Sur la page **Sauvegarde**, le joueur peut cliquer sur le bouton **Charger une sauvegarde** pour **charger** une sauvegarde existante.
