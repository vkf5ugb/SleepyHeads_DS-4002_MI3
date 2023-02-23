# SleepyHeads_DS-4002_MI3
Adam Cook (leader), Quinn Glovier, Victoria Feist
## Contents
- SRC
  * Installing/Building Code
  * Usage of Code
- Data
  * Dataset
  * Data Dictionary
  * Notes
- Figures
  * Contents
- References


## SRC
#### Necessary Packages

library(dplyr)
library(tidyverse)
library(ggplot2)
library(dplyr)
library(tm)
library(SnowballC)
library(tidyverse)
library(randomForest)
library(rio)
library(plotly)
library(caret)
library(pROC)

#### Usage of Code
- Download the fake and true .csv's from the original data link and save them 
- Open the code file in RStudio and ensure your working directory is the folder that contains the data
- Install necessary packages
- Clear the variables by clicking the broom icon
- Run all the code in order to prepare the data, run the model, and evaluate the results


## DATA 
### Original Data
The original dataset before any cleaning: [Original Data](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset?select=True.csv)
- The data is separated into two csv's, fake and true, each of over 20,000 news articles.

### Final Data

The data after manipulation, ready to be used by the model: [Model_Data.csv](https://github.com/acook24/SleepyHeads_DS-4002_MI3/files/10794141/Model_Data.csv)

### Data Dictionary  
| Column        | Description                                                     |
| ------------- | -------------                                                   |
| Text          | Full article text with no punctuation and all lowercase letters |
| Type          | Classifies the article as true or fake (0 = true, 1 = fake)     |


## Figures
<img width="1200" alt="Frequency of Fake News in Data" src="https://user-images.githubusercontent.com/98351076/220919896-1c6ea529-3f33-420b-bbb3-1d18b811285f.png">

![Error Rate of Random Forest Model](https://user-images.githubusercontent.com/98351076/220920370-39c13c95-9823-4a70-92e9-b178fb8baa64.png)

<img width="1198" alt="Variable Importance Plot" src="https://user-images.githubusercontent.com/98351076/220920505-4c188984-c5c2-412d-b1d5-e8dee07073d2.png">

<img width="1040" alt="ROC Curve Plot" src="https://user-images.githubusercontent.com/98351076/220920559-1a639eb2-7a4a-4d62-9b0b-63e1e28ed0ca.png">


## References
[1]	ACC Library Services. (2023, Jan. 23). Fake News and Alternative Facts: Finding          Accurate News: Why is Fake News Harmful? [Online]. Available:-https://researchguides.austincc.edu/c.php?g=612891&p=4258046. [Accessed February 7, 2023].

[2]	Center for Information Technology and Society at UC Santa Barbara. (2018, Aug. 2). Why We Fall for Fake —----------News [Online]. Available:-https://www.cits.ucsb.edu/fake-news/why-we-fall. [Accessed February 7, 2023]

[3] D.M. West, “How to combat fake news and disinformation”, Brookings, December 18, 2017. [Online]. Available: —---------https://www.brookings.edu/research/how-to-combat-fake-news-and-disinformation/. [Accessed February 7, 2023].

[4] S. Desai and J.A. Oehrli, “‘Fake News,’ Lies and Propaganda: How to Sort Fact from Fiction”, University of Michigan Library: Research Guides, August 4, 2022. [Online]. Available: https://guides.lib.umich.edu/fakenews [Accessed February 7, 2023].

[5]Cook, Adam, Feist, Victoria, Glovier, Quinn. “Detecting Misinformation: Milestone 1,” 7-Feb-2023.Available:https://docs.google.com/document/d/1ieGReksXmIdDk5Jl153Wra9peDQyTA0KdFyvxSYZ0vk/edit

[6]C. Bisaillon, “Fake and real news dataset,” Kaggle, 26-Mar-2020. [Online]. Available: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset?select=True.csv. [Accessed: 14-Feb-2023]. 

[7]T. Yiu, “Understanding random forest,” Medium, 29-Sep-2021. [Online]. Available: https://towardsdatascience.com/understanding-random-forest-58381e0602d2#:~:text=The%20random%20forest%20is%20a,that%20of%20any%20individual%20tree. [Accessed: 14-Feb-2023]. 

[8]Cook, Adam, Feist, Victoria, Glovier, Quinn. “Detecting Misinformation: Milestone 2,” 7-Feb-2023. Available:https://docs.google.com/document/d/1vt-xL_zc_DKJPt1OahjVKtb6iz_EKf0JVSAVTI3pj9g/edit
