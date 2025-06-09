# Rapport mini-projet

Étudiants : Lucas Charbonnier, Cristhian Ronquillo, Vicky Butty

## Sujet choisi

**Projet 5: Génomes Mitochondriaux**
- Comparer, pour les espèces S. Pombe et S. Cerevisiae, les caractéristiques de leurs génomes mitochondriaux (mtDNA)
- Extraire les gènes codants et leurs annotations
- Extraire et visualiser des statistiques comme la taille, composition en bases, nombre de gènes codants, etc
- Identifier les voies métaboliques impliquées dans la digestion du glucose en aérobie (respiration) ou anaérobie (fermentation) et placer les gènes mitochondriaux dans ce contexte
- Présenter les résultats

## Contexte

Les levures à analyser, *S. Pompe* et *S. Cerevisiae*, aussi connues sous les noms respectifs de "levure de fission" et "levure de boulangerie", sont deux organismes très documentés et souvent exminées en laboratoire pour comprendre le fonctionnement du vivant.

L'être humain a démontré à de nombreuses reprises son obsession pour la pratique consistant à "laisser traîner accidentellement" des préparations dans des récipients fermés, ce qui a conduit à la création de nombreux produits : 
- Le pain : Les levures consomment le sucre contenu dans la pâte et produisent du Co2, ce qui permet de faire lever la pâte et donner au pain une texture aérée, au lieu d'une simple galette.
- Le fromage : Les levures jouent un rôle clé durant l'affinage de certains fromages.
- Boissons alcoolisées : Les levures sont à la base de nombreuses boissons alcoolisées car elles produisent de l'alcool suite à la consommation du sucre (glucose). 
- Le kéfir : C'est une boisson à base d'eau (ou de lait) faite à partir de grain de kéfir (combinaison de levures et bactéries lactiques).
- Le kimchi : Élément important de la cuisine coréenne, la préparation du kimchi consiste à laisser fermenter du chou chinois dans de la saumure pendant plusieurs semaines. 
- La kombucha : La kombucha est préparée à partir d'une culture de levures et bactéries plongées dans un mélange sucré (généralement du thé noir).
- En boulangerie, les levures sont utilisées pour faire lever la pâte. Durant la fermentation, les cellules consomme le sucre et produisent du Co2. Combiné à l'elasticité que procure le gluten, cela a pour effet de faire gonfler la pâte et d'obtenir une texture aérée.

Mis à part les préparations culinaires, les levures sont également utilisées dans la création de produits pharmaceutiques. Le principe repose sur la modification du génome d'une levure pour qu'elle synthétise une molécule spécifique. Par exemple, des biologistes ont réussi à faire en sorte que des levures synthétise de la psylocybine. Une molécule qui serait généralement assez compliquée à obtenir car elle nécessiterait de faire pousser des champignons pour en extraire le principe actif. C'est donc un gain de temps impressionnant.

## Analyse des voies métaboliques de digestion du glucose

Dans cette section, nous analyserons les voies métaboliques impliquées dans la digestion du glucose pour les deux levure en question. Nous contextualiserons ensuite les gènes trouvés aux étapes précédentes afin d'identifier leur utilité dans ces voies métaboliques. Plus particulièrement, il faudra comparer les différences entre les voies métaboliques de ces deux levures et les deux modes de métabolisation (aérobie et anaérobie).

### Qu'est-ce qu'une voie métabolique ?

Une voie métabolique est l'ensemble des réactions chimiques impliquées dans la transformation d'une molécule en une autre au sein d'un être vivant. Cette transformation s'effectue au moyen d'enzymes.
Dans notre cas, il s'agira d'analyser les voies métaboliques permetttant de digérer le glucose pour en tirer de l'énergie (ATP).

### Différents modes de métabolisation

***Métabolisme en aérobie*** : Lorsque les levures disposent de glucose **et** d'oxygène, elles produisent du Co2.
***Métabolisme en anaérobie*** : Lorsque les levures disposent de glucose mais pas d'oxygène, elles produisent du Co2 **et** de l'éthanol. C'est pour cette raison que la fermentation dans le but de créer des boissons alcoolisées se fait généralement dans des récipients fermés (également pour éviter les contaminations).

