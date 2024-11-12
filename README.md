<h2>Part one regression:</h2>
<h4>1. Apply the Exploratory data analysis technics to understand and visualize the given Dataset.</h4>
<h6>ptraitement des donnees</h6>
<p>
  conversion  du champ symbol en type numérique
  suppression du champ date 
  suppression des lignes en double et lignes vides
  Remplacer les valeures aberrantes par le moyen
</p>
<h6>visualisation des données</h6>
<P>matrice de la corrélation entre les donnees
un graphe pour la comparaison entre les différents prix (low ,high,open,close)
un graphe qui montre la distribution du volume de transaction
</P>

<h4>2.Establish a Deep Neural network Architecture by using PyTorch library to handle the
regression task. </h4>
<p>
  1. **Génération des données** : Création d'une matrice de caractéristiques 
2. **Organisation en DataFrame** : Les données sont organisées dans un DataFrame Pandas pour améliorer la lisibilité et la manipulation des colonnes.

3. **Division des données** : Séparation des données en ensembles d’entraînement et de test, avec une proportion de 80% pour l’entraînement et 20% pour le test.

4. **Normalisation des données** : Normalisation des caractéristiques avec `StandardScaler` afin d'assurer une convergence plus rapide et stable lors de l’entraînement du réseau de neurones.

5. **Conversion en tenseurs PyTorch** : Transformation des ensembles d’entraînement et de test en tenseurs PyTorch, prêts à être utilisés pour l’entraînement d’un réseau de neurones profond avec PyTorch.
</p>
<p>
  <h4>Part two multi class classification:</h4>
  <h6>
    
  </h6>
Initialisation des couches : Le modèle est constitué de trois couches linéaires :

Une première couche cachée (fc1) qui reçoit en entrée les données normalisées.
Une deuxième couche cachée (fc2).
Une couche de sortie (fc3) qui génère la prédiction.
Fonction d’activation : Utilisation de la fonction d'activation ReLU pour ajouter de la non-linéarité après chaque couche cachée, permettant ainsi au modèle de capturer des relations complexes.

Propagation avant (forward) : La méthode forward définit le flux de données à travers le réseau. Les données traversent les couches et les activations successives, produisant en sortie une prédiction pour une tâche de régression.
</p>
<p>
   configuration d'un modèle de régression basé sur un réseau de neurones, une fonction de coût pour évaluer les erreurs de prédiction, et un optimiseur pour ajuster les paramètres du modèle.
  entraînement  du modèle de régression en itérant sur les données d'entraînement et en optimisant les paramètres du modèle pour minimiser l'erreur de prédiction.


</p>
<h4>3. By using GridSearch tool from sklearn library chose the best hyper-parameters (learning rate ,
optimizers, epoch, model architecture, etc) that will give an efficient model.</h4>
<p>
   création  d'un réseau de neurones pour la régression en utilisant PyTorch, encapsulé dans une classe compatible avec scikit-learn pour permettre la recherche d'hyperparamètres. Il utilise GridSearchCV pour tester plusieurs combinaisons de paramètres et trouver la configuration optimale. Le meilleur modèle est ensuite évalué sur un ensemble de test en calculant l'erreur quadratique moyenne (MSE).
</p>
<h4>4. Visualize the two graph (Loss / Epochs) and (Accuracy / Epochs) for both training and test
data, give your interpretation.</h4>
<p>
   entraînement du modèle PyTorchRegressor sur les données d'entraînement pendant 50 époques, puis trace de deux graphes : la perte (Loss) et la précision (Accuracy) en fonction du nombre d'époques, pour les ensembles d'entraînement et de test. Ces visualisations permettent d'analyser la performance du modèle et de détecter un éventuel surapprentissage ou sous-apprentissage
</p>

<h4>
  5-Apply several regularization techniques on your architecture then compare the obtained result
with the first model.
</h4>
<p>    implémentation d'un modèle de régression PyTorch avec régularisation L2 (weight decay) et Dropout.  entraînement du modèle sur un ensemble de données et comparaison des performances (perte et précision) du modèle avec et sans régularisation, en affichant les courbes de perte et de précision pour les ensembles d'entraînement et de test à travers les époques. Les résultats sont visualisés à l'aide de graphiques montrant l'évolution de la perte et de la précision pour les deux versions du modèle.</p>
<P>interpretation:
  Lorsque les nouveaux hyperparamètres ont été utilisés, le modèle a montré une amélioration des résultats.
</P>
<h2>part two multi class classifocation</h2>
<h4>Apply the per-processing technics and the given dataset to clean,
standardization/normalization of the data.</h4>
<h6>ptraitement des donnees</h6>
<p>
  conversion  des champs de types categorique en type numérique
  suppression des ids
  suppression des lignes en double et lignes vides
  Remplacer les valeures aberrantes par le moyen
  standarisation des donnees
</p>

<h4>
  Apply the Exploratory data analysis technics to understand and visualize the given Dataset.
</h4>
<h6>visualisation</h6>
<p>
un graohe qui montre la distribution de   Tool wear [min]' selon 'Failure Type'
un graphe qui montre la distribution de 'Air temperature [K]' selon 'Failure Type
</p>
<h4>4. Establish a Deep Neural network Architecture by using PyTorch library to handle the multi
class classification task.</h4>
<p>
  Création d'un modèle de réseau de neurones profond avec deux couches cachées, utilisant l'activation ReLU pour une tâche de classification multiclasses.
Normalisation des données, les divise en ensembles d'entraînement et de test, et les convertit en tenseurs PyTorch.
Entraînement du  modèle sur 50 époques avec la fonction de perte CrossEntropyLoss et l'optimiseur Adam.
Évaluation de  la précision du modèle sur l'ensemble de test en comparant les prédictions avec les étiquettes réelles.


</p>
<h4>5. By using GridSearch tool from sklearn library chose the best hyper-parameters (learning rate ,
optimizers, epoch, model architecture, etc) that will give an efficient model.</h4>
<p>
 Le Charge du jeu de données Iris et le divise en ensembles d’entraînement et de test.
Standardisation des caractéristiques pour améliorer la performance du modèle.
Définition d'un perceptron multicouche (MLPClassifier) comme modèle de base pour la classification.
Utilisation de  RandomizedSearchCV pour effectuer une recherche aléatoire sur une grille de paramètres afin de trouver les meilleurs hyperparamètres pour le modèle.
Affichage des meilleurs paramètres trouvés, la précision obtenue en validation croisée et la précision finale sur les données de test.
</p>
<h4>6. Visualize the two graph (Loss / Epochs) and (Accuracy / Epochs) for both training and test
data, give your interpretation.</h4>
<p> Lorsqu'on a utilisé les nouveaux hyperparamètres, le modèle a donné des résultats plus précis.</p>
<h4>7. Calculate metrics like accuracy, sensitivity, f1 score, etc, on both training and test dataset.</h4>
