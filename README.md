# RecomendationProj
<img src="./images/4_FilmWizard.png " width="700" height="600" />

## Overview

This project implements a Recommendation System for Movies.

## Business Problem

Interested in a targeted system in order to improve stickiness on the gaming site.  Researching a Collaborative Filtering System initially

## Data

MovieLens 100K -GroupLens research lab at the University of Minnesota
4 files
-100K user ratings of movies (.5 - 5)                                                            
-Tags for descriptions
-Movies
-Links to tmdb, imdb


Data containing 100K User ratings from 600 users 3000 descriptive tags

<img src="./images/gr4.png " width="200" height="350" /><img src="./images/download.png " width="200" height="350" />


## Methods

We performed KFold Cross Validation on the movie ratings with Matrix reduction algorithms and optimized with GridSearch.
We were looking for minimal errors choosing RMSE as our main metric and also time it takes to fit the moved as the matric will need to run to re fit after a user updates their ratings.

We used a Collaborative Filtering Model Based approach for this first implementation.


## Results

Best Predictive Results were found with the SVD algorithm
With a RMSE of .8696, Fit time of 4 seconds which was reduced to 2 sec with Hyperparameter tuning.

<table>
<thead>
  <tr>
    <th>Model</th>
    <th>RMSE</th>
    <th>MSE</th>
    <th>Fit Time(sec)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>SVD</td>
    <td>0.8696 </td>
    <td>0.6670 </td>
    <td>4.99   </td>
  </tr>
  <tr>
    <td>BaselineOnlyALS</td>
    <td>0.8725 </td>
    <td>0.6727 </td>
    <td>0.25</td>
  </tr>
  <tr>
    <td>KNNwMeans</td>
    <td>0.8924</td>
    <td>0.6815 </td>
    <td>0.24</td>
  </tr>
  <tr>
    <td>CoClustering</td>
    <td>0.9420</td>
    <td>0.7295</td>
    <td>2.89</td>
  </tr>
  <tr>
    <td>KNNBasic</td>
    <td>0.9458</td>
    <td>0.7254 </td>
    <td>0.18</td>
  </tr>
</tbody>
</table>

## Conclusions



Challenges<br>


## Next Steps
Finalize web app to be fully Operational<br>
Implement Hybrid Collaborative Model <br>
		Sentence of interest, mood, type NLP<br>
		Flexible between recommender models<br>


## For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/SunTzuLombardi/RecommendationProj/blob/main/code/RecSys_notebook.ipynb) or review this [presentation](https://github.com/SunTzuLombardi/RecommendationProj/blob/main/presentation.pdf)

For additional info, contact Daniel M. Smith at danielmsmith1@gmail.com

## Repository Structure

├── code<br>
│   ├── __init__.py<br>
│   ├── __.py<br>
├── data<br>
├── images<br>
├── __init__.py<br>
├── README.md<br>
├── presentation.pdf<br>
├── gitbhub.pdf<br>
├── notebook_RecSys.pdf<br>
├── RecSys_notebook.ipynb<br>





