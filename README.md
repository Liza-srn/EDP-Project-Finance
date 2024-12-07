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
