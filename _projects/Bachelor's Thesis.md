---
layout: page
title: Analysis of the Energy Price in the Italian Electricity Market
title2: Bachelor's Thesis
img: assets/img/bac-cover.png
importance: 2
category: Theses
---
<div class="row justify-content-sm-center">

    <div class="col-10">
        {% include figure.html path="assets/img/bac-cover.png" class="img-fluid rounded" %}
    </div>
</div>

<p2> Abstract </p2>

<p>
In the thesis work, the price of electricity in the Italian market has been examinated, firstly understanding which indipendent parameters influence more the price, and then modelling it, trying to minimize the R-square parameter.
Finally, a model with R-square=0.35 has been achieved. The values shows how the correlation is not sufficient for the model to be used, hence more parameters are necessary.
</p>


<p2 > Description </p2>
<p>
<p3> Objectives </p3>
<ul>
<li> Research of indipendent variables characterizing electricity price </li> 
<li> Development of a consistent model </li>
</ul>
<p3> Results </p3>
<ul>
<li> The main parameter influencing the electricity price in Italy is the natural gas price, with a R-square on daily basis of 0.67.  </li> 
<li> Further parameters added to better describe the price are the hour of the day and the day of the week </li>
<li> The model reach a moderated values of R-squared of around 0.35, showing how more indipendent parameters should be included  </li>
</ul>


<p3> Development </p3>

<p> In the Italian electricity market the price is estabilished in an auction made the day before the delivery. Sellers and buyers send their bids, and a equilibrium price is determined, called PUN (italian acronynum for Unique National Price).
Owning a efficient model, allows to already predict the balance price. </p>

The study has been based on the publicly available data about the electricity market, made available by the <a href="https://www.mercatoelettrico.org/it/" target="_blank">Gestore dei Mercati Energetici (GME)</a> , 
from which hourly data about the electricity price for the previous year have been collected. Data have been analyzed thorugh Excel. </p>

<p> The first parameter considered has been the natural gas price. Indeed, as known, Italy's electricity production is largely from thermoelectric plants, running mainly on natural gas. 
However, data available about natural gas price had only a daily resolution. Here is shown the correlation with a daily-averaged PUN, with a R-squared value of 0.67 .

<div class="row justify-content-sm-center">

    <div class="col-10">
        {% include figure.html path="assets/img/bac-el-ng.png" class="img-fluid rounded" %}
    </div>
</div>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/bac-el-ng-2.png" class="img-fluid rounded" %}
    </div>
</div>



<p> It has been noted how natural gas price is less sensitive at the day of the week respect to the PUN. 
Furthermore, the object model requires a hourly resolution. For this reason, in the model has been inserted two dedicated parameters.
These have been obtained dividing the average PUN for the day/hour with the total average PUN.
The final formula of the model has this form: </p>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/bac-formula.png" class="img-fluid rounded" %}
    </div>
</div>

<br>
<p> In the following pictures are shown the results for a single month sample. 
It is clear how the model is able to follow the general trend of the PUN, however is not able to follow the daily fluctuations, both in terms of peaks and lows. 
This poor rapresentation is confirmed by the R-square value of 0.35. 
<div class="row justify-content-sm-center">

    <div class="col-10">
        {% include figure.html path="assets/img/bac-el-mod.png" class="img-fluid rounded" %}
    </div>
</div>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/bac-el-mod-2.png" class="img-fluid rounded" %}
    </div>
</div>
