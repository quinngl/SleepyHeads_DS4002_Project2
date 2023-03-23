# SleepyHeads_DS4002_Project2
Victoria Feist (leader), Quinn Glovier, Adam Cook
## Contents of Repository 
This repository contains all the source code and data necessary to run a TensorFlow machine learning model to diagnose COVID-19 using chest x-rays.
- SRC Folder
  * Contains annotated R code file
- Data File Folder
  * Contains method of accessing orginal image files (Original Data) and cleaned/downloaded image data (Covid19-dataset).
- Figures Folder
  * Contains 3 figures
- LICENSE.md
  * Statement of MIT License
- README.md
  * Explains contents of repository and process of project execution

## SRC
#### Necessary Packages and Set Seed

```{r}
#Installing and loading necessary packages
#install.packages('tensorflow')
#install.packages('keras')
#install.packages('tfdatasets')
#install_tensorflow()
library(tensorflow)
library(keras)
set.seed(1234)
```


#### Usage of Code
- Download the image files and delete the "viral pneumonia" folder.
- Open the code file in R and ensure your working directory is the folder that contains the data
- Install necessary packages
- Run all the code in order to prepare the data, run the model, and evaluate the results


## DATA 
### Original Data
The original dataset before any cleaning: [Original Data](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset)
- The data is separated into three folders (COVID, normal, viral pneumonia), each composed of 70-110 images.

| Category       | Description                                                     |
| -------------  | -------------                                                   |
| COVID          | Chest x-rays of patients with COVID-19                          |
| Viral Pneumonia| Chest x-rays of healthy patients with no other lung infections  |
| Normal         | Chest x-rays of healthy patients with no other lung infections  |


### Final Data

The data after manipulation, ready to be used by the model: 

### Data Dictionary  
| Category      | Description                                                     |
| ------------- | -------------                                                   |
| COVID         | Chest x-rays of patients with COVID-19                          |
| Normal        | Chest x-rays of healthy patients with no other lung infections  |


## Figures
Bar graph showing the distrubution of images across 3 patient statuses: healthy, pneumonia, covid.


## References

[5]Cook, Adam, Feist, Victoria, Glovier, Quinn. “COVID-19 Diagnosis: Milestone 1,” 14-Mar-2023.Available: https://docs.google.com/document/d/1yZRRc8Uew2SW6e5kopsG7C5JLSKtqQjvSgnSoKYU3J8/edit

[8]Cook, Adam, Feist, Victoria, Glovier, Quinn. “COVID-19 Diagnosis: Milestone 2,” 16-Mar-2023. Available: https://docs.google.com/document/d/1u_pljSKlBErJu4n3dEF1ZCG7TjLRkuWQpu5EimiqvXA/edit