Sous certaines conditions, les levures peuvent métaboliser le sucre de manière anaérobique même en présence d'oxygène. Cet effet est connu sous le nom d'effet "***Crabtree***". Lorsque l'organisme se trouve dans un environnement avec une forte teneur en glucose, la respiration (métabolisation aérobique) serait inhibée et la fermentation (anaérobie) prendra le dessus.

### Voies métaboliques de digestion du glucose

Cette section décrit les différentes voies métaboliques impliquées dans la digestion du glucose ainsi que leur rôle.

#### Glycolyse
La Glycolyse (ou voie d'Embden-Meyerhof-Parnas) est la première étape de la digestion du glucose. Ici, les molécules de glucose sont "cassées" en deux et elles sont converties en pyruvate. Un petit peu d'ATP est déjà produit durant ce processus. Cette voie métabolique est commune à la respiration et à la fermentation. Pour que la glycolyse puisse s'effectuer, la cellule a besoin de glucose et de NAD+. Le NAD+ peut-être synthétisé par la cellule (à partir de vitamine B3) ou lors de la fermentation, en recyclant le NADH en trop (voir ci-dessous).

#### Fermentation
En cas de fermentation, donc en l'absence d'oxygène, la voie métabolique utilisée est celle de la **fermentation alcoolique**. La fermentation alcoolique, au travers de multiples réactions chimiques et de l'utilisation de plusieurs enzymes différentes, prend le pyruvate issu de la glycolyse et produit 2 choses :
1. De l'alcool (éthanol)
2. **Du NAD+**

À proprement parler, la fermentation ne permet pas de créer plus d'énergie. Cela dit, elle produit du NAD+, ce qui permet de faire en sorte que la glycolyse s'effectue à nouveau. C'est avantageux car le NAD+ nécessite habituellement d'être synthétisé à partir de la vitamine B3 et est donc relativement difficile à obtenir. La fermentation permet donc de sauter cette étape et d'effectuer la glycolyse en continu.

#### Respiration
En présence d'oxygène, 3 voies métaboliques supplémentaires doivent être traversées afin de produire de l'ATP :
1. Décarboxylation du pyruvate -> Prépare le pyruvate obtenu à partir de la glycolyse pour le cycle de Krebs
2. Cycle de Krebs -> produit du NADH à partir du pyruvate
3. Phosphorylation oxydative -> Convertit le NADH en ATP

#### Cycle de Krebs
Cycle de Krebs (aussi appelé cycle des acides tricarboxyliques) 
- voie des pentoses phosphates (ou voie de Warburg-Dickens-Horecker) -> TODO
- Phosphorylation oxydative -> permet la conversion de l'ADP en ATP

### Comparaison génétique de S. Pompe et S. Cerevisiae

![alt text](genes.png)

Les gènes atp6, atp8, atp9, cox1, cox2, cox3, rps3 sont communs aux deux espèces et sont relatifs à la dernière voie métabolique de digestion du glucose; la phosphorylation oxydative. C'est cette dernière réaction qui permet de convertir le NADH en ATP.

Les gènes CYTB et COB respectivement spécifiques à S. Cerevisiae et S. Pombe servent tout deux à coder la protéine **apocytochrome b** qui un rôle important dans la respiration.

Les gènes COB-I1 COX1-I1b et COX1-I2b servent à (lire deux dernières sources)

TODO
TODO
TODO

# Comparaison des protéines mitochondriales homologues entre S. pombe et S. cerevisiae

Nous comparons les protéines mitochondriales de deux espèces de levures : Schizosaccharomyces pombe et Saccharomyces cerevisiae. L’objectif est de voir à quel point leurs protéines sont similaires, en particulier celles qui jouent un rôle dans la production d’énergie à l’intérieur de la cellule.

Pour cela, nous utilisons l’outil EMBOSS Needle, qui permet d’aligner deux séquences de protéines du début à la fin. Cet alignement global est utile pour comparer des protéines de même type (dites « homologues ») et voir si elles ont évolué de manière similaire. Si deux protéines sont très proches, cela peut indiquer qu’elles assurent encore la même fonction, malgré les différences entre les espèces.

Nous avons sélectionné sept protéines présentes dans les deux espèces : atp6, atp8, atp9, cox1, cox2, cox3 et rps3. Les six premières participent à la respiration cellulaire, c’est-à-dire à la fabrication d’ATP, la molécule qui fournit de l’énergie à la cellule. Rps3 joue un rôle dans la fabrication des protéines à l’intérieur de la mitochondrie. En comparant ces protéines, nous cherchons à mieux comprendre leur conservation et leur importance pour le fonctionnement de la cellule.

Cette analyse nous aidera à voir si ces deux espèces, qui utilisent différemment le glucose selon qu’il y ait ou non de l’oxygène, partagent encore des bases communes dans la manière dont elles produisent leur énergie.

## Protéine atp6

### 1. Alignement global

| **Critère**          | **Valeur**             | **Interprétation**                                                                 |
| -------------------- | ---------------------- | ---------------------------------------------------------------------------------- |
| **Longueur alignée** | 271 aa                 | Longueur totale de la protéine alignée chez les deux espèces                       |
| **Identité**         | 119 / 271 (**43.9 %**) | Moins de la moitié des acides aminés sont strictement identiques                   |
| **Similarité**       | 171 / 271 (**63.1 %**) | La majorité des substitutions conservent des propriétés chimiques proches          |
| **Gaps (indels)**    | 26 / 271 (**9.6 %**)   | Des insertions/délétions dans les boucles, sans perturber les régions essentielles |
| **Score**            | 571.5                  | Score élevé malgré une divergence modérée : structure probablement conservée       |

---

### 2. Comparaison de la fonction

**Fonction déclarée pour les deux espèces** (selon UniProt) :
ATP6 est une sous-unité essentielle du domaine **F₀** de l’ATP synthase mitochondriale. Elle participe à la formation du **canal à protons**, permettant le couplage entre le passage des H⁺ et la synthèse d’ATP par le domaine catalytique F₁.

Les deux descriptions sont **identiques**, ce qui confirme une **fonction biochimique partagée**.  
Elle est indispensable à la **respiration cellulaire aérobie** et à la production d’énergie chez les eucaryotes.  

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| --------------- | ---------- |
| ![ATP6\_cerevisiae](./figures/atp6/cerevisiae.png) | ![ATP6\_pombe](./figures/atp6/pombe.png) |

Les deux structures AlphaFold montrent une organisation **quasi identique** :

* **Dix hélices transmembranaires** alignées en cylindre.
* Les variations se limitent aux **boucles périphériques** (parties non transmembranaires).
* L’axe central du canal à protons reste **parfaitement conservé**.

Cela confirme que, malgré une divergence de séquence, **la structure 3D et la fonction de canal sont préservées**.

---

### 4. Impact fonctionnel

| Espèce          | Stratégie métabolique                     | Implication sur ATP6                                                        |
| --------------- | ----------------------------------------- | --------------------------------------------------------------------------- |
| *S. cerevisiae* | Fermentation prioritaire (effet Crabtree) | Une pression évolutive plus faible sur la respiration → variations tolérées |
| *S. pombe*      | Respiration mitochondriale dominante      | ATP6 plus conservée → canal plus stable et performant                       |

* Chez *S. cerevisiae*, le recours à la fermentation en présence de glucose rend l’optimisation d’ATP6 moins critique.
* Chez *S. pombe*, qui dépend plus directement de la chaîne respiratoire, une **structure plus conservée d’ATP6** est cohérente avec une fonction essentielle maintenue.

**Conclusion** : malgré une identité < 50 %, ATP6 conserve sa structure et son rôle dans les deux espèces. La différence reflète davantage la stratégie métabolique que la perte de fonction.

## Protéine atp8

### 1. Alignement global

| **Critère**          | **Valeur**           | **Interprétation**                                                             |
| -------------------- | -------------------- | ------------------------------------------------------------------------------ |
| **Longueur alignée** | 48 aa                | Protéine courte, de même longueur chez les deux espèces                        |
| **Identité**         | 25 / 48 (**52.1 %**) | Plus de la moitié des acides aminés sont strictement identiques                |
| **Similarité**       | 33 / 48 (**68.8 %**) | Les deux tiers des acides aminés ont des propriétés chimiques similaires       |
| **Gaps (indels)**    | 0 / 48 (**0.0 %**)   | Aucun décalage → topologie parfaitement alignée                                |
| **Score**            | 126.0                | Score alignement significatif pour une petite protéine → conservation probable |

---

### 2. Comparaison de la fonction

**Fonction déclarée pour les deux espèces** (selon UniProt) :
ATP8 est une **sous-unité mineure** du domaine **F₀** de l’ATP synthase. Elle est située dans la membrane mitochondriale, proche de la sous-unité a, et participe au couplage entre le **flux de protons** et la **synthèse d’ATP**.

Les deux fiches UniProt donnent une **fonction strictement identique**.  
Elle joue un **rôle complémentaire** à d'autres sous-unités dans la structure du complexe.  

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| --------------- | ---------- |
| ![ATP8\_cerevisiae](./figures/apt8/cerevisiae.png) | ![ATP8\_pombe](./figures/apt8/pombe.png) |

Les deux structures AlphaFold montrent :

* Une **seule hélice transmembranaire**, droite ou légèrement courbée
* Quelques différences dans les extrémités, mais le cœur hélicoïdal est **strictement conservé**

Les modèles confirment que la **forme nécessaire à l’insertion dans la membrane et au contact avec la sous-unité a est maintenue**.

---

### 4. Impact fonctionnel

| Espèce          | Stratégie métabolique                  | Implication sur ATP8                                               |
| --------------- | -------------------------------------- | ------------------------------------------------------------------ |
| *S. cerevisiae* | Fermentation préférée (effet Crabtree) | Variations tolérées dans les acides aminés non essentiels          |
| *S. pombe*      | Respiration privilégiée                | Structure plus conservée pour soutenir une synthèse efficace d’ATP |

* Le fait qu’ATP8 soit **courte et bien conservée** indique une forte contrainte structurale : elle **ne peut pas beaucoup varier sans perdre sa fonction**.
* La présence d’une hélice transmembranaire identique valide son **rôle stabilisateur dans le complexe F₀**, malgré une identité de seulement 52 %.

**Conclusion** : ATP8 conserve sa forme et son rôle malgré une divergence modérée. Son importance dans l’ancrage de l’ATP synthase explique cette stabilité entre espèces aux stratégies métaboliques différentes.

## Protéine atp9

### 1. Alignement global

| **Critère**          | **Valeur**            | **Interprétation**                                                                  |
| -------------------- | --------------------- | ----------------------------------------------------------------------------------- |
| **Longueur alignée** | 76 acides aminés (aa) | Longueur totale de l’alignement                                                     |
| **Identité**         | 45 / 76 (**59.2 %**)  | Plus de la moitié des acides aminés sont strictement identiques                     |
| **Similarité**       | 64 / 76 (**84.2 %**)  | Forte similarité : mêmes propriétés physicochimiques dans la majorité des positions |
| **Gaps**             | 2 / 76 (2.6 %)        | Très peu d’indels → alignement fiable et structure comparable                       |
| **Score**            | 253.0                 | Très bon score → ressemblance fonctionnelle et structurale probable                 |

---

### 2. Comparaison de la fonction

**Fonction décrite pour les deux espèces (UniProt)** :
ATP9 correspond à la **sous-unité c** de l’ATP synthase mitochondriale (complexe V, domaine F₀).
Elle est fortement hydrophobe, et forme un **anneau homomérique (c-ring)** d’environ **10 sous-unités**. Ce c-ring joue un rôle crucial dans le **mécanisme rotatif** qui transforme le passage des protons (H⁺) en énergie mécanique pour la synthèse d’ATP.

Les deux descriptions sont **strictement identiques**, confirmant une **fonction critique et conservée**.

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| -------------- | ---------- |
| ![ATP9\_cerevisiae](./figures/atp9/cerevisiae.png) | ![ATP9\_pombe](./figures/atp9/pombe.png) |

Les modèles AlphaFold montrent pour les deux espèces :

* **Deux hélices transmembranaires** parallèles, typiques de la sous-unité c
* Une architecture très compacte, adaptée à la formation de l’anneau rotatif (c-ring)
* Les deux images sont **quasi superposables**, malgré quelques variations mineures en surface

La **forme canonique** de la sous-unité c est **clairement conservée**, expliquant la forte similarité observée.

---

### 4. Impact fonctionnel

| Espèce          | Stratégie énergétique principale        | Implication sur ATP9                                  |
| --------------- | --------------------------------------- | ----------------------------------------------------- |
| *S. cerevisiae* | Fermentation fréquente (effet Crabtree) | ATP9 est conservée, mais peut être **moins exprimée** |
| *S. pombe*      | Respiration prioritaire                 | Structure et séquence fortement conservées            |

* Malgré les différences de stratégie métabolique, **ATP9 reste indispensable dans les deux espèces**, car le complexe ATP synthase doit rester fonctionnel pour assurer la respiration mitochondriale.

* La **pression évolutive élevée** sur cette protéine explique la **forte conservation de sa structure et de sa séquence**, en particulier dans les segments transmembranaires qui s’insèrent dans le c-ring.

**Conclusion** : ATP9 montre une **conservation remarquable** (84,2 % de similarité), illustrant la nécessité de maintenir un moteur rotatif efficace pour la production d’ATP. Sa stabilité structurelle malgré les stratégies métaboliques divergentes renforce son rôle fondamental dans la chaîne respiratoire.

## Protéine cox1

### 1. Alignement global

| **Critère**          | **Valeur**             | **Interprétation**                                                        |
| -------------------- | ---------------------- | ------------------------------------------------------------------------- |
| **Longueur alignée** | 543 aa                 | Protéine de grande taille, parfaitement alignée entre les deux espèces    |
| **Identité**         | 326 / 543 (**60.0 %**) | 60 % des acides aminés sont strictement identiques                        |
| **Similarité**       | 415 / 543 (**76.4 %**) | 76 % ont des propriétés similaires → substitutions souvent conservatrices |
| **Gaps**             | 14 / 543 (**2.6 %**)   | Très peu de décalages → structure bien alignée                            |
| **Score**            | 1814.0                 | Très bon score, typique d’une forte conservation fonctionnelle            |

---

### 2. Comparaison de la fonction

**Fonction pour les deux espèces** (selon UniProt) :
COX1 est une **sous-unité catalytique** du complexe IV (cytochrome c oxydase), situé à l’extrémité de la chaîne respiratoire mitochondriale. Elle :

* **Transfère les électrons** depuis le cytochrome c vers l’oxygène moléculaire
* **Catalyse la réduction de O₂ en H₂O** via un centre binucléaire (héme A3 + cuivre B)
* Contribue à la **génération du gradient de protons** nécessaire à la synthèse d’ATP

Les fonctions décrites sont **strictement identiques** entre *S. pombe* et *S. cerevisiae*  
COX1 est une **protéine essentielle à la respiration aérobie**  

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| --------------- | ---------- |
| ![COX1\_cerevisiae](./figures/cox1/cerevisiae.png) | ![COX1\_pombe](./figures/cox1/pombe.png) |

Les modèles AlphaFold montrent :

* **Une structure dense et complexe** faite de nombreuses hélices transmembranaires
* Une forte **superposition des deux formes**, malgré quelques variations aux extrémités ou en surface
* Le **cœur catalytique** et le repliement global sont très proches

La forme globale est **hautement conservée**, garantissant le bon positionnement des groupes héminiques et des atomes de cuivre nécessaires à la catalyse

---

### 4. Impact fonctionnel

| Espèce          | Stratégie énergétique principale        | Implication sur COX1                                                 |
| --------------- | --------------------------------------- | -------------------------------------------------------------------- |
| *S. cerevisiae* | Fermentation fréquente (effet Crabtree) | COX1 conservée mais l’activité respiratoire peut être moins utilisée |
| *S. pombe*      | Respiration mitochondriale dominante    | Forte pression évolutive pour maintenir une COX1 efficace            |

* Malgré 40 % de non-identité, la conservation structurelle et fonctionnelle de COX1 est forte.
* Chez *S. cerevisiae*, les mutations peuvent refléter une **moindre dépendance** à la respiration.
* Chez *S. pombe*, la structure plus optimisée suggère une **utilisation intensive de la chaîne respiratoire**.

**Conclusion** : COX1 est une protéine clé de la respiration, conservée structurellement dans les deux levures. Les divergences de séquence semblent refléter non une perte de fonction, mais des **adaptations métaboliques** différentes à l’environnement riche en glucose.

## Protéine cox2

Voici la fiche structurée complète pour la **protéine COX2**, dans le même format que les précédentes :

---

## Protéine cox2

---

### 1. Alignement global

| **Critère**          | **Valeur**             | **Interprétation**                                                              |
| -------------------- | ---------------------- | ------------------------------------------------------------------------------- |
| **Longueur alignée** | 254 aa                 | Longueur totale des deux séquences après alignement                             |
| **Identité**         | 129 / 254 (**50.8 %**) | Un acide aminé sur deux est identique → conservation moyenne mais significative |
| **Similarité**       | 176 / 254 (**69.3 %**) | Deux tiers des acides aminés ont des propriétés similaires → fonction conservée |
| **Gaps**             | 9 / 254 (**3.5 %**)    | Faible nombre de décalages → structure comparable                               |
| **Score Needle**     | 713.0                  | Score élevé → alignement fiable et structurellement pertinent                   |

---

### 2. Comparaison de la fonction

**Fonction décrite pour les deux espèces (UniProt)** :
COX2 est une **sous-unité catalytique membranaire** du complexe IV (cytochrome c oxydase). Elle joue un rôle central dans la respiration mitochondriale :

* Elle **reçoit les électrons** du cytochrome c via son centre cuivre A (CU(A))
* Elle les transmet au site actif du COX1 (binuclear center : héme A3 + cuivre B)
* Elle participe ainsi à la **réduction de l’oxygène en eau**, dernière étape de la chaîne respiratoire

Les descriptions des deux espèces sont **quasiment identiques**, confirmant une **fonction catalytique critique et hautement conservée**

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| --------------- | ---------- |
| ![COX2\_cerevisiae](./figures/cox2/cerevisiae.png) | ![COX2\_pombe](./figures/cox2/pombe.png) |

Les modèles AlphaFold révèlent :

* **Une forme très similaire**, avec des hélices transmembranaires stables et un domaine extracellulaire en repliement complexe
* Quelques variations visibles sur les boucles exposées, mais la **position du centre cuivre A est vraisemblablement conservée**

La **structure générale et la topologie** sont compatibles avec une fonction catalytique équivalente dans les deux levures

---

### 4. Impact fonctionnel

| Espèce          | Stratégie énergétique                   | Implication sur COX2                                        |
| --------------- | --------------------------------------- | ----------------------------------------------------------- |
| *S. cerevisiae* | Fermentation fréquente (effet Crabtree) | COX2 reste fonctionnelle, mais son expression est modulable |
| *S. pombe*      | Respiration privilégiée                 | Forte pression de conservation → COX2 bien maintenue        |

*Même chez une levure capable de fermentation, COX2 est indispensable **dès que l’oxygène est présent**
* Le taux de similarité élevé (69,3 %) montre que la **fonction respiratoire est préservée** dans les deux espèces
* Les différences pourraient refléter une **optimisation respiratoire plus poussée chez *S. pombe***, espèce strictement aérobie

**Conclusion** : COX2 est une composante essentielle du complexe IV, et sa **structure et sa fonction sont conservées** entre *S. cerevisiae* et *S. pombe*. Son rôle dans la respiration mitochondriale rend sa séquence peu tolérante aux mutations, malgré des stratégies métaboliques divergentes.

## Protéine cox3

Voici la fiche structurée complète pour la **protéine COX3**, dans le même format que les précédentes :

---

## Protéine cox3

---

### 1. Alignement global

| **Critère**          | **Valeur**             | **Interprétation**                                                            |
| -------------------- | ---------------------- | ----------------------------------------------------------------------------- |
| **Longueur alignée** | 271 aa                 | Taille complète de l’alignement                                               |
| **Identité**         | 129 / 271 (**47.6 %**) | Moins de la moitié des acides aminés sont identiques → conservation partielle |
| **Similarité**       | 177 / 271 (**65.3 %**) | Forte similarité : acides aminés ayant des propriétés chimiques comparables   |
| **Gaps**             | 4 / 271 (**1.5 %**)    | Très peu d’indels → alignement propre                                         |
| **Score Needle**     | 678.5                  | Bon score → conservation structurale et fonctionnelle probable                |

---

### 2. Comparaison de la fonction

**Fonction déclarée (UniProt)** :
COX3 est une **sous-unité membranaire du complexe IV (cytochrome c oxydase)**. Elle joue un rôle essentiel dans la respiration mitochondriale :

* Elle **stabilise l’ensemble du complexe IV**
* Elle permet la **bonne interaction des sous-unités catalytiques COX1 et COX2**
* Elle contribue indirectement à la **réduction de l’oxygène en eau** et à la création du **gradient de protons**

La fonction de COX3 est **équivalente dans les deux espèces**, mais **moins directement catalytique** que COX1/2.

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| --------------- | ---------- |
| ![COX3\_cerevisiae](./figures/cox3/cerevisiae.png) | ![COX3\_pombe](./figures/cox3/pombe.png) |

Les modèles AlphaFold montrent :

* Deux structures **très similaires**, avec une **organisation en hélices transmembranaires parallèles**
* Des différences localisées surtout au niveau des **boucles périphériques ou des extrémités**
* Le cœur structural est **identique**, compatible avec une fonction stabilisatrice du complexe IV

La **topologie membranaire est conservée**, assurant une interaction correcte avec COX1 et COX2

---

### 4. Impact fonctionnel

| Espèce          | Stratégie énergétique                   | Implication sur COX3                            |
| --------------- | --------------------------------------- | ----------------------------------------------- |
| *S. cerevisiae* | Fermentation fréquente (effet Crabtree) | COX3 peut être moins exprimée ou optimisée      |
| *S. pombe*      | Respiration dominante                   | Forte nécessité de maintenir COX3 fonctionnelle |

*Une identité modérée (\~48 %) mais une forte similarité (\~65 %) indiquent que **la structure et la fonction sont globalement préservées**
* Cela permet à *S. pombe* de maintenir un **complexe IV stable**, crucial pour sa respiration active
* Les différences dans les boucles ou surfaces pourraient **moduler l'interaction entre sous-unités** ou la régulation locale

**Conclusion** : COX3 est modérément conservée entre les deux espèces, ce qui reflète sa fonction structurelle dans le complexe IV. Sa conservation assure la respiration mitochondriale, mais les variations pourraient expliquer des **différences d’efficacité respiratoire**, notamment entre *S. cerevisiae* (plus fermentaire) et *S. pombe* (plus respiratoire).

## Protéine rps3

### 1. Alignement global

| **Critère**          | **Valeur**             | **Interprétation**                                             |
| -------------------- | ---------------------- | -------------------------------------------------------------- |
| **Longueur alignée** | 406 aa                 | Taille totale de l’alignement                                  |
| **Identité**         | 71 / 406 (**17.5 %**)  | Très faible conservation → nombreuses substitutions            |
| **Similarité**       | 117 / 406 (**28.8 %**) | Un tiers seulement des résidus ont des propriétés similaires   |
| **Gaps**             | 198 / 406 (**48.8 %**) | Alignement très fragmenté → nombreuses insertions ou délétions |
| **Score Needle**     | 108.5                  | Score faible → séquences très divergentes                      |

---

### 2. Comparaison de la fonction

**Fonction principale dans les deux espèces (selon UniProt)** :
Rps3 est une **protéine ribosomique** faisant partie de la **petite sous-unité 40S** du ribosome. Elle participe à :

* L’**initiation de la traduction** (liaison aux ARNm et sélection des ARNt)
* Le **maintien de la fidélité de lecture**
* La **réparation de l’ADN** (activité endonucléase)
* Certaines fonctions **extraribosomiques** (apoptose, export ribosomique, stress cellulaire)

Les descriptions de fonction sont identiques, mais l’étendue fonctionnelle de Rps3 dépasse largement le simple rôle structural.

---

### 3. Comparaison de la structure 3D

| *S. cerevisiae* | *S. pombe* |
| --------------- | ---------- |
| ![RPS3\_cerevisiae](./figures/rps3/cerevisiae.png) | ![RPS3\_pombe](./figures/rps3/pombe.png) |

* Les deux structures présentent un **noyau commun (pli β-α-β)** typique des protéines ribosomiques
* La forme globale est **relativement conservée**, mais les **régions périphériques** (en jaune/orange) sont **très variables**
* Ces segments variables pourraient correspondre à des **extensions spécifiques à l’espèce**, impliquées dans des rôles extraribosomiques

La **structure centrale ribosomique est préservée**, mais les extrémités évoluent rapidement

---

### 4. Impact fonctionnel

| Espèce          | Fonctions attendues                         | Implication sur Rps3                                     |
| --------------- | ------------------------------------------- | -------------------------------------------------------- |
| *S. cerevisiae* | Traduction + réparation ADN + apoptose      | Rps3 est multifonctionnelle, avec des rôles bien établis |
| *S. pombe*      | Traduction + potentiel de fonctions annexes | Forte divergence → possible spécialisation ou adaptation |

* La **faible identité** (17.5 %) indique une **dérive évolutive marquée**, notamment dans les domaines non structuraux
* Pourtant, le **noyau fonctionnel (ribosomal)** reste visible dans la structure → **conservation des fonctions essentielles**
* Les différences pourraient refléter une **divergence dans les fonctions régulatrices ou adaptatives** (par exemple, réponse au stress, réparation)

**Conclusion** : Bien que la séquence de Rps3 soit très divergente entre *S. cerevisiae* et *S. pombe*, les fonctions ribosomiques de base sont probablement conservées. Les régions divergentes suggèrent des **adaptations spécifiques**, notamment pour les **fonctions extraribosomiques**, qui varient selon le contexte cellulaire de chaque espèce.


## Source, références, bibliographie
- Levures et fromage : https://www.actalia.eu/les-levures-dans-les-differents-types-de-fromage/
- Kimchi : https://fr.wikipedia.org/wiki/Kimchi
- Kombucha : https://fr.wikipedia.org/wiki/Kombucha
- aérobie et anaérobie des levures : https://www.svt-a-feuillade.fr/pages/doc_spe_Term/1485796993.
- Utilisation de levure pour synthétiser de la psylocybine : https://www.sciencedirect.com/science/article/pii/S109671761930401X?via%3Dihub
- Métabolisme des levures : https://chem.libretexts.org/Bookshelves/Biological_Chemistry/Fermentation_in_Food_Chemistry_(Graham)/01%3A_Modules/1.10%3A_Yeast_Metabolism#:~:text=The%20metabolic%20pathways%20utilized%20by,phosphate%20pathway%2C%20and%20oxidative%20phosphorylation.
- Glycolyse : https://www.kegg.jp/entry/sce00010
- Glycolyse : https://www.ncbi.nlm.nih.gov/books/NBK482303/
- Cycle de Krebs : https://www.genome.jp/dbget-bin/www_bget?pathway+hsa00020
- atp6, atp8, atp9 : https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0078105
- https://www.uniprot.org/uniprotkb/P05501/entry
- https://pubmed.ncbi.nlm.nih.gov/12187383/