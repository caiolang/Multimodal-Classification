# Multimodal Classification
- Caio ELMOR LANG
- Amani MOKNI

Using multimodal (image+audio) data to classify an environment class. Project made for the MI203 - Machine Learning course at ENSTA Paris, 2021.

## Original Kaggle competition
The original data can be obtained in the following link:
> https://www.kaggle.com/birdy654/scene-classification-images-and-audio


## About the project
[EN]
The main objective of this project is to understand if the use of multimodal data can improve the classification power of a model.
It consists in an environment classification problem, where the environment must be chosen between 9 classes (Beach/City/Forrest/Classroom/Restaurant…) using images and ambient audio as inputs.

The goal is then to combine these two data sources to create a performing model.

In the beggining of the project, we have made a classifier using only the audio data, with a Support Vector Machine (SVM) with an RBF kernel.
The score obtained for this strategy was **94,028%** on Kaggle. The corresponding Notebook is in this repo as `audio_only.ipynb`.

Then, we've made a submission using only image data, which led to a score of **94,811%**.

Finally, we have used a network that has as input the image and audio data, and that resulted in a score of **99,65%**, using transfer learning.

The Notebook `multimodal_data.ipynb` shows the development of the models and their validation.

------------
[FR]
L'objectif fondamental de ce projet est de valider si l'utilisation de données multimodals apporte au pouvoir de classification d'un modèle.
En effet, il s'agit d'un problème de classification d’environnement entre 9 classes (Beach/City/Forrest/Classroom/Restaurant…) à partir des images et des audios qui sont entrés comme données.

Alors le but est de combiner les sources et trouver un modéle performant.

Au début du projet, on a fait une classification à partir des données audio seulment, avec une SVM de kernel RBF.
Le score obtenu pour cette stratégie était de **94,028%** sur Kaggle. Le Notebook utilisé est `audio_only.ipynb`.

Après, on a fait une submission en utilisant seulement des données d'image, ce qui nous a apporté un score de **94,811%**.

Finalement, on a fait une réseau qui admet comme entrée les données d'image et d'audio, et cela nous a donné comme résultat **99,65%** comme score.

Le Notebook `multimodal_data.ipynb` montre la démarche utilisé dans le développement des modèles et leurs validation.