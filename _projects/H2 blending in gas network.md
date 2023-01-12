---
layout: page
title: H<sub>2</sub> Blending in Gas Network
description: 
img: assets/img/h2-bg-image.png
importance: 1
category: University
---
<p2> Abstract </p2>

<p>
In this project, the introduction of hydrogen in a local natural gas network has been studied. 
From regulatory and physical consideration a maximum molar percentage of blending have been identified. 
After have modeled a reference gas network, and have performed fluidodynamic simulations, increased pressure at the reduction point have been identified, in order to maintain the minimum pressure in every node.
The results have shown a possible emission reduction, however pressure losses have to be taken in account.

</p>


<p2 > Description </p2>
<p>
<p3> Objectives </p3>
<ul>
<li> Studying influence of H<sub>2</sub> blending in a gas connection </li> 
<li> Identifying maximum H<sub>2</sub> percentage in a local network </li>
<li> Identifying pressure setting variation to maintain the service </li>
<li> Calculate emission reduction </li>
</ul>
<p3> Results </p3>
<ul>
<li> H<sub>2</sub> introduction causes reduction in the Wobbe Index and increase in the pressure drop  </li> 
<li> For further increase in H<sub>2</sub> blending, new regulation on Wobbe Index limit is necessary </li>
<li> If produced through electrolysis from renewable energy, H<sub>2</sub> can reduce emissions from combustion. However, pressure losses have to be taken in account  </li>
</ul>


<p3> Development </p3>

<p> The project has been based on the <span class="strong2"> python </span> based solver developed by the University of Florence for the modelling and simulation of gas network, called NWGsolver (here reference), in collaboration with colleague Dr. Claudio Galli. </p>

<p> A preliminary analysis on a single pipeline has been carried to test the effect of the blending. 
The simple results showed how an introduction of hydrogen in the gas flux leads to an increase in both velocity and pressure losses. </p>

<div class="row justify-content-sm-center">

    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/simple-network.png" title="Elementary network" class="img-fluid rounded" %}
    </div>
    <div class="col-sm-9 mt-3 mt-md-0">
        {% include figure.html path="assets/img/v-h2.png" title="Velocity-H2" class="img-fluid rounded " %}
    </div>
</div>

<p> A gas network based on the country side town of Baccaiano (Florence, Italy) has been modeled, comprending domestic and industrial load estimations. 
These have been obtained from a combination of total consumption and load profile.</p>

<div class="row justify-content-sm-center">

    <div class="col-sm">
        {% include figure.html path="assets/img/network.png" title="Network" class="img-fluid rounded" %}
    </div>
</div>
<p> A tuning of the the pressure at the reduction point has been carried based, assuring that every point could have a pressure bigger than the legislation limitation (19mbar).</p>

<p> In gas network leglislation, a limit on the Wobbe Index (WI) parameter is set. 
The parameter combines the Higher Heating Value and Standard Gravity of a gas, and is a index of interchangability of fuels. 
The injection of H<sub>2</sub> has the effect of lowering this value, hence the maximum quantity of injectable hydrogen is limited. 
The limit has been calculated, from the physic characteristic of the selected natural gases and hydrogen, with a result of a maximum 22% belnding on molar basis.</p>

<p> Simulating the new pressure drops derived by the blending, some network nodes result in having a lower pressure than admited. 
For this reason, increased pressure at the reduction point has been detected in order to preserve the service. </p>

<p> Finally, a 22% molar H<sub>2</sub> blend could reduce the CO<sub>2</sub> emission of around 8%. In order to unlock further emission reduction, less stringent WI limit has to be set. 
    Furthermore, in this simulation the injection location was at the reduction point. 
    In the case of a hydrogen hub willing to transport hydrogen through gas pipeline on long distance, pressure drops can be relevant, poning questions on the requested power for compression.</p>

</p>