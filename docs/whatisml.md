#### Qu'est-ce que le machine learning ?
Le machine learning, c'est toute technique utilisée dans le but de donner aux machines la capacité d'apprendre à partir de données pour résoudre un problème donné. Une question se pose : qu'apprend la machine ? Prenons l'exemple de la reconnaissance faciale. Parmi tous les visages que tu as mémorisés dans ta mémoire, il y a des caractéristiques propres à ces objets, des règles qui les lient. Ces règles permettent d'identifier ton ami d'une manière unique. C'est cette règle que la machine va chercher à apprendre, à établir pour ensuite les utiliser sur d'autres visages de ton ami. Ton rôle est d'apprendre à la machine à apprendre à partir de ces données.

##### C'est quoi l'intelligence artificielle et en quoi elle diffère de la ML?

L'intelligence artificielle est plus global, c'est l'ensemble des technique utilisé pour donner á la machine la capacité de prendre les décision sans l'intervention de l'homme. La machine learning y est inclus. Quand á ce dernier, les decisions sont prise aussi mais á partie des données. Parfois la machine learning fait appèle á des objects qu'on appèle les réseaux de neuronnes en imitant le fonctionnenement des réseauz humains, l'ensemble des techniques utilisé faisant intervenir les réseaux de neuronnes est le deep learning ou apprentissage profond. il se base aussi sur les données.

##### On parle de données, c'est quoi une donnée, et particulièrement avec le machine learning ?

Dans le processus de résolution de problème, tu utilises les données, parfois sans t'en rendre compte, car une fois que le cerveau est habitué à effectuer quelque chose, il ne cherche plus à comprendre comment ça fonctionne. __Une donnée, c'est toute information supplémentaire que tu as qui te facilite la résolution de ton problème.__ Je me rappelle au lycée quand je résolvais mes problèmes de physique (la mécanique), à la fin de l'énoncé on me fournissait une information supplémentaire : **g, la pesanteur terrestre est de 9,81 m/s carré.** Ces informations supplémentaires donnent des indications, facilitent la compréhension ou interviennent dans le raisonnement.
Quand je dis 17, ça n'a aucun sens et cela n'est pas utile pour résoudre un problème. Par contre, si je dis qu'il a 17 ans, cette information me sera très utile si je cherche à connaître une personne. Lorsque tu pars sur les sites internet, les informations qu'on demande sont tes données personnelles, tes préférences par exemple, à l'aide de ça, on peut t'identifier, te connaître et résoudre le problème de proposition de produit personnalisé.

**Les types de données:**

Les données sont de différents types, structurées ou non structurées. Voici quelques types de données : numériques (entier, décimal), texte, image, vidéo, audio, etc.<br>
**Où tu peux trouver les données :**

Les données sont partout autour de toi. Tu peux créer tes propres objets ou les collecter ailleurs. Certaines sont privées et l'accès n'est pas autorisé à tous (comme par exemple tes données personnelles, celles des entreprises), et d'autres sont publiques, certaines données qu'on laisse à la portée de tous.

##### À quoi les données sont-elles transmises ?

Une fois que tu disposez des données, comment apprend-tu à la machine à apprendre ? En fonction du type de problème auquel tu es confronté, tu utilises ce qu'on appelle un modèle. Il s'agit d'un algorithme, d'une logique pour résoudre un problème donné. Cet ensemble de logiques, d'algorithmes constitue l'apprentissage profond. Je vais donner un exemple d'algorithme très populaire appelé les "k plus proches voisins". Supposons que tu aies un objet, un fruit, disons une orange nommée _obj a_ par exemple, que la machine doit identifier. tu disposes de _données images_ sur plusieurs fruits. tu dit à la machine de comparer, ou encore de mesurer la similarité entre _obj a_ et tous les fruits de la base de données, puis de retourner les k fruits qui sont les plus proches de _obj a_ et d'attribuer à ce dernier les fruits dont l'occurrence est la plus nombreuse. tu as défini un algorithme qui permet d'identifier un fruit. Ces algorithmes, ces techniques sont appelés les modèles. Ce sont ces modèles que tu vas entraîner à partir des données. Il existe plusieurs modèles, mais tu peux aussi créer ta propre modèle. C'est la liberté que tu as.

##### Quand est la difference entre l'approche traditionnelle et celui de machine learning

Comment est ce qu'on ressoud les problèmes dans la programmation traditionnelle? Un ensemble de règle est prédéfinie, la logique pour faire simple. On passe des entrées qu'on appel **input** qui sont les données, et on obtient un **un output** qui est le resultat attendue. Dans le cas de la machine learning, la logique n'est pas connue d'avance, on passe en entré des **inputs** dans le modèle, en sortie on obtient un modèle qui est ensuite utilisé sur des nouvelle entré et produit un résultat attendus. La phase où tu apprend les règles liant ces objet est appellé la phase d'entrainement. La machine va apprendre les règles réliant ces objects. Après maintenant la phase de prédiction ou tu utilise ces règle sur des nouvelles entrées.

