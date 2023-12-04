---
title: "Publications"
permalink: /publications/
author_profile: true
---

<html>
<style>
.filterDiv {
  float: left;
  display: block;
  width: 100%;
  margin: 2px;
  display: none;
}

.show {
  display: block;
}

.container {
  margin-top: 20px;
  overflow: hidden;
}

/* Style the buttons */
.btn {
  border: none;
  outline: none;
  padding: 12px 16px;
  background-color: #f1f1f1;
  cursor: pointer;
}

.btn:hover {
  background-color: #ddd;
}

.btn.active {
  background-color: #666;
  color: white;
}
</style>
<body>

<h2>All my publications</h2>

<div id="myBtnContainer">
  <button class="btn active" onclick="filterSelection('all')"> Show all</button>
  <button class="btn" onclick="filterSelection('resilience')"> Transportation and community resilience</button>
  <button class="btn" onclick="filterSelection('environment')"> Environment-friendly transportation system</button>
  <button class="btn" onclick="filterSelection('equity')"> Transportation equity</button>
  <button class="btn" onclick="filterSelection('travel-behavior')"> Land use and travel behavior</button>
  <button class="btn" onclick="filterSelection('transit')"> Transit planning</button>
</div>

<div class="container">
  <div class="filterDiv travel-behavior transit">Tao, T., & Cao, J. (2023). Exploring nonlinear and collective influences of regional and local built environment characteristics on travel distances by mode. Journal of Transport Geography, 109. https://doi.org/10.1016/j.jtrangeo.2023.103599 
  </div>
  <div class="filterDiv travel-behavior">Cao, J., & Tao, T. (2023). Using machine-learning models to understand nonlinear relationships between land use and travel. Transportation Research Part D: Transport and Environment, 123. https://doi.org/10.1016/j.trd.2023.103930 
  </div>
  <div class="filterDiv travel-behavior">Tao, T., & Næss, P. (2022). Exploring nonlinear built environment effects on driving with a mixed-methods approach. Transportation Research Part D: Transport and Environment, 111. https://doi.org/10.1016/j.trd.2022.103443 
  </div>
  <div class="filterDiv travel-behavior">Tao, T., & Cao, J. (2022). Examining motivations for owning autonomous vehicles: Implications for land use and transportation. Journal of Transport Geography, 102. https://doi.org/10.1016/j.jtrangeo.2022.103361 
  </div>
  <div class="filterDiv equity">Tao, T., Lindsey, G., Cao, J., & Wang, J. (2021). The effects of pedestrian and bicycle exposure on crash risk in Minneapolis. Journal of Transport and Land Use, 14(1), 1187–1208. https://doi.org/10.5198/jtlu.2021.1980 
  </div>
  <div class="filterDiv transit">Tao, T., Cao, J., & Wu, X. (2021). The Road Less Traveled: Does Rail Transit Matter? Journal of Planning Education and Research, 0739456X2110358. https://doi.org/10.1177/0739456x211035825 
  </div>
  <div class="filterDiv equity resilience">Tao, T., & Cao, J. (2021). Exploring the interaction effect of poverty concentration and transit service on highway traffic during the COVID-19 lockdown. Journal of Transport and Land Use, 14(1), 1149-1164. https://doi.org/10.5198/jtlu.2021.1978 
  </div>
  <div class="filterDiv travel-behavior transit">Tao, T., Wang, J., & Cao, X. (2020). Exploring the non-linear associations between spatial attributes and walking distance to transit. Journal of Transport Geography, 82, 102560. https://doi.org/10.1016/j.jtrangeo.2019.102560 
  </div>
  <div class="filterDiv environment">Wu, X., Tao, T., Cao, J., Fan, Y., & Ramaswami, A. (2019). Examining threshold effects of built environment elements on travel-related carbon-dioxide emissions. Transportation Research Part D: Transport and Environment, 75, 1-12. https://doi.org/10.1016/j.trd.2019.08.018 
  </div>
  <div class="filterDiv transit">Dou, X., Gong, X., Guo, X., & Tao, T. (2017). Coordination of Feeder Bus Schedule with Train Service at Integrated Transport Hubs. Transportation Research Record: Journal of the Transportation Research Board, 2648(1), 103-110. https://doi.org/10.3141/2648-12 
  </div>
</div>

<script>
filterSelection("all")
function filterSelection(c) {
  var x, i;
  x = document.getElementsByClassName("filterDiv");
  if (c == "all") c = "";
  for (i = 0; i < x.length; i++) {
    w3RemoveClass(x[i], "show");
    if (x[i].className.indexOf(c) > -1) w3AddClass(x[i], "show");
  }
}

function w3AddClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    if (arr1.indexOf(arr2[i]) == -1) {element.className += " " + arr2[i];}
  }
}

function w3RemoveClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    while (arr1.indexOf(arr2[i]) > -1) {
      arr1.splice(arr1.indexOf(arr2[i]), 1);     
    }
  }
  element.className = arr1.join(" ");
}

// Add active class to the current button (highlight it)
var btnContainer = document.getElementById("myBtnContainer");
var btns = btnContainer.getElementsByClassName("btn");
for (var i = 0; i < btns.length; i++) {
  btns[i].addEventListener("click", function(){
    var current = document.getElementsByClassName("active");
    current[0].className = current[0].className.replace(" active", "");
    this.className += " active";
  });
}
</script>

</body>
</html>


- [Transportation and community resilience](/publications/transportation-and-community-resilience)
- [Environment-friendly transportation system](/publications/environment-friendly-transportation-system)
- [Transportation equity](/publications/transportation-equity)
- [Land use and travel behavior](/publications/land-use-and-travel-behavior)
- [Transit planning](/publications/transit-planning)

See a complete list of my pulications from my [CV](/files/CV_Tao.pdf).
