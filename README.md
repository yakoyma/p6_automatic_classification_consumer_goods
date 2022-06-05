# Projet 6 : Classifiez automatiquement des biens de consommation

Parcours Data Scientist d'OpenClassrooms en partenariat avec CentraleSupélec.

L'objectif du projet est d'effectuer une étude de faisabilité rapide d'un moteur de classification d'articles. Le notebook permet de traiter, d'extraire les features des données textuelles et visuelles, de les analyser et de les comparer par une approche de classification non supervisée. Une approche facultative rapide de classification supervisée est également implémentée en annexe.

La composition du jeu de données :
- Un fichier csv contenant les caractéristiques de 1050 articles ;
- Un dossier comportant 1050 images des produits.


## Les différentes méthodes d'extraction de features implémentées dans le notebook :
- Pour le traitement des données textuelles :
  - Le preprocessing (utilisation des packages NLTK, Wordcloud et Contractions) ;
  - Les approches de type "Bag-of-Words" : comptage simple de mots et TF-IDF (Term Frequency-Inverse Document Frequency) ;
  - L'approche de type "Word/Sentence embeddings" classique avec Word2Vec/Glove/FastText (utilisation de la librairie Gensim) ;
  - Les approches de type "Word/Sentence embeddings" avec BERT (Bidirectional Encoder Representations from Transformers) :
    - BERT HuggingFace ;
    - BERT TensorFlow Hub ;
    - SBERT (Sentence-BERT).
  - L'approche de type "Word/Sentence embeddings" avec USE (Universal Sentence Encoder).

- Pour le traitement des données visuelles :
  - Le preprocessing des images (utilisation de la librairie OpenCV) ;
  - Les algorithmes de type ORB/SIFT/SURF :
    - L'algorithme ORB ;
    - L'algorithme SIFT.
  - Les alogorithmes de type réseaux de neurones convolutifs (CNN) par le Transfer Learning (TensorFlow et la bibliothèque Keras) :
    - Le modèle ResNet50 ;
    - Le modèle ResNet101 ;
    - Le modèle EfficientNetB7.


## Implémentation de deux méthodes pour comparer les différents modèles d'extraction de caractéristiques :
- Les clusterings (classifications non supervisées) avec les features des données textuelles, visuelles et la combinaison des deux features (utilisation de la librairie Sklearn) ;
- Les classifications supervisées (facultatives) avec les features des données textuelles, visuelles et la combinaison des deux features (utilisation de la librairie PyCaret). 

