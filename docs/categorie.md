#### Les diferents catégories d'apprentisage

Les catégories de modèle (algorithme) de machine learning se classe dans plusieurs catégorie dépendant tu problème qui est présenté. Mais avant que je te présente ces catégorie, je vais te parlez des phases á suivre jusqu'as l'utilisation du modèle. Ceci te faciliteras la compréhension.


***Les phases***

__Phase d'entrainement__

Suppossons que tu aies des données bien nétoyer avec des variables que tu penses seront utile pour le modèle. L'algorithme ne connait pas encore les règles qui lie ces différent données, la loie qu'elles suivent. Je prends toujours mon exemple de reconnaissance facial, tu as beaucoup d'image, mais qu'est ce qui rend ces images unique, qu'elle sont les règles qui vont te permettre de reconnaitre ces visage de ton ami parmis des milliers d'autre visage? Ces règle tu les as apprends durant le moment que tu as passé avec lui. 
Revenons á la machine learning, dans cette phase, tu vas entrainner le modèle á identifier la relations entre les données que tu dispose, une logique, **on dit dans le domaine que tu apprend á la machine á trouver les paramètres modèle **. Ces paramètre sont la loie, une fois tu les trouve avec certituide, tu peux les appliqués sur d'autre nouvelles données. 
Le modèle á bien apprend les paramètres du modèles, tu ne vas pas directement l'utiliser pour la production, il peux arrivé que ces paramètre sont appris parfaitement seulement sur ** l'échatillons de données** que tu as. Pour éviter cela, tu passe á une second phase la phase de test du modèles.

__Phase de test__

Dans cette phase, tu as le modèle entrainer c'est á dire avec les paramètre déterminer, tu vas l'appliquer sur d'autre échatillons pour voir s'il se comporte bien, vérifier s'il n'as pas de comportement anormal, ou s'il n'arrive pas á prédir parfaitement de nouvelle données. Sil arrive tu vas ajuster le modèle. Prenons toujours l'exemple de reconnaissance facial, tu crois pouvoir reconnaitre ton ami (c'est á dire connaitre les règle qui vont te permettre de l'identifier), on te présente une photo de lui et tu n'arrive pas á la déterminer, cela veux dire tes règle sont éronner, et n'ont pas pris en compte tous les aspects, tu vas faire quoi? Ajuster tes règles, vis á vis de cette nouvelle photo. C'est exactement ce que tu vas faire dans la phase de test.
Parfois il arrive qu'un modèle se comporte bien sur les données d'apprentissage mais il echoue á faire les prédictions, parfois aussi il arrive que le modèle á du mal á capturer la relation entre les données d'entrainement mais sur le test il fonctionnent bien. Ces modèle sont destiner á prendre des décisions á ta place, tu dois minimiser vois zero les erreurs si possible. Image tu crée un modèle qui va á partir d'une image produit par un scanner d'un patient prédire sa maladie. Si ton modèle commis des erreurs, ce sont des vie qui sont en jeux. Différent technique sont utilisés pour améliorer un modèle, je te les présente après.

__Évaluation__

Cette phase, tu vas donner une valeur á ton modèle, pour évaluer sa performance

##### Les types de données et les catégories d'apprentissage

Je te parles ici des différent stucture de données utilisés et la catégorie d'algorithme qui est utilisés.
***Apprentissage superviser***
Comme son nom l'indique, l'apprentissage dans ce cas est superviser, la machine est aider á connaitre les paramètre du modèle. Ces catégorie d'algorithme utilise un type de données qu'on appèl **les données labéliser (gardé bien ça)**. Une données labélisé est une données contient une partie de caractéristique et une partie cible, sur lesquelle la machine se base pour apprendre les règles.
Pour t'aider á t'imaginer ces données, je te donnes un exemple de reconnaissent de fruits. Tu dispose de plusieurs images de fruits , (manges, oranges, avocat, raisin) par exemple, on dit ils sont dans l'ensemble **A** lesquelle tu vas te basé pour prédire d'autre image de fruits qui ne sont pas dans ce ensemble **A**, ensemble **B** par exemple. Donc l'ensemble **A** est l'ensemble connue, tes données d'apprentissage, l'ensemble  **B** sont les données á prédire. Tu vas premierement apprendre les règle d'identifiaction de chaque fruit dans l'ensemble **A**.
Si tu n'avais pas le données de l'ensemble **A**, tu vas qu'as même les reconnaitres, pourquoi parceque tu as ces règle connue dans ta mémoire, tu les as appris dans ton enfance, ton ton cerveau n'as plus besoin de les apprendres. On va reprendre cette processus d'apprentissage en utilisant l'apprentissage superviser. 
Met toi à la place de la machine, images tu n'aies jamain vu ces fruit du catégorie **A**, quelqu'un oui il va te guider á les reconnaitre. Qu'est ce que tu faire, tu prendre un fruit tu notes ces caractéristique **la forme, la couleur, etc** toutes caractéristique des fruits, celui qui te guide te dit le nom et tu le notes (c'est la cible). Dans cette phase tu as annoté le fruit. Tu fais pareil pareil pour tous les fruits de l'ensemble **A**.  Tu viens d'annoté les fruits, **tu les as labéliser**. Maintenant tu apprend les règles. Par exemple, toutes les mangues ont cette couleurs, avec cette formes etc, c'est ce qui les differencie des autre fruits. Tu fais pareil pour les autres, tu apprends leur règles.
Viens maitenant la phase de prédiction, tu applique tes règles sur les fruits du catégorie *+B**. **tu viens de faire une apprentissage superviser**. Superviser parceque tu as le caractéristique et la cible á trouver.

Quand la cible est catégorique, appartient á une catégorie comme l'exemple que tu viens de voir on dit **Classification**. Parcontre quand la cible est continue, prédire par exemple la température de demain, cette valeur peux prendre n'importe quelle valeure, on dit la **regression**
**Apprentissage non superviser**

Contrairement á l'apprentissage qu'on vient de voir, ces algorithme ne sont pas aidés, ce qu'il dispose ce sont les caractéristiques, il n'ont pas la cible pour être superviser c'est á une même d'apprendre les règles.
Prénons l'exemple des fruits, du voie les caractéristique, tu n'as pas leur nom, a partir de ces caractéristique toi même tu apprends les règles. C'est l'apprentissage superviser.
***Apprentissage par renforcement***
Dans cet apprentissage tu apprend les règles en t'améliorant, lorsque tu commet une erreurs, tu tient compte de ce dernier et amélior tes règles (les paramètre du modèle).
**Il existe d'autre technique d'apprentissage mais c'est les plus utilisé**