# Economic-Development
Based on open source remote sensing data and deep learning technology, we propose an unsupervised method for estimating China's grid scale development index. This method consists of four steps: feature extraction, feature clustering, model training based on ranking learning and index assignment. It has the characteristics of easy data acquisition and interpretability of the model, and provides a new idea for the research on China's fine-grained social development level. 
## Data Collection
The data we use for training includes daytime remote sensing image and nighttime light image. The collection method is shown in the ***/DataCollection/data_guide.ipynb***.

The daytime remote sensing images are crawled from the arcgis website. You can also download it directly from here https://www.kaggle.com/datasets/hhyyyyyy/daytime-image-zl12. And nighttime light image can be downloaded from https://eogdata.mines.edu/products/vnl/.

## Model Training
Train the model and extract the score. This method consists of four steps: feature extraction, feature clustering, model training based on ranking learning and index assignment. See ***/extract_score***. Through these steps, we can get the score for each image, that is, the grid scale score.

## Evaluation
The effect of model feature extraction is visualized by the Grad-CAM method. See ***/Grad-CAM/Grad-CAM.ipynb***.

We conducts research on the balance and agglomeration of  regional development in China. The Theil index is used to decompose the regional development differences, study the main sources of the differences.  See ***/theil&moran/cor&theil.ipynb***.
 
Then we use  spatial autocorrelation analysis to identify whether the unbalanced state is randomly distributed. See ***/theil&moran/Moran.ipynb***


