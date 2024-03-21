### Les différentes catégories d'apprentissage

Les catégories de modèles (algorithmes) de machine learning se classent dans plusieurs catégories selon le problème présenté. Mais avant de présenter ces catégories, je vais vous parler des phases à suivre jusqu'à l'utilisation du modèle. Ceci facilitera votre compréhension.

**Les phases**

**Phase d'entraînement**

Supposons que vous disposiez de données bien nettoyées avec des variables que vous pensez utiles pour le modèle. L'algorithme ne connaît pas encore les règles qui relient ces différentes données, la loi qu'elles suivent. Prenons toujours l'exemple de la reconnaissance faciale : vous avez beaucoup d'images, mais qu'est-ce qui rend ces images uniques ? Quelles sont les règles qui vont vous permettre de reconnaître ces visages parmi des milliers d'autres ? Ces règles, vous les avez apprises durant le temps passé à les observer. 

Revenons à la machine learning, dans cette phase, vous allez entraîner le modèle à identifier la relation entre les données que vous disposez, une logique. On dit dans le domaine que vous apprenez à la machine à trouver les paramètres du modèle. Ces paramètres sont la loi ; une fois que vous les trouvez avec certitude, vous pouvez les appliquer sur d'autres nouvelles données. 

Le modèle a bien appris les paramètres du modèle, vous ne devez pas l'utiliser directement pour la production. Il peut arriver que ces paramètres soient appris parfaitement seulement sur l'échantillon de données que vous avez. Pour éviter cela, vous passez à une seconde phase, la phase de test du modèle.

**Phase de test**

Dans cette phase, vous avez le modèle entraîné, c'est-à-dire avec les paramètres déterminés, vous allez l'appliquer sur d'autres échantillons pour voir s'il se comporte bien, vérifier s'il n'a pas de comportement anormal, ou s'il n'arrive pas à prédire parfaitement de nouvelles données. S'il échoue, vous allez ajuster le modèle. 

Parfois, un modèle se comporte bien sur les données d'apprentissage mais échoue à faire les prédictions, parfois aussi il a du mal à capturer la relation entre les données d'entraînement mais sur le test il fonctionne bien. Ces modèles sont destinés à prendre des décisions à votre place ; vous devez minimiser au maximum les erreurs si possible. Imaginez que vous créez un modèle qui va, à partir d'une image produite par un scanner d'un patient, prédire sa maladie. Si votre modèle commet des erreurs, des vies sont en jeu. Différentes techniques sont utilisées pour améliorer un modèle, je vous les présenterai après.

**Évaluation**

Dans cette phase, vous allez donner une valeur à votre modèle pour évaluer sa performance.

**Les types de données et les catégories d'apprentissage**

Je vais vous parler ici des différentes structures de données utilisées et de la catégorie d'algorithme qui est utilisée.

**Apprentissage supervisé**

Comme son nom l'indique, l'apprentissage dans ce cas est supervisé, la machine est aidée à connaître les paramètres du modèle. Ces catégories d'algorithmes utilisent un type de données qu'on appelle **les données labélisées**. Une donnée labélisée est une donnée qui contient une partie de caractéristiques et une partie cible, sur laquelle la machine se base pour apprendre les règles.

Pour vous aider à vous imaginer ces données, je vous donne un exemple de reconnaissance de fruits. Vous disposez de plusieurs images de fruits (mangues, oranges, avocats, raisins), par exemple. On dit qu'ils sont dans l'ensemble **A**, sur lequel vous allez vous baser pour prédire d'autres images de fruits qui ne sont pas dans cet ensemble **A**, ensemble **B** par exemple. Donc, l'ensemble **A** est l'ensemble connu, vos données d'apprentissage, l'ensemble **B** sont les données à prédire. Vous allez premièrement apprendre les règles d'identification de chaque fruit dans l'ensemble **A**.

Si vous n'aviez pas les données de l'ensemble **A**, vous allez quand même les reconnaître. Pourquoi ? Parce que vous avez ces règles connues dans votre mémoire, vous les avez apprises dans votre enfance, votre cerveau n'a plus besoin de les apprendre. On va reprendre ce processus d'apprentissage en utilisant l'apprentissage supervisé.

Mettez-vous à la place de la machine. Imaginez que vous n'avez jamais vu ces fruits de la catégorie **A**, quelqu'un va vous guider à les reconnaître. Qu'est-ce que vous faites ? Vous prenez un fruit, vous notez ses caractéristiques (la forme, la couleur, etc.), toutes les caractéristiques des fruits. Celui qui vous guide vous dit le nom et vous le notez (c'est la cible). Dans cette phase, vous avez annoté le fruit. Vous faites de même pour tous les fruits de l'ensemble **A**. Vous venez d'annoter les fruits, **vous les avez labélisés**. Maintenant, vous apprenez les règles. Par exemple, toutes les mangues ont cette couleur, cette forme, etc., c'est ce qui les différencie des autres fruits. Vous faites de même pour les autres, vous apprenez leurs règles.

Vient maintenant la phase de prédiction, vous appliquez vos règles sur les fruits de la catégorie **B**. **Vous venez de faire un apprentissage supervisé**. Supervisé parce que vous avez les caractéristiques et la cible à trouver.

Quand la cible est catégorique, appartient à une catégorie comme l'exemple que vous venez de voir, on dit **Classification**. Par contre, quand la cible est continue, prédire par exemple la température de demain, cette valeur peut prendre n'importe quelle valeur, on dit la **régression**.

**Apprentissage non supervisé**

Contrairement à l'apprentissage que nous venons de voir, ces algorithmes ne sont pas aidés. Ce qu'ils possèdent ce sont les caractéristiques ; ils n'ont pas la cible pour être supervisés, c'est à eux-mêmes d'apprendre les règles.

Prenons l'exemple des fruits : vous avez les caractéristiques, mais pas leur nom. À partir de ces caractéristiques, vous-même vous apprenez les règles. C'est l'apprentissage non supervisé.

**Apprentissage par