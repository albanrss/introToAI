# Introduction à l'Intelligence Artificielle

Cours pratique d'introduction au deep learning, en mode **learning by doing** (style Epitech).  
L'objectif : comprendre et construire des réseaux de neurones capables de reconnaître des chiffres manuscrits (MNIST), en partant de zéro.

> **Note :** Les notebooks de cours ont été générés avec l'aide d'une IA (Claude Opus 4.6).

## Contenu

### 1. Réseau de neurones from scratch — [`nn_from_scratch.ipynb`](nn_from_scratch.ipynb)

Construction d'un réseau de neurones **entièrement à la main avec NumPy**, sans aucun framework ML.  
Chaque multiplication matricielle, chaque dérivée, chaque mise à jour de poids est codée manuellement.

**Modules couverts :**
- Rappels mathématiques (produit matriciel, transposée, broadcasting)
- Le neurone : somme pondérée, biais, activation
- Fonctions d'activation : Sigmoid, ReLU, Softmax et leurs dérivées
- Forward propagation
- Loss functions : MSE, Cross-Entropy
- Backpropagation et chain rule
- Gradient descent, learning rate, mini-batch
- Assemblage dans une classe `NeuralNetwork`
- Entraînement et évaluation sur MNIST
- Améliorations : Momentum, He init, learning rate decay

**Stack :** Python, NumPy, Matplotlib

### 2. Classification MNIST avec Keras — [`mnist_cours.ipynb`](mnist_cours.ipynb)

Approche progressive de la classification d'images avec des frameworks ML, de la baseline classique jusqu'au CNN optimisé.

**Modules couverts :**
- Exploration et visualisation du dataset MNIST
- Preprocessing : normalisation, reshape, one-hot encoding
- Baseline avec régression logistique (scikit-learn)
- MLP (réseau dense) avec Keras
- CNN (réseau convolutif) : Conv2D, MaxPooling, feature maps
- Amélioration : Data augmentation, Dropout, EarlyStopping
- Pipeline complet d'inférence et analyse des erreurs

**Stack :** Python, NumPy, Matplotlib, Seaborn, scikit-learn, TensorFlow / Keras

**Résultats typiques :**

| Modèle | Accuracy (test) |
|--------|-----------------|
| Régression Logistique | ~92% |
| MLP (2 couches denses) | ~97-98% |
| CNN simple | ~99% |
| CNN + augmentation + dropout | ~99.2-99.4% |

## Prérequis

- Python 3.10+
- Les dépendances s'installent directement depuis les notebooks

## Utilisation

1. Cloner le dépôt
2. Ouvrir les notebooks dans Jupyter ou VS Code
3. Suivre les cellules dans l'ordre — les cellules marquées `# TODO` sont à compléter

