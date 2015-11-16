---
id: 2869
title: Development Planning Toolkit Step 1
author: Candice Heberer
layout: page
guid: http://modi.mech.columbia.edu/?page_id=2869
---
 

## Development Planning Toolkit

<div class="row-fluid" style="padding-top: 20px;">
  <div class="span12 rpt-menu">
    <ul class="dptmenu">
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dpt/" class="dptmenu">Intro</a>
      </li>
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-overview" class="dptmenu">Overview</a>
      </li>
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-step-1" class="dptmenu" style="background-color:#2483b3 !important;">1. Households</a>
      </li>
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-step-2" class="dptmenu">2. Facilities</a>
      </li>
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-step-3" class="dptmenu">3. Demand</a>
      </li>
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-step-4" class="dptmenu">4. Technology</a>
      </li>
      <li class="dptmenu">
        <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-step-5" class="dptmenu">5. Plan</a>
      </li>
    </ul>
  </div>
</div>

<div class="row-fluid">
  <div class="span12">
    <h3>
      Step 1: Locate residential facilities
    </h3>
  </div>
</div><div class="row-fluid" style= background-color:#FFFFFF;"> 

<div class="span4 rpt-body" style="padding: 26px; 0px; 0px; 20px;">
  <p"><strong>ACTION STEPS:</strong></p> 
  
  <ul>
    <li>
      Geographically map the population
    </li>
  </ul>
  
  <p>
    <strong>IN RUHIIRA:</strong>
  </p>
  
  <p>
    Although households aren’t heavy electricity users, they are good indicators of energy requirements for an area. For instance, the denser the population, the more likely the need for other services like health facilities. Therefore, we started by mapping the population. Like all energy planning, we required a geographically located resolution of the population at 1 km<sup>2</sup> (ideally 500 m<sup>2</sup>) because 1 km is the maximum distance for reliable low voltage line operation.
  </p>
  
  <p>
    We had existing polygon<sup>1</sup> population data, but to achieve the desired 1 km<sup>2</sup> resolution, we needed household data. If this data doesn&#8217;t already exist from census or other government sources, we generally gather this data in one of two ways. We either use satellite imagery to locate households or collect population data by household enumeration with <a href="http://formhub.org" target="blank">Formhub</a>, a tool we developed to make mobile data collection fast, flexible and easy.
  </p>
  
  <p>
    In Ruhiira, because of the large area and poor roads, we decided against household enumeration. Instead, we created automated software (using image recognition in Python) for finding rooftops in high-resolution satellite imagery from QuickBird. Locating households using satellite imagery can also be done manually.
  </p>
  
  <p style="color:#589917">
    TIP: Household enumeration is a good option when existing site data is lacking and local governments are willing and able to use modernized data gathering tools. In these cases, focus on developing the capacity of local stakeholders for ongoing data acquisition and maintenance rather than collecting the data with your own team.
  </p>
  
  <p>
    Our software identified 13,366 households in Ruhiira, which we clustered at a resolution of 500 m<sup>2</sup>. In our model, we assumed the number of people in each household to be the same, which we found to be XX people per household.
  </p>
  
  <p>
    <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-overview">Prev</a> | <a href="http://modi.mech.columbia.edu/dev-planning-toolkit-step-2">Next: Step 2</a>
  </p>
</div>

<div class="span8">
  <div id="cf">
    <img class="bottom" src="http://modi.mech.columbia.edu/wp-content/uploads/2013/09/Map_Clusters.jpg" /> <img class="top" src="http://modi.mech.columbia.edu/wp-content/uploads/2013/09/Map_Rooftops.jpg" />
  </div>
  
  <p style="color:#589917; font-size:13px;">
    Mouseover the map to see clusters of households
  </p>
</div></div> 

<div class="row-fluid">
  <div class="span12 rpt-body" style="padding-top: 10px;> 
  
  <p style="color:#808080">
    <i><sup>1</sup>The main two ways countries represent their population data is with polygons or points. Polygons are bounded geographic areas containing a given population (usually around 5000 people). Point population data, on the other hand, involves individual households or clusters of households that are assigned geospatial locations. Polygons are often problematic to use for energy planning because areas can range up to as much as 100 km<sup>2</sup> depending on population density.</i>
  </p>
</div></div>