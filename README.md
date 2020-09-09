# COVID

Objectif : Prédire si une personne est infectée en fonction des données cliniques disponibles

# 1/ Explotary Data Analysis:
    * Comprendre du mieux possible nos données :
    * Developper une premiere strategie de modelisation
   ## 1-1/ Analyse de la forme : 
      * Variable Target : SARS-Cov-2 exam result
      * lignes et colones : (5644,111)
      * Types de variables :   object     20
                               float64    14
                               int64       4
      * Analyses des variables manquantes : On remarque qu'on a beaucoup de Blanc , beaucoup de valeurs manquantes surtout à partir de la variable " Urine - Esterase " Du coup , ce qu on paut faire, c'est ragarder les probablitées des valeurs manquantes pour chaque variable.2 groupes de donnees (test viral 76% et test sanguin 89%)
   ## 1-1/ Analyse de fond :
      * Visualisation de la Target : negative    5086
                                     positive     558
          Nos 2 classes ne sont pas equilibrées , on a une majorite des personnes non infectées 90% .
      * Signification des variables : à propos de la variables "Patient age quantile" qui varie entre 0 et 19 ;Peut etre chaque nb est attribué a une tranche d'age.
                                     Variables continues standardisées 
                                     Variables qualitatives sont tous binaire ( detected , non detected ) à part la variable "Parainfluenza 2" qui possede q'une seule valeur not detected ; la variable "Rhinovirus/Enterovirus" est plus significative
                                     
      * Relation Variables / Target : Target/Blood ==> les taux de "Platlets" , " Monocytes " et " Lymphocytes " semblent different pour un porteur du Covid
                                      Target/Age ==> les individus de faible age sont tres peu contaminés mais on ne peut rien en deduire vu qu'on ne connait pas trop la signification de  la variable " Patient quantile age "
                                      Target/Age ==>  les doubles maladies sont tres raraes . 
      