##### Comprendre comment l'humain apprend

Pour comprendre la manière dont la machine apprend, il faut d'abord comprendre comment l'humain apprend, puisque, comme  définit, c'est donner à la machine la capacité de prendre des décisions. C'est toi qui donnes cette capacité, il faut donc comprendre la manière dont tu prends les décisions sur la base du passé.
Voici le processus :

***Rappel-Formule-Décision***
1.__Rappel__
Dans cette première partie, nous consultons le passé pour voir les problèmes qui sont similaires au problème auquel nous faisons face. On les trouve dans notre mémoire, nos archives ou en demandant l'avis des autres qui ont déjà fait face à ce même problème.
2.__Formule__
Par la suite, en disposant de ces données et des résultats qu'elles ont produits, nous définissons une règle, nous formulons une formule qui s'appliquera à tout problème similaire.
3.__Décision__
Lorsque nous sommes confrontés à un nouveau problème, nous appliquons notre formule à ce problème. Nous prenons alors une décision en nous basant sur le résultat obtenu.
__Un exemple :__
Imaginons que tu doives te rendre à un endroit pour discuter d'un projet avec un collaborateur. Tu es quelqu'un de ponctuel, tu arrives toujours à l'heure et tu détestes attendre longtemps une personne. Le problème est : comment arriver sans prendre de retard par rapport à la personne et ne pas trop attendre la personne ? Tu as une décision à prendre.

En te basant sur le passé, tu examines les problèmes similaires rencontrés lors de tes rendez-vous avec cette personne : est-elle venue à l'heure ? Combien de retard a-t-elle pris ? Dans quelles circonstances, etc. A partir de ces informations, tu définis une règle,tu l'applique et tu prends une décision en te basant sur le résultat. Plus tu as d'informations sur le passé, plus ta règle sera fiable, car elle tiendra compte de tous les cas possibles. C'est pourquoi on dit que plus il y a de données, plus le modèle de machine learning sera fiable. Pour t'aider à mieux comprendre le machine learning, exerce-toi d'abord à résoudre des problèmes en suivant ces étapes.

##### Concrètement, qu'est-ce que la ML ?
La machine learning est un ensemble d'algorithmes (pour rappel, un algorithme est une succession d'instructions à exécuter pour résoudre un problème) qui prend en entrée des données et produit en sortie des règles générales sur ces données. Chaque algorithme est appelé un modèle. Un modèle est appliqué à un type de problème. La méthodologie ou technique que tu utilises pour prendre des décisions peut différer d'un problème à un autre. Il existe plusieurs modèles. Tu ne vas pas apprendre tous ces modèles d'un coup, mais au fur et à mesure que tu évolues, tu vas remarquer que certains modèles ont des limites et d'autres sont plus efficaces dans certains cas que d'autres. C'est pourquoi il faut toujours pratiquer.

##### Quelles bases théoriques as-tu besoin ?
En t'engageant en machine learning, tu auras besoin de quelques bases.
***Les Mathématiques***
Les mathématiques sont indispensables dans la plupart des domaines, car elles fournissent des outils pour des problèmes faisant appel à la logique. Quand je dis les mathématiques, c'est très vaste. Les outils que tu vas utiliser le plus souvent sont la logique, l'analyse et l'algèbre.
***Les Statistiques et la Probabilité***
Du moment où tu travailles avec des données, ces deux domaines sont indispensables. Ils te fournissent un langage pour comprendre et expliquer les données.
***La Programmation***
Tu seras amené à apprendre aux machines la capacité d'apprendre. Tu dois comprendre leur langage pour pouvoir communiquer avec elles. Les machines comprennent différents langages ; les langages les plus utilisés en IA sont le Python, Java, R et Julia. Tu auras besoin de quelques notions de base. J'ai une formation sur Python qui est disponible [ici](https://github.com/mabakal/begin-with-python)
##### Les outils dont tu auras besoin
Beaucoup d'outils sont disponibles, notamment les bibliothèques de modèles, etc. La plupart de ces outils sont utilisés en Python, qui est d'ailleurs le langage de l'IA. Il dispose d'une communauté qui développe ces outils de manière gratuite. [Clique ici pour les voir et les installer](/docs/outils.md). Note bien que tu auras beaucoup de difficulté à utiliser ces outils si tu ne connais pas leurs bases théoriques et celles du machine learning.
