 MODELE DE PREDICTION D'APPROBATION DE PRET IMMOBILIER
=====================================================================
Objectif : predire si une demande de pret immobilier sera APPROUVEE
ou REFUSEE, a partir des caracteristiques du demandeur.

Ce script :
  1. Genere un jeu de donnees synthetique realiste
  2. Pretraite les donnees (encodage, mise a l'echelle)
  3. Entraine deux modeles (Regression Logistique + Random Forest)
  4. Evalue et compare les performances
  5. Sauvegarde le meilleur modele
  6. Fournit une fonction pour predire un nouveau dossier

Pour l'utiliser avec VOS propres donnees : remplacez la fonction
generate_synthetic_data() par un pd.read_csv("votre_fichier.csv")
en gardant les memes noms de colonnes (ou adaptez FEATURES ci-dessous).
