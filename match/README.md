## required data
* satellite daytime images
* nightlight data
* Administrative division data

## Code
The task can be divided into the following parts：
### Feature extraction
The night light data is used as a proxy variable to train the CNN model, and extract the features of satellite daytime images. See ***feature_extract.ipynb***.
### Image clustering
The images are clustered into several categories according to the extracted image features in the previous step. See ***sicluster&extract_cluster.ipynb***.
### Directed graph Construction
Constructing a directed graph of clusters under the guidance of nightlight and training CNN model based on the gragh and ranking learning. See ***siscore.ipynb***.
### Images scoring
Scoring images as well as the corresponding areas covered by them via CNNs. See ***extract_score.ipynb***.

The file ***match_center2PAC.ipynb*** is used to match the picture with the administrative division data.

