
### Fonctions de Mesure des Erreurs d'un Modèle

Lorsque vous entraînez un modèle susceptible de rencontrer des anomalies, il est crucial de mesurer les erreurs qu'il commet. Voici quelques fonctions couramment utilisées pour mesurer les erreurs d'un modèle :

#### Pour les valeurs continues
- Mean Square Error (Erreur quadratique moyenne)
$\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$
- Root Mean Square Error (Erreur quadratique moyenne)
$\text{RMSE} = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2}$
- Mean Absolute Error (Erreur absolue moyenne)
$\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} \left| y_i - \hat{y}_i \right|$
- R-squared (Coefficient de détermination)
$R^2 = 1 - \frac{\sum_{i=1}^{n} (y_i - \hat{y}_i)^2}{\sum_{i=1}^{n} (y_i - \bar{y}_i)^2}$

#### Pour les valeurs catégoriques
Dans le contexte des valeurs catégoriques, nous utilisons les notations suivantes :
- $TP$ (True Positive) : Les observations correctement identifiées comme positives.
- $FP$ (False Positive) : Les observations incorrectement identifiées comme positives.
- $FN$ (False Negative) : Les observations incorrectement identifiées comme négatives.
- $TN$ (True Negative) : Les observations correctement identifiées comme négatives.

$n$ représente le nombre total d'observations.

- Accuracy (Précision)
\[ \text{accuracy} = \frac{TP}{n} \]
- Precision (Précision)
\[ \text{precision} = \frac{TP}{TP + FP} \]

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
