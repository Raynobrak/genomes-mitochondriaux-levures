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

## Conclusion générale

| **Protéine** | **Identité (%)** | **Similarité (%)** | **Gaps (%)** | **Score** |
| ------------ | ---------------- | ------------------ | ------------ | --------- |
| cox1         | 60.0             | 76.4               | 2.6          | 1814.0    |
| atp8         | 52.1             | 68.8               | 0.0          | 126.0     |
| atp6         | 43.9             | 63.1               | 9.6          | 571.5     |
| atp9         | 59.2             | 84.2               | 2.6          | 253.0     |
| cox2         | 50.8             | 69.3               | 3.5          | 713.0     |
| cox3         | 47.6             | 65.3               | 1.5          | 678.5     |
| rps3         | 17.5             | 28.8               | 48.8         | 108.5     |

---

### **Interprétation des résultats**

1. **Conservation des protéines respiratoires**
   Les protéines mitochondriales clés (*cox1*, *cox2*, *cox3*, *atp6*, *atp8*, *atp9*) présentent une **identité modérée à élevée** (44–60 %) et une **similarité substantielle** (63–84 %), avec très peu de gaps (1–10 %). Cela indique une **forte conservation structurale et fonctionnelle**, cohérente avec leur rôle crucial dans la chaîne respiratoire mitochondriale.

2. **RPS3 : une divergence remarquable**
   En revanche, *rps3* est **fortement divergente** (identité \~17 %, similarité \~29 %, gaps \~49 %), révélant une évolution significative de cette protéine ribosomique, probablement liée à des fonctions extraribosomiques et à des adaptations spécifiques.

---

### **Lien avec le métabolisme du glucose**

* *S. cerevisiae* est une levure **Crabtree-positive** : elle active préférentiellement la **fermentation** même en présence d’oxygène et de glucose (\[Crabtree effect description]\([frontiersin.org][1], [fr.wikipedia.org][2])). Cette préférence est régulée au niveau génomique, notamment par la répression de gènes respiratoires en conditions de glucose élevé (\[Crabtree repression]).

* *S. pombe* est **Crabtree-negative** à plusieurs égards : elle continue à **respirer même en présence de glucose**, et réduit la fermentation sous certaines conditions de stress ou carence (\[respiration constante]\([link.springer.com][3])).

Ce contraste métabolique se reflète dans la **divergence des protéines respiratoires** :

* Les protéines avec une **conservation élevée** (*cox1*, *atp9*) montrent que la **machinerie respiratoire est intacte** dans les deux espèces, mais peut être **régulée différemment**.
* Les protéines **modérément divergentes** (*atp6*, *cox3*) pourraient indiquer des ajustements structuraux liés à la **modulation respiratoire** en fonction de la stratégie énergétique de chaque espèce.

---

### **Synthèse**

La comparaison des protéines mitochondriales souligne une **conservation fonctionnelle générale**, essentielle pour la respiration, mais également des **variations significatives** corrélées à la divergence métabolique entre les levures :

* **S. cerevisiae** conserve sa machinerie respiratoire, mais la **repression transcriptionnelle** sous haute teneur en glucose favorise la fermentation (effet Crabtree).
* **S. pombe**, mieux adaptée à la respiration constante, affiche des protéines **plus conservées**, sans répression aussi prononcée.

**Conclusion** :
*Bien que les deux espèces partagent une base respiratoire commune, les différences observées dans des protéines clés reflètent leur adaptation métabolique divergente, avec une fermentation dominante chez S. cerevisiae et une respiration préservée chez S. pombe.*

[1]: https://www.frontiersin.org/journals/molecular-biosciences/articles/10.3389/fmolb.2014.00017/full?utm_source=chatgpt.com "An evolutionary perspective on the Crabtree effect - Frontiers"
[2]: https://fr.wikipedia.org/wiki/Culture_en_fed-batch?utm_source=chatgpt.com "Culture en fed-batch"
[3]: https://link.springer.com/article/10.1007/BF02907779?utm_source=chatgpt.com "Respiration and fermentation during growth and starvation in the ..."




