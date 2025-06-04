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

Le gène CYTB, spécifique à S. Pompe

todo continuer ici

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