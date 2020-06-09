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
Other Notebooks    : <a href=https://github.com/a-woodbury/RxID/blob/master/RxID15_Modeling.ipynb>Modeling</a>, <a href=https://github.com/a-woodbury/RxID/blob/master/RxID15_Data_Collection.ipynb>Data Collection Notebook </a>
Dataset Links      : <a href=https://www.nlm.nih.gov/databases/download/pill_image.html>NIH RxImage Portal</a>, <a href=Link>GCP Bucket</a>
Presentation       : <a href=https://github.com/a-woodbury/RxID/blob/master/Presentation/RxID.pdf>Slide Deck</a>, <a href=https://docs.google.com/presentation/d/1f2bLza9GFhIXUAMudNsb00RTpHAwg5JegGIw2i2Jg8A/edit?usp=sharing>Google Slides</a>
Other              : <a href=Link>Recreating the Model Guide</a>, <a href=Link>Drug Classes</a>
</pre>

### ReadME Navigation

[Problem](https://github.com/a-woodbury/A-House-with-a-View/blob/master/README.md#problem) - 
[Data](https://github.com/a-woodbury/A-House-with-a-View#data) -
[Model](https://github.com/a-woodbury/A-House-with-a-View#model) -
[Results](https://github.com/a-woodbury/A-House-with-a-View#results) - 
[Recommendations](https://github.com/a-woodbury/A-House-with-a-View#recommendations) - 
[Future](https://github.com/a-woodbury/A-House-with-a-View#future) - 
[Project Info](https://github.com/a-woodbury/A-House-with-a-View#project-info) -



## Problem





## Data


## Model

## Results

We recognized early on that location has a prominent role in the selling price of a home. Our model clarified this hypothesis through zipcode feature weights:

Zipcode | Median Price | Premium
--- | --- | --- 
Base | $193,094.98 | 1.00x
98039 | $668,108.63 | 3.46x
98004 | $587,005.76 | 3.04x
98040 | $463,427.95| 2.40x
98033 | $409,361.36 | 2.12x

### Improving the current model


## Recommendations:

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


