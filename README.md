## **Introduction**
Ce projet s'inscrit dans le domaine fascinant des équations aux dérivées partielles (EDP) appliquées à la finance. L'objectif principal est de résoudre des problèmes complexes liés à la valorisation des options et à la modélisation des taux d'intérêt en utilisant des méthodes numériques modernes.

Les modèles étudiés, notamment **Black-Scholes**, **Cox-Ingersoll-Ross (CIR)** et **Vasicek**, sont des piliers en finance quantitative, décrivant des phénomènes essentiels tels que l'évolution des prix des options ou des taux d'intérêt.

---

## **Points clés du projet**
- Application des **méthodes numériques** pour résoudre des EDP financières.
- Étude de **modèles financiers fondamentaux** : Black-Scholes, CIR, Vasicek.
- Mise en œuvre de **techniques de discrétisation** pour approcher des solutions numériques :
  - Schéma explicite
  - Schéma implicite
  - Schéma de Crank-Nicholson

---

## **Structure du projet**

### **1. Modèle de Black-Scholes**
Utilisé pour la valorisation des options européennes, ce modèle simule l'évolution du prix des options dans le temps en fonction du prix de l'actif sous-jacent, de la volatilité, et du taux sans risque.

### **2. Modèle CIR**
Ce modèle décrit l'évolution des taux d'intérêt en tenant compte des caractéristiques stochastiques, comme la volatilité et un retour à la moyenne.

### **3. Modèle Vasicek**
Un autre modèle pour les taux d'intérêt, basé sur un processus d'Ornstein-Uhlenbeck, qui permet une analyse plus simplifiée et symétrique des erreurs numériques.

---

## **Prérequis**
Pour exécuter ce projet, les outils suivants sont nécessaires :
- **Python 3.7+**
- Les bibliothèques suivantes :
  - `numpy`
  - `scipy`
  - `matplotlib`
  - `multiprocessing`
  - `jupyter`

Installez les dépendances avec la commande suivante :
```bash
pip install -r requirements.txt
