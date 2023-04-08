# Projet 6 : Classifiez automatiquement des biens de consommation

Parcours Data Scientist d'OpenClassrooms en partenariat avec CentraleSupélec.

L'objectif du projet est d'effectuer une étude de faisabilité rapide d'un moteur de classification de biens de consommation. Le notebook réalisé permet de traiter, d'extraire les features des données textuelles et visuelles, de les analyser et de les comparer par une approche de classification non supervisée. Une approche facultative rapide de classification supervisée est également implémentée en annexe.

La composition du jeu de données :
- Un fichier csv contenant les caractéristiques de 1050 articles.
- Un dossier comportant 1050 images des produits.


## Les différentes méthodes d'extraction de features pour le traitement des données textuelles :
- L'import du jeu de données.
- Le preprocessing (utilisation des packages NLTK, Wordcloud et Contractions).
- Les approches de type "Bag-of-Words" avec le comptage simple de mots (CountVectorizer) et la vectorisation TF-IDF (Term Frequency-Inverse Document Frequency).
- L'approche de type "Word/Sentence embeddings" classique avec Word2Vec/Glove/FastText (utilisation de la librairie Gensim).
- Les approches de type "Word/Sentence embeddings" avec BERT (Bidirectional Encoder Representations from Transformers) :
  - BERT HuggingFace ;
  - BERT TensorFlow Hub ;
  - SBERT (Sentence-BERT).
- L'approche de type "Word/Sentence embeddings" avec USE (Universal Sentence Encoder).


## Les différentes méthodes d'extraction de features pour le traitement des données visuelles :
- L'import des images.
- Le preprocessing des images (utilisation de la librairie OpenCV).
- L'implémentation des algorithmes de type ORB/SIFT/SURF :
  - ORB (Oriented FAST and Rotated BRIEF) ;
  - SIFT (Scale-Invariant Feature Transform).
- L'implémentation des algorithmes de type réseaux de neurones convolutifs (CNN) par le Transfer Learning (TensorFlow et la bibliothèque Keras) :
  - Le modèle ResNet101 ;
  - Le modèle ResNet50 ;
  - Le modèle EfficientNetB7.


## La combinaison des features et la comparaison des classifications :
- Les clusterings (classifications non supervisées) avec les features des données textuelles, visuelles et la combinaison des deux features (utilisation de la librairie Sklearn).
- Les classifications supervisées rapides (facultatives) avec les features des données textuelles, visuelles et la combinaison des deux features (utilisation de la librairie PyCaret). 

