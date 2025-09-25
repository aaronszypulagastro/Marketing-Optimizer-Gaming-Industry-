# Marketing-Optimizer-Gaming-Industry-
Dieses Projekt untersucht Marketingkampagnen in der Gaming-Industrie. Ziel ist es, vorherzusagen, welche Kampagnen erfolgreich sind und welche Marketing-Kanäle den größten Beitrag zur Spielerakquise leisten. Die Modelle unterstützen Unternehmen dabei, Budgets effizienter einzusetzen und Spielerwachstum gezielt zu fördern.

##  Business Relevance
Mit den entwickelten Modellen können Gaming-Unternehmen:
- Marketingbudgets effizienter einsetzen.
- Vorhersagen, welche Zielgruppen und Kanäle die besten Conversions bringen.
- Kampagnenplanung datengetrieben optimieren.

## Projektübersicht

**Daten:**
Social Media & Kampagnen-Daten (z. B. Audience, Channel, Duration, ROI, Engagement).



**Ziel:**
Vorhersage, ob eine Kampagne erfolgreich ist (Conversion Rate > Schwelle).



**Methodik:**
Train/Test-Split mit Stratifikation
Preprocessing-Pipeline (Imputation, Scaling, OneHot-Encoding)



**Modelle:** 
Logistic Regression, Random Forest, XGBoost
Vergleich anhand Accuracy, F1-Score, ROC-AUC



**Besonderheit:** 
Umgang mit Klassenungleichgewicht (75 % Erfolg vs. 25 % Nicht-Erfolg) durch
class_weight="balanced"
scale_pos_weight bei XGBoost



**Tech Stack**
Python 3.12
Pandas / Numpy (Datenaufbereitung)
Scikit-Learn (Preprocessing, Logistic Regression, Random Forest)
XGBoost (Gradient Boosting)
Matplotlib / Seaborn (Visualisierung)



**Ergebnisse**
| Modell              | Accuracy | F1-Score | ROC-AUC | Kommentar                         |
|---------------------|----------|----------|---------|-----------------------------------|
| Logistic Regression | 0.51     | 0.61     | 0.50    | schwach, kaum besser als Zufall   |
| Random Forest       | 0.70     | 0.81     | 0.59    | solide Ergebnisse                 |
| XGBoost (balanced)  | 0.75     | 0.86     | 0.50    | stark, aber Mehrheitsklasse-lastig |


Aktuell liefert Random Forest mit Balancing die besten Ergebnisse.



**Nächste Schritte**
- [ ] Hyperparameter-Tuning  
- [ ] Feature Engineering (Datum → Saison, Regionale Effekte)  
- [ ] Visualisierung (ROC-Kurven, Feature Importance)  
- [ ] Deployment als Streamlit-App  



**Autor**
Aaron Szypula – interessiert an Data Science, KI und Gaming-Industrie.
