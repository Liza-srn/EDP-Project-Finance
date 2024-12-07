# Gestion des Risques EDP

## Introduction
Ce projet explore l'application des équations aux dérivées partielles (EDP) dans le domaine de la finance. Il aborde des modèles mathématiques sophistiqués, tels que les modèles de **Black-Scholes**, **Cox-Ingersoll-Ross (CIR)** et **Vasicek**, pour résoudre des problèmes financiers comme la valorisation des options et des obligations.

L'objectif principal est de résoudre des EDP pour des variables financières dans les dimensions temporelles et spatiales en utilisant des approches numériques, notamment **la méthode des différences finies** et **le schéma de Crank-Nicholson**.

---

## Équations étudiées

### 1. Modèle de Black-Scholes
L'équation de Black-Scholes, utilisée pour la valorisation des options européennes, s'écrit :
\[
\frac{\partial V}{\partial t} + \frac{\sigma^2 S^2}{2} \frac{\partial^2 V}{\partial S^2} + r S \frac{\partial V}{\partial S} - rV = 0
\]

### 2. Modèle CIR
L'équation de Cox, Ingersoll et Ross décrit l'évolution des taux d'intérêt instantanés :
\[
dr_t = \kappa (\theta - r_t) dt + \sigma \sqrt{r_t} dW_t
\]

### 3. Modèle Vasicek
Le modèle de Vasicek utilise un processus d'Ornstein-Uhlenbeck pour modéliser les taux d'intérêt :
\[
dr_t = a (b - r_t) dt + \sigma dW_t
\]

---

## Méthodes numériques
Les modèles sont résolus numériquement en utilisant :
- **Schéma explicite**.
- **Schéma implicite**.
- **Schéma de Crank-Nicholson**.

Les différences finies centrées sont utilisées pour approximer les dérivées partielles, et des algorithmes comme **TDMA** (Tri-Diagonal Matrix Algorithm) sont implémentés pour résoudre les systèmes linéaires.

---

## Paramètres des modèles

### Black-Scholes :
| Paramètre | Valeur |
|-----------|--------|
| \( \theta \) | 0.5    |
| \( K \)     | 100    |
| \( \sigma \) | 0.20   |
| \( \tau \)  | 0.25   |
| \( r \)     | 0.08   |
| \( b \)     | -0.04  |

### CIR :
| Paramètre | Valeur |
|-----------|--------|
| \( \kappa \) | 0.8    |
| \( \theta \) | 0.10   |
| \( \sigma \) | 0.5    |
| \( \lambda \) | 0.05  |

### Vasicek :
| Paramètre | Valeur |
|-----------|--------|
| \( a \)     | 0.95   |
| \( b \)     | 0.10   |
| \( \sigma \) | 0.2    |
| \( \lambda \) | 0.05  |

---

## Organisation du projet
Le projet est structuré comme suit :
- **`notebook.ipynb`** : Contient les implémentations des modèles et les visualisations.
- **`README.md`** : Documentation du projet.
- **`requirements.txt`** : Liste des dépendances nécessaires.

---

## Prérequis
1. **Python 3.7+** doit être installé.
2. Installez les bibliothèques Python requises avec la commande suivante :
   ```bash
   pip install -r requirements.txt
