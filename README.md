# Sentiment-Analysis-IMDB-Review


Travail d'analyse de sentiment sur les commentaires IMDB provenant du site de kaggle https://www.kaggle.com/utathya/imdb-review-dataset. Le jeu de donnée comporte 100000 commentaires regroupés en 2 ensembles de train/test, labelisés en positif, en négatif et en unsup. Il y a 0 valeur manquante. 

On supprime le label unsup qui représente un sentiment indéfini, on se retrouve avec 50000 commentaires. On va chercher à prédire si le commentaire est négatif ou positif. On supprime les balises html, les mots avec peu de sens(stopword) et rassembler les mots qui ont des accords différents.

On utilise le Tf-Idf Vectorizer de scikit-learn, pour avoir une matrice document-terme. Puis, on compare divers modèles pour choisir le modèle adéquat pour la classification des commentaires.
