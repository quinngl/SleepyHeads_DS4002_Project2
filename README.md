# SleepyHeads_DS4002_Project2
Victoria Feist (leader), Quinn Glovier, Adam Cook
## Contents of Repository 
This repository contains all the source code and data necessary to run a TensorFlow machine learning model to diagnose COVID-19 using chest x-rays.
- SRC Folder
  * Contains annotated R code file
- Data File Folder
  * Contains method of accessing orginal image files (Original Dataset) and cleaned/downloaded image data (Cleaned Dataset).
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
- Download the image files and delete the "viral pneumonia" folder. Alternatively, download the cleaned dataset in the Data file.
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

The data after manipulation, ready to be used by the model: [Cleaned Data](https://drive.google.com/drive/folders/1M6D-41vEOOeMSL6QIo5UEMeCqJCpaDne?usp=sharing)

### Data Dictionary  
| Category      | Description                                                     |
| ------------- | -------------                                                   |
| COVID         | Chest x-rays of patients with COVID-19                          |
| Normal        | Chest x-rays of healthy patients with no other lung infections  |


## Figures
Bar graph showing the distrubution of images across 3 patient statuses: healthy, pneumonia, covid.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project2/blob/main/Figures/DataDist.jpeg" title= "Data Distribution">

Accuracy and loss fluctuate over the course of image testing.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project2/blob/main/Figures/Accuracy.jpeg" title= "Accuracy">

The model can easily classify normal, healthy lungs as such. However, it can only classify COVID-19 patient lungs correctly ~86% of the time.
<img src="https://github.com/vkf5ugb/SleepyHeads_DS4002_Project2/blob/main/Figures/CorrectClassifications.jpeg" title= "Correct Classifications">

## References
[1]M. R. Gordon and W. P. Strobel, “WSJ News Exclusive | Lab leak most likely origin of covid-19 pandemic, Energy Department now says,” The Wall Street Journal, 28-Feb-2023. [Online]. Available: https://www.wsj.com/articles/covid-origin-china-lab-leak-807b7b0a. [Accessed: 14-Mar-2023].

[2]  A. Abougazia et al., “Chest X-ray findings in COVID-19 patients presenting to primary care during the peak of the first wave of the pandemic in Qatar: Their association with clinical and laboratory findings,” Pulmonary medicine, 27-Oct-2021. [Online]. Available: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8553512/. [Accessed: 14-Mar-2023].

[3]A. Cook, V. Feist, Q. Glovier, “Covid-19 Diagnosis: Milestone 1”, The Sleepyheads, 14-Mar-2023, [Online]. Available: Project2_MI1 [Accessed 16-Mar-2023]

[4]ApokalypsePartyTeam, “How to build your own image recognition app with R! [part 1]: R-bloggers,” R-Bloggers, 16-Mar-2021. [Online]. Available: https://www.r-bloggers.com/2021/03/how-to-build-your-own-image-recognition-app-with-r-part-1/. [Accessed: 23-Mar-2023]. 

[5]A. Cook, V. Feist, Q. Glovier. “COVID-19 Diagnosis: Milestone 2,” 16-Mar-2023. Available: https://docs.google.com/document/d/1u_pljSKlBErJu4n3dEF1ZCG7TjLRkuWQpu5EimiqvXA/edit
