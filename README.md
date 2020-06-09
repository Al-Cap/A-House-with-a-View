<p align="center">
   <img src=https://github.com/a-woodbury/Regression-King_County_House_Prices/blob/master/Resources/stlsplash2.jpg />
<div align="center">
   <figcaption></figcaption>
</div>
</p>


**Predicting House prices in King County, WA**

### Overview

The King County housing challenges data scientists to create a model for predicting home prices. We used the available features in addition to some engineered features in this pursuit, ultimately identifying location as the primary feature determing the price of a home. 
 

### Repository Navigation
<pre>
Technical Notebook : <a href=Link>Technical Notebook </a>
Other Notebooks    : <a href=Link>Modeling</a>, <a href=Link>Data Collection Notebook </a>
Dataset Links      : <a href=https://www.kaggle.com/harlfoxem/housesalesprediction>Kaggle: Houseing Prediction</a>
Presentation       : <a href=https://github.com/a-woodbury/A-House-with-a-View/blob/master/Presentation/kch_presentation.pdf>Slide Deck</a>
</pre>

### ReadME Navigation

[Data](https://github.com/a-woodbury/A-House-with-a-View#data) -
[Model](https://github.com/a-woodbury/A-House-with-a-View#model) -
[Results](https://github.com/a-woodbury/A-House-with-a-View#results) - 
[Recommendations](https://github.com/a-woodbury/A-House-with-a-View#recommendations) - 
[Future](https://github.com/a-woodbury/A-House-with-a-View#future) - 
[Project Info](https://github.com/a-woodbury/A-House-with-a-View#project-info) -


## Data
The dataset is obtained from [Kaggle Housing Prediction](https://www.kaggle.com/harlfoxem/housesalesprediction). It includes just over 21,000 observations, each representing a home sold in King County, Washington, between May 2014 and 2015. The median price of the homes are $450,000, and 99% of the homes sold for less than $2 million.

![price.png](https://github.com/a-woodbury/A-House-with-a-View/blob/master/Images/ppt_price99_hist.png)

## Modeling

### Features

**Continuous**

- Price (target)
- square feet of living space
- square feet of lot
- floors
- effective build: the number of years since the house was last renovated or built. Also, see [heat map of house ages across King County](https://github.com/a-woodbury/A-House-with-a-View/blob/master/Images/rm_age_heat.png); it is interesting to see the newer renovations/constructions closer to city center correlating with higher prices; gentrification?
![age.png](https://github.com/a-woodbury/A-House-with-a-View/blob/master/Images/ppt_age_bar.png)

**Categorical**

- Zipcode (one hot encoded; total of 70)
- Condition: 1 to 5 rating; an objective assessment of the cphysical condition of the home
- View: 0 to 4 rating; a subjective assessment of the view from the property
- Waterfront: boolean

![waterfront.png](https://github.com/a-woodbury/A-House-with-a-View/blob/master/Images/ppt_waterfront_bar.png)

- has basement: boolean

These features were fitted using statmodels OLS. 


## Results

Explained variance: 80%

We recognized early on that location has a prominent role in the selling price of a home. Our model clarified this hypothesis through zipcode feature weights:

Zipcode | Median Price | Premium
--- | --- | --- 
Base | $193,094.98 | 1.00x
98039 | $668,108.63 | 3.46x
98004 | $587,005.76 | 3.04x
98040 | $463,427.95| 2.40x
98033 | $409,361.36 | 2.12x

A major feature of location is the view from the property. We discovered homes with a higher view rating are typically located on a waterfront or proximal to Seattle's central business district; these houses may provide visibility to downtown Seattle or another scene with high appeal. Additionally, the homes sell for more. 

![view.png](https://github.com/a-woodbury/A-House-with-a-View/blob/master/Images/ppt_view_bar.png)


This scatter/heatmap displays the view-price relationship. The relative geography of King County can be inferred; large blue regions are bodies of water (Pugot sound), larger points are higher prices. Notice the higher view ratings along water and near city center.

![view.png](https://github.com/a-woodbury/A-House-with-a-View/blob/master/Images/ppt_view_map.png)

## Future

To derive even more accurate results, we'd like to expand the project with additional data, specifically housing prices over time, quality of schools, crime metrics. Additionally, we know the kitchen is often the selling point in a house, so kitchen features would provide even further insight on a home's sellability.


## Project Info
<pre>
Contributors : <a href=https://github.com/a-woodbury>Alphonso Woodbury</a>
               <a href=https://github.com/Joe-Bit-lab>Joseph McHugh</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Anaconda, Colab
Libraries    : pandas, matplotlib, statsmodels, sklearn
</pre>

<pre>
Duration     : March 2020
Last Update  : 06.08.2020
</pre>


