---
layout: page
title: Optimization of the Energy Scheduling in the Microgrid of Tilos Island
title2: Master's Thesis
description: June 2022
img: assets/img/t-tilos.jpeg
importance: 1
category: Theses
---
<div class="row justify-content-sm-center">

    <div class="col-10">
        {% include figure.html path="assets/img/t-tilos.jpeg" title="Tilos island" class="img-fluid rounded" %}
    </div>
</div>

<p2> Abstract </p2>

<p>
In the thesis work, the microgrid of the Greek island of Tilos was examined. 
The local solar-wind-battery hybrid generation system has been modeled, with the objective of optimizing the scheduling of storage activities while maximizing revenues from external electricity sales. 
A new simplified approach for evaluating battery wear within the optimization was developed, based on previous tuning through sensitivity analysis. 
Output load profiles, partly constrained by agreements with the grid operator, were reworked to demonstrate current underutilization of the microgrid's energy potential.
</p>


<p2 > Description </p2>
<p>
<p3> Objectives </p3>
<ul>
<li> Energy Modelling of the hybrid energy system whitin the microgrid </li> 
<li> Optimization of the energy output scheduling </li>
<li> Proposal of new output agreements with the grid operator </li>
</ul>
<p3> Results </p3>
<ul>
<li> A new python model of the system have been developed, with a novel approach for including battery wear management  </li> 
<li> The optimized scheduling output outperform the previous one by 87% on energy and 84% on earnings </li>
<li> New proposed agreement doubles energy export and increases earnings by 1.5 times (referring to optimized scheduling)  </li>
</ul>


<p3> Development </p3>

<p> Tilos is a little island located in the Greek Dodecanese with a population of 500 inhabitants that has been recognized as the first autonomous renewable green island in the Mediterranean, following a European Union-funded project of international collaboration. 
This has consisted in the realization of a hybrid generation system which powers the island microgrid, composed by an 800 kW wind turbine, a 160 kWp solar park, and a 2.88 GWh NaNiCl2 battery prototype.  </p>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/t-tilos-layout.png" class="img-fluid rounded" %}
    </div>
</div>

<p> The microgrid is connected to the energy system of the island of Kos, and it may function autonomously or interconnectedly. 
The latter is the method in which it is currently operating, under the management of the Greek company Eunice Energy Group (EEG). 
The existing agreement with the grid regulator involves a remuneration for the energy output in three power levels (0 kW, 200 kW, 400 kW), with hourly dispatch provided the day before. 
Economic penalties are applied for failure to respect power levels, whether in the form of excess or deficiency. </p>

<p> The necessity of a new scheduling technique emerges from the understanding that the current one is not efficient: 
it forces the microgrid to rely largely on renewable energy curtailment to avoid penalties and therefore significantly reduces the energy production.</p>

<p> The system has been modeled in a <span class="strong2"> python </span> environment, using <span class="strong2"> Mixed Integer Linear Programming </span>.

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/t-model.png" title="System model scheme" class="img-fluid rounded" %}
    </div>
</div>

<p> A new system optimization is proposed, based on the scenario of the current microgrid operation. 
Its purpose is to better exploit the potential energy, without excessively rely on energy curtailment, and thus increasing the revenues, featuring a novel strategy for managing battery wear in a lean approach. 
For the optimization, the commercial solver Gurobi has been used.</p>

<div class="row justify-content-sm-center">

    <div class="col-8">
        {% include figure.html path="assets/img/t-standard.png" class="img-fluid rounded" %}
    </div>
</div>

<div class="caption">
    Example of the optimized scheduling
</div>
 
<p> Furthermore, novel scenarios have been developed, following different criterias. The aim has been to explore solution to better exploit the renewable energy potential of the system. </p>

<p> The results show how effective the new schedules are in increasing the exported energy and the annual revenues. 
In particular, the different methods confirm their intent, whether it is to decrease the amount of overshooting energy or to increase the total amount of exported energy. 
Specifically, the new schedule would allow for an increase in exported energy by 86.9% and earnings by 84.2% over the current operations. 
Values that increase in the best exploration scenario brought forward: the method that involved the power level extension at 600 kW doubles the energy production and increases the earnings by 1.5 times. </p>


<div class="row justify-content-sm-center">

    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/t-results-1.png"  class="img-fluid rounded"   %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/t-results-2.png" class="img-fluid rounded"  %}
    </div>
</div>

