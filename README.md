# Melbourne Airbnb Listings
This repo chronicles my cleaning and analysis of the Melbourne listings data collected by Inside Airbnb in order to better understand the impact of Airbnb listings on neighbourhoods and cities. The data contains "public" information posted on the Airbnb site, including, but not limited to, pricing information, neighbourhood reviews, listing specifications, and listing locations.

## The Data
The data used in thie project was acquired from [kaggle](https://www.kaggle.com/tylerx/melbourne-airbnb-open-data) and can also be downloaded from the source on [Inside Airbnb's website](http://insideairbnb.com/get-the-data.html).

## A General Overview
Using the data and working in Jupyter Notebook, I performed what cleaning was necessary for the data, and conducted/created exploratory analysis and visualizations. The initial data review/cleaning and general exploratory analysis can be found in `Melbourne_Airbnb-Exploratory_Analysis.ipynb`. Cleaned data was saved from this notebook into the `"Data_out"` folder.
Additional and more in-depth analysis and visualizations can be found in `Melbourne-A_Deeper_Look.ipynb`.

In conducting more expansive exploratory analysis, I created word clouds for the various "review" features, including the neighbourhood overview feature, such as:

![alt text](/Img_static/Neigh_Over/Round_2/SB_wordhouse.png "Second round South Bank word cloud")

The above word cloud was created for the South Bank neighbourhood which abuts the Yarra River and in which the Crown Casino, a popular tourist attraction, is located. One would assume from the cloud that South Bank is:
* Centrally located (given the high prevelance of words/phrases such as "minutes walk", "walking distance", and "short walk")
* Close to multiple other interesting attractions such as the:
  * Central Busniess District
  * Botanical Gardens
  * Exhibition Center
  * National Gallery
  * South Market
* A generally good district for tourists looking to stay in a walking friendly, central location full of local attractions

All of this can be quickly, and correctly, verrified by reviewing Melbourne using any map technology.

## Install Requirements
The majority of the requirements for this project can be installed, after cloning the repo to your computer, by using `pip install -r requirements.txt`.

The wordcloud package is not included in the `requirements.txt` file, as, in order to utilize image masking to specify different image shapes for the word clouds in the notebook, word cloud must be installed using the terminal, as below:

    git clone https://github.com/amueller/word_cloud.git
    cd word_cloud
    pip install .
