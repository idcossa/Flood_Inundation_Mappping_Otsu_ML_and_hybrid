
Exploring Landsat-8 imagery for flood inundation mapping using thresholding, machine learning and hybrid techniques: A case study of the April 2022 flood event in the East Coast of South Africa

This study attempts to answer questions such as (i) can the Otsu threshold be used to derive training data for ML applications? and (ii) how reliable is the Otsu threshold in detecting flooded areas in South African landscapes? To answer the aforementioned questions. 
This study set objectives to: 
  (i)	Map flood-inundated areas in eThekwini (ETH) Metropolitan Municipality and Ugu District Municipality (Ugu DM) using a gradient boosting machine (GBM), random forest (RF), the Otsu threshold, and a hybrid model combining Otsu with GBM and RF, all applied to Landsat-8 imagery. 
  (ii)	Assess the extent of the flood events that occurred from 10–12 April 2022 in both study areas, and 
  (iii)	Evaluate the empirical integration of threshold and supervised ML models to support labelled data derivation. 


1	Flood mapping scenario
The flood-mapping scenarios 1 and 2 in Fig. 1 were followed to define the study framework. This study classifies water using single models (RF, GB, and Otsu threshold). 
Explicitly, scenario 1 follows the traditional approach of flood mapping using ML and Otsu. In this scenario, RF and GBM were trained using defined labelled data. The Otsu threshold 
was calculated and adjusted based on overall accuracy. Change detection was applied to identify flooded areas using these three models. Because ML and threshold models are built on different principles, 
the aim was not to compare Otsu against RF and GBM. In scenario 1, Otsu was used to prepare for scenario 2.
Scenario 2 used the Otsu flood map from scenario 1 as a labelled dataset to train and validate new RF and GBM; we considered this approach a hybrid-ML model. The RF and GBM trained in scenario 2 were not 
inherently related to scenario 1. Additionally, in scenario 2, RF and GBM models were applied only on the post-image, without considering change detection. However, the pre-event classified image (GBM) from
scenario 1 was used to mask permanent or pre-event water bodies from the scenario 2 post-classified images. Following the conceptualisation of the scenarios, a framework is presented in Fig. 3. 


<img width="940" height="674" alt="image" src="https://github.com/user-attachments/assets/43a8be45-3a83-4150-8441-376d69a40b46" />
