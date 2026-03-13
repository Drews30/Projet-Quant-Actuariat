# Projet-Quant
Ce projet vise à modéliser l'impact des variations de taux d'intérêt sur la valeur d'un portefeuille obligataire. En utilisant les données historiques de la Banque du Canada, l'outil calcule la sensibilité du capital face à différents scénarios macroéconomiques.

Modélisation et prédiction de la vulnérabilité d'un portefeuille obligataire face aux chocs de taux d'intérêt.
Ce projet de bout en bout vise à analyser l'impact historique des fluctuations des taux de la Banque du Canada sur la valeur des obligations, et à utiliser le concept de ML pour prédire les rendements futurs et estimer le risque financier d'un portefeuille?

Vocabulaire :

  * Yield/Rendement : C'est le taux d'intérêt global exigé par le marché à un instant T (en %).
  * Prix de l'obligation : La valeur actuelle de ton obligation sur le marché (en $).

Fait : 

  * Importation et formatage des données brutes (gestion des dates et des valeurs manquantes).
    
  * Création d'une variable cible synthétique (Prix_Simule) à l'aide de formules mathématiques financières.
     $$PV = \sum_{t=1}^{n} \frac{C}{(1+i)^t} + \frac{F}{(1+i)^n}$$
    
  * Preuve visuelle de la relation inverse entre le Yield/Rendement et le Prix de l'obligation.
    
     -Conclusion : Lorsque le rendement (courbe bleue) monte, ils peuvent obtenir de meilleurs taux ailleurs. L'obligation                     à 3 % perd de son attrait, et son prix (courbe rouge) doit baisser (à l'escompte) pour se revendre. À                       l'inverse, si les taux du marché chutent, ton obligation devient très rentable et son prix grimpe (à                        prime).

A faire :

  * Remplacer la formule financiere déterministe, par un modele d'apprentissage automatique pour introduire l'aspect 'prédiction'.
    
  * Feature engineering avancé : Créer de nouvelles colonnes prédictives a partir de la df existante. Ajouter également des données macroéconomiques externes pour aider le modele a comprendre pourquoi les taux bougent.
    
  *  ML prep: Diviser la données en un ensemble Train et un Test pour éviter l'overfitting.
    
  *  Modelisation : Entrainer un algo (a determiner) pour prédire le Yield futur a partir des features selectionnées.
    
  *  Évaluation : Évaluer la précision de tes prédictions avec des métriques de Data Science (a determiner).
    
     -But : Traduire les erreurs en vrais dollars, injecter dans un portefeuille contenant plusieurs                                    obligations (différentes échéances, différents coupons) pour calculer l'impact total en                                     dollars.

