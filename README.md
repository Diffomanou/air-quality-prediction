# Air Quality Prediction (AQI ML Project)

##  Description
Ce projet utilise des modèles de Machine Learning pour **prédire l'Indice de Qualité de l'Air (AQI)** à partir de données de pollution atmosphérique quotidiennes.  
Les polluants pris en compte incluent : **PM2.5, PM10, NO₂, SO₂, CO et Ozone**.  
Le projet permet également d’étudier l’impact des jours fériés et des variations journalières sur la qualité de l’air.

---

## 📊 Dataset
Le dataset contient :  
- `Date` : Jour, Mois, Année  
- `Holidays_Count` : 1 = jour férié, 0 = jour ouvré  
- `Days` : Nom du jour de la semaine  
- Paramètres de pollution : PM2.5, PM10, NO2, SO2, CO (mg/m³), Ozone  
- `AQI` : Indice de Qualité de l’Air  

Toutes les valeurs sont en **µg/m³** sauf CO (mg/m³).

---

##  Technologies et librairies
- Python 3  
- Pandas, NumPy  
- Scikit-learn (Random Forest, Gradient Boosting, XGBoost, Linear Regression)  
- Matplotlib, Seaborn pour les visualisations  

---

##  Méthodologie
1. Prétraitement des données (gestion des valeurs manquantes, encoding des jours fériés et jours de la semaine)  
2. Séparation des données en **features (`X`)** et **target (`y`) = AQI**  
3. Entraînement de plusieurs modèles ML :  
   - Régression Linéaire  
   - Random Forest  
   - Gradient Boosting (meilleur modèle)  
   - XGBoost  
4. Évaluation avec **RMSE** et **R² Score**  
5. Sauvegarde du modèle entraîné (`.pkl`) pour utilisation future  

---

## Comment utiliser
1. Cloner le repo :  
```bash
git clone https://github.com/Diffomanou/air-quality-prediction.git
