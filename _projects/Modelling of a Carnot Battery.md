---
layout: page
title: Modelling of a Carnot Battery
description: 
img: assets/img/carnot-cover.png
importance: 2
category: University
---
<div class="row justify-content-sm-center">

    <div class="col-10">
        {% include figure.html path="assets/img/carnot-cover.png" title="Example of a Carnot Battery cycle" class="img-fluid rounded" %}
    </div>
</div>

<p2> Abstract </p2>

<p>
In this project, a Carnot Battery featuring a reversible compressor expander is analyzed, with the possibility of integration of a wast heat stream. The working cycle has been modeled in MATLAB, thanks to the thermodynamic lybrary COOLPROP. 
The aim of the study has been to evaluate the main parameters influencing the performance of this device.
Results show the importance of the waste heat stream in the P2P ratio, and identify the expander efficiency as the main parameter to focus for improving the performance.
</p>


<p2 > Description </p2>
<p>
<p3> Objectives </p3>
<ul>
<li> Determining which are the most important design and performance parameters </li> 
</ul>
<p3> Results </p3>
<ul>
<li> Detected the efficiency of the expansor as a parameter that could improve performance up to 20% with a reasonable improvement  </li> 
<li> The possibility of heat integration, even with a stream under 100°C, would be heavly beneficial, with improvement up to 50% </li>
</ul>


<p3> Development </p3>

<p> A Carnot Battery is a innovative storage device for electric energy. Its principle is to store the energy in thermal form, to exploit its cost effectiveness and low losses. 
In order to do so, an energy cycle to transform the electricity to heat, and then back to electricity, is needed. 
For the charging cycle, a compressor is used to both increase the temperature  and pressure of the working fluid, in order to transfer the energy in the thermal storage while condensing.
For the discharging cycle, a possible solution is the utilization of a rankine cycle (i.e. a cyle where pressure is increased in the liquid state with a pump, with a evaporator and condenser linking the pump and the expander device).
The use of an organic fluid allows to work with more limited temperature than with other working fluids (in this case has been utilize the R1233Zd(E)), while as storage medium water has been chosen. 
In the particular design analyzed in the project, is explored the possibility to use a reversible compressor-expander, with the aim to reduce the system cost and complexity.
</p>

<p> The system has been modeled in <span class="strong2"> MATLAB </span> and solved due to the implementation of the thermodynamic library <a href="http://www.coolprop.org" target="_blank">COOLPROP</a> in the model. 

</p>

<div class="row justify-content-sm-center">

    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/car-cycle-1.png" title="Charging cycle" class="img-fluid rounded" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/car-cycle-2.png" title="Discharging cycle" class="img-fluid rounded " %}
    </div>
</div>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/car-cycle-3.jpg" class="img-fluid rounded" %}
    </div>
</div>



<p> To asses the performance of this Carnot Battery, a sensitivity analysis has been performed on some design and performance parameters:
<ul>
<li> T_waste<sub>waste</sub> : the temperature of the waste heat stream </li> 
<li> T<sub>lift</sub> : the increase in temperature due to the compression</li>
<li> &Delta;T<sub>pp</sub> : the pinch point temperature (design parameter of the heat exchangers)</li>
<li> &Delta;T<sub>storage</sub> : difference between hot and cold tank in the energy storage</li>
<li> T<sub>air</sub> : external temperature </li>
<li> &eta;<sub>exp</sub> : efficiency of the expansor </li>
</ul>
 </p>







<p> The performance has been evaluated on the Power to Power (P2P) parameter, i.e. the ratio between the power needed to charge the battery and the extractable power.
The most influential parameter among the ones evaluated is the T<sub>waste</sub>, with a variation of 50% on P2P between the maximum and standard value. This demonstrate the valorization that this device could give to a warm waste heat stream, but also his poor performance in the absence of it.
The second most influential parameter is the efficiency of the expander. Reversible compressor-expander are a relatively new technology, hence there is room for improvement. From the result is clear how further research and development on this machines could be beneficial for Carnot Battery performances.
Least influencial parameters from the ones examinated result the lift temperature and the storage delta temperature.
</p>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/car-results.jpg" class="img-fluid rounded" %}
    </div>
</div>


