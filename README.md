# Marketing-Optimizer-Gaming-Industry-
Dieses Projekt analysiert Marketingdaten und baut ML-Modelle, um vorherzusagen:

Welche Marketing-Kanäle den größten Spieler-Zuwachs bringen.

Welche Budget-Strategien die beste Conversion Rate liefern.

**------Projektübersicht------**

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
Logistic Regression (balanced): Schwach, kaum besser als Zufall.
Random Forest: Liefert solide Ergebnisse (Accuracy ~0.70, F1 ~0.81).
XGBoost (balanced): Sehr stark bei F1-Score, berücksichtigt aber ohne Balancing nur Mehrheitsklasse.

Aktuell liefert Random Forest mit Balancing die besten Ergebnisse.



**Nächste Schritte**
Hyperparameter-Tuning (GridSearch / RandomizedSearch).
Feature Engineering (z. B. Saisonabhängigkeit aus Datum).
Mehr Visualisierung der Ergebnisse (ROC-Kurve, Feature Importance).
Optional: Web-App/Dashboard (Streamlit) zur interaktiven Nutzung.



**Autor**
Aaron Szypula – interessiert an Data Science, KI und Gaming-Industrie.
