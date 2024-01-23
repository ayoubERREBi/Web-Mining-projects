Sentiment Analysis on Moroccan Arabic Dialect
➢ Objectif
L'objectif de ce projet est de développer un système de classification de commentaires en arabe 
dialecte marocain. Ce système vise à catégoriser automatiquement les commentaires en fonction de 
leurs contenus.
➢ Description du projet et les étapes de mis en place
1. Prétraitement des Données
Le processus commence par un prétraitement détaillé des commentaires en arabe dialecte 
marocain. Les données textuelles subissent plusieurs étapes de nettoyage, notamment la 
 aucune ont’n qui') كل', 'ما', 'فينهو', 'الكل', 'لو', 'باش', 'بان', 'ودوك') comme stopwords des suppression
valeur significative, la gestion des séquences répétitives, et l'élimination des mots d'un seul 
caractère. Ces étapes visent à purifier les données et à préparer un corpus textuel cohérent.
2. Word2Vec pour la Représentation Sémantique :
Le modèle Word2Vec joue un rôle crucial dans la capture de la sémantique des mots. Nous avons 
effectué l’entraînement du modèle Word2Vec spécifiquement pour le dialecte marocain de l'arabe, 
avec une dimension de vecteur de 300. Cette dimensionnalité élevée permet une représentation plus 
complexe des relations sémantiques entre les mots.
3. Normalisation des Données Word2Vec :
Les embeddings Word2Vec obtenus sont normalisés à l'aide de StandardScaler. Cette normalisation 
garantit que les vecteurs de mots sont à une échelle comparable, ce qui facilite la convergence lors 
de l'entraînement du modèle de classification.
4. Modèle de Classification Neuronal :
Le modèle de classification est construit comme un réseau neuronal artificiel (ANN). Il est composé 
de 3 couches cachées, chacune avec une fonction d'activation ReLU pour introduire la non-linéarité. 
La couche de sortie utilise l'activation softmax.
5. Compilation et Entraînement :
Le modèle est compilé avec un optimiseur Adam personnalisé et une perte catégorielle croisée. Ces 
choix sont guidés par la nature de la tâche de classification multiclasse. L'ensemble de données 
d'entraînement est utilisé pour ajuster les poids du modèle au fil des époques. La validation sur 
l'ensemble de test permet de surveiller la généralisation du modèle.
6. Performance et Évaluation :
La performance du modèle est évaluée à l'aide de la précision (accuracy), qui mesure la proportion 
de classifications correctes. Atteignant une précision de 83.2%, le modèle démontre une capacité 
significative à catégoriser les commentaires dans le dialecte marocain.

Deux autres liens vers deux autres fichiers pour que le code fonctionne :
file 1 : https://drive.google.com/file/d/1givIgm-MGk5f4qyxn6cXbDrmbifo4ayu/view?usp=sharing
file 2 : https://drive.google.com/file/d/1dM5CHG9NcjMDMj6SwUbrzdB3SwcdTUyV/view?usp=sharing, https://drive.google.com/file/d/1givIgm-MGk5f4qyxn6cXbDrmbifo4ayu/view?usp=sharing
