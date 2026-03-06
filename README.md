# Projet-Quant-Actuariat
Ce projet vise à modéliser l'impact des variations de taux d'intérêt sur la valeur d'un portefeuille obligataire. En utilisant les données historiques de la Banque du Canada, l'outil calcule la sensibilité du capital face à différents scénarios macroéconomiques.

🛠️ Méthodologie 

  (Pipeline Quant)Ingestion & Nettoyage : Extraction automatisée des rendements obligataires (10 ans) via l'API Valet de la BoC.
  
  Analyse de Tendance : Application d'une régression linéaire pour identifier la dérive (drift) historique des taux.
  
  Évaluation : Moteur de calcul de la Valeur Actuelle ($PV$) basé sur les principes de mathématiques financières.
  
  Stress Testing : Simulation de chocs de taux (ex: +200 bps) pour quantifier la perte de valeur maximale.
