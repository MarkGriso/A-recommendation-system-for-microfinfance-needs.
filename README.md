# A recommendation system for microfinfance needs.


This project set out to develop a content-based recommendation system. 
The dataset used was that released by the Mircoredito Kiva platform, one of the largest microcredit platforms in the world. 

 HOW TO USE THE SYSTEM:
 
The system can be used by importing the two files 'Functions_for_recommendationSystem_Gui' and 'Gui_content_based_recommendationSystem'. 
The file with which to use the final system is the second one. The dataset to be imported is Kiva_loans_20k. The file has been reduced to twenty thousand observations for convenience. The files imported periodically by Kiva can exceed half a million observations.


RESULTS:

![image](https://user-images.githubusercontent.com/95644969/210348873-5315998e-0eb4-4b9d-a03b-562f094e061d.png)

By entering any word within the space provided, the system will bring up all words containing that particular word. The user can then decide which presitite he/she prefers depending on the additional features present. 
By selecting the ID and inserting it into the label provided, it will then be possible to receive the presites most similar to the one selected.

![image](https://user-images.githubusercontent.com/95644969/210350611-16a9bf38-7cce-4126-9caa-23e2ffa85be9.png)

It then becomes possible to display all loans that are most similar to the one selected, resulting in the cosine distance used for this purpose.

DIFFERENT APPROACHES:

![image](https://user-images.githubusercontent.com/95644969/210350694-ba6e7c0d-edcf-434c-9ff6-5b0ce3776474.png)

Within the code in the two selected files you will find sections where an approach was developed to convert the selected variables even with different distances including Euclidean and Levenshtein distances.
However, it was decided to retain the cosine distance as a more robust measure in relation to the different lengths of the verbal arrays created prior to the use of transformers (Tf-idf vectorizer) to produce the distances mentioned.
