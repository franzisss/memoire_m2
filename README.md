# memoire_m2

Ce dépôt contient les données, ainsi que les notebooks de code ayant servi à la chaîne de collecte et de traiteement des données, pour le mémoire de Master 2 Humanités Numériques de l'ENC, produit par Francesca Hemery. Le mémoire s'intitule "Expertise et émotion dans les discours de désinformation sur le climat en Français sur YouTube (2020-2025) : détection automatique et analyse linguistique". 

Ce dépôt Git contient : 

- un dossier données, dans lequel on trouve :
  
- tous les fichiers de données, segmentés et corrigés.
- un document csv comprenant toutes les indications nécessaires sur les vidéos du corpus : titre, date, auteur, lien.
  
- un dossier code, dans lequel on trouve :

- notebook_1_collecte_de_donnees.ipynb : contient le code utilisé pour scrapper les sous-titres des vidéos sélectionnées. 
- notebook_2_correction_et_ponctuation_du_texte.ipynb : contient le code pour effectuer la première étape de prétraitement : correction et ponctuation avec LLM fine-tuné.
- notebook_3_segmentation.ipynb : contient le code pour faire la seconde étape du prétraitement, avec la segmentation du corpus entre différentes unités de texte.
- notebook_4_annotation_emotion.ipynb : permet d'effectuer l'annotation de l'intensité émotionnelle sur les segments du corpus, avec une version de CamemBert spécialisé sur une tâche d'analyse de sentiment. 
- notebook_5_annotation_expertise.ipynb : permet d'effectuer l'annotation de l'expertise sur les segments du corpus, avec GPT-4. 
- notebook_6_analyse_du_corpus.ipynb : contient le code pour l'analyse des scores émotionnels et experts.

La grande majorité de ces notebooks ont été faits dans Google Colab.
