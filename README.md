
# Item Sales Prediction Analysis

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter%20Notebook-6.1.4-orange)

This repository contains an item sales prediction analysis conducted in July 2023. The analysis aims to predict item sales from stores using data science techniques and machine learning algorithms.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Notebook](#notebook)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In this analysis, we explore historical sales data and develop a predictive model to forecast future item sales. The goal is to provide insights for store owners or managers to optimize operations, inventory management, and decision-making processes.

## Installation

To run the notebook and replicate the analysis, please follow these steps:

1. Clone this repository: `git clone https://github.com/corycates8298/Prediction-Analyses.git`
   

## Usage

1. Launch Jupyter Notebook: `jupyter notebook`
2. Open the "Item Sales Prediction Analysis July 2023.ipynb" notebook.
3. Run each cell sequentially to reproduce the analysis and predictions.

## Dataset

The dataset used for this analysis is not included in this repository due to its size. However, you can find the dataset from https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view?usp=sharing and place it in the same directory as the notebook.

## Notebook

The notebook, "Item Sales Prediction Analysis July 2023.ipynb," contains the complete analysis pipeline, including data exploration, preprocessing, feature engineering, model training, evaluation, and prediction generation. It also includes detailed explanations and code comments to guide you through the process.

## Results

The results of this analysis include the predicted item sales, evaluation metrics, and insights derived from the trained model. The notebook provides visualizations and interpretations to facilitate a comprehensive understanding of the sales trends and patterns.  This is definitely better (Random Trees after tuning). The R values are closer to one another. Still underfitted, but better. The MAE and MSE values are also more closely related, which further solidifies that this is the better model.

The R values aren't horrible, but fairly low. What lead me to definitively determine underfitting was due to the fact that both the test and training values were fairly similar.
Based on regression testing, I have determined that this model (Featrues) is not equipped enough to accurately predict the Item Sales. I based this off of interpreting the the R, RMSE, and R values.

So an R^2 of .674 (Which is the training data after tuning) means that the model can explain 67% of the variation in the target. I did not select the MAE and MSE, because I am interested in the negative values and not just the magnitude (when interpreting Sales data). Also, I want a less complicated model to follow than MSE. The R values were much easier to interpret and to explain, but the MAE/MSE may be more suitable models.  

### Visualizations

![Alt Text](https://github.com/corycates8298/Prediction-Analyses/blob/main/Image1.png#:~:text=t-,Image1,-.png)

- Outlet Size by Outlet Sales Comparison.  As you can see, Store 3 is outranking the competitors.
  
![Alt Text[]([https://github.com/corycates8298/Prediction-Analyses/blob/main/Image1.png#:~:text=t-,Image2,-.png](https://github.com/corycates8298/Prediction-Analyses/edit/main/README.md#:~:text=README.md-,image2,-.png))](https://github.com/corycates8298/Prediction-Analyses/blob/main/image2.png?raw=true)

- Heatmap correlation  between item_mrp an item_outlet_sales, however not that strong. Looks to be at 0.57, with 1 being the strongest.


![Alt Text](https://github.com/corycates8298/Prediction-Analyses/blob/main/image5.png?raw=true)

- An example of the type of data that is excluded based on the current analysis.  Column Identifiers can be overlooked in this case.  

![Alt Text](https://github.com/corycates8298/Prediction-Analyses/blob/main/image6.png?raw=true)

![Alt Text](https://github.com/corycates8298/Prediction-Analyses/blob/main/image7.png?raw=true)

- Outlet Location type definitely plays a major factor in Sales.  The client demographic changes based on where the store is located.  

![Alt Text](https://github.com/corycates8298/Prediction-Analyses/blob/main/Image8.png?raw=true)

- This is a pretty positive correlation with r at 0.57. X increases and so does Y. Which makes sense, it's the actual list price. Actual price includes markup for profit.


## Recommendations 

My recommendation is to pay attention to some of the visualizations discribed above.  Most particularly, the Outlet Size, Location, and Item MRP.  They seem to play a pretty strong role in determining what the sales patterns are.

Although, this analysis wasn't 100% conclusive, the overall MAE and RMSE numbers that I have provided, may give you some insight into what the future wholes for your sales.  Please contact us if you need any further clarification.

## Contributing

Contributions to this project are welcome. If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.



Feel free to use the code and adapt it to your needs.

-------------------

By Cory N. Cates
