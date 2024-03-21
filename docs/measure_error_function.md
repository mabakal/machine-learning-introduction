
### Fonctions de Mesure des Erreurs d'un Modèle

Lorsque tu entraînez un modèle, tu peux rencontrer des anomalies, il est crucial de mesurer les erreurs qu'il commet. Voici quelques fonctions couramment utilisées pour mesurer les erreurs d'un modèle :

#### Pour les valeurs continues
- Mean Square Error (Erreur quadratique moyenne)
$\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$
- Root Mean Square Error (Erreur quadratique moyenne)
$\text{RMSE} = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2}$
- Mean Absolute Error (Erreur absolue moyenne)
$\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} \left| y_i - \hat{y}_i \right|$
- Rsquared (Coefficient de détermination)
$\text{R} = 1 - \frac{\sum_{i=1}^{n} (y_i - \hat{y}_i)^2}{\sum_{i=1}^{n} (y_i - \bar{y}_i)^2}$

#### Pour les valeurs catégoriques
Je te présente ces notion. Pour mieux les comprendre je te donne un exemple. Supposons que tu as construit un modèle dont le but est de reconnaitre chat sur plusieurs images qu'on fait passés. Voici les cas possible de classification
- $TP$ (True Positive) : le modèle á correctement classifier l'observation. L'observation dans notre cas c'est le chat, __le modèle á correctement identifier les chats__
- $FP$ (False Positive) : le modèle n'as pas pu identifier l'observation correct __il a classé une image non chat alors qu'en réalité c'est un chat__
- $FN$ (False Negative) : observations incorrect identifier incorrect. __il á classer correct  l'image qui n'est pas celui d'un chat__
- $TN$ (True Negative) : observation incorrect sont identifier correct. __c'est pas un chat mais il l'as classé chat__

$n$ représente le nombre total d'observations.

- Accuracy (Précision)
Le nombre des observations correctement classié sur le nombre total d'observation
$\text{accuracy} = \frac{TP}{n}$
- Precision (Précision)
Le nombre d'observation correctement classé sur le nombre total d'observation classé correct
$\text{precision} = \frac{TP}{TP + FP}$

### Matrice de Confusion
La matrice de confusion est un outil d'évaluation de la performance d'un modèle de classification. Elle est utilisée pour mesurer le nombre de prédictions correctes et incorrectes faites par le modèle par rapport aux classes réelles.

La matrice de confusion est organisée sous forme de tableau, où chaque ligne représente les instances dans une classe réelle, tandis que chaque colonne représente les instances dans une classe prédite par le modèle.

<table>
  <tr>
    <td></td>
    <td colspan="2"><strong>Classe Prédite</strong></td>
  </tr>
  <tr>
    <td rowspan="2"><strong>Classe Réelle (P)</strong></td>
    <td><strong>Positif</strong></td>
    <td><strong>Négatif</strong></td>
  </tr>
  <tr>
    <td>TP (Vrai Positif)</td>
    <td>FN (Faux Négatif)</td>
  </tr>
  <tr>
    <td>Classe Réelle (N)</td>
    <td>FP (Faux Positif)</td>
    <td>TN (Vrai Négatif)</td>
  </tr>
</table>
