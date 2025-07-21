---
layout: default
title:  "Green Skill Space"
description: "Interactive maps for the Green Skill Space."
permalink: /green-skill-project/green-skill-space/
---

# Green Skill Space

Select a view:

 

<select id="map-select"
        onchange="switchMap()"
        style="font-size: 1.5rem;
               padding: 0.5rem 0.75rem;
               width: 540px;">
 <option value="overview">Overall with 10 occupations highlighted</option>
  <option value="zone-1">JobZone 1 – Little or no preparation</option>
  <option value="zone-2">JobZone 2 – Some preparation</option>
  <option value="zone-3">JobZone 3 – Medium preparation</option>
  <option value="zone-4">JobZone 4 – Considerable preparation</option>
  <option value="zone-5">JobZone 5 – Extensive preparation</option>
</select>



<div id="overview" class="map-frame">
  <iframe
    src="../assets/skillspace/GreenSkillSpace_cluster_plot_highlight.html"
    width="1400" height="1100" frameborder="0">
  </iframe>
</div>

<div id="zone-1" class="map-frame" style="display:none;">
  <iframe
    src="../assets/skillspace/GreenSkillSpace_JobZone_1.html"
    width="1400" height="1100" frameborder="0">
  </iframe>
</div>

<div id="zone-2" class="map-frame" style="display:none;">
  <iframe
    src="../assets/skillspace/GreenSkillSpace_JobZone_2.html"
    width="1400" height="1100" frameborder="0">
  </iframe>
</div>

<div id="zone-3" class="map-frame" style="display:none;">
  <iframe
    src="../assets/skillspace/GreenSkillSpace_JobZone_3.html"
    width="1400" height="1100" frameborder="0">
  </iframe>
</div>

<div id="zone-4" class="map-frame" style="display:none;">
  <iframe
    src="../assets/skillspace/GreenSkillSpace_JobZone_4.html"
    width="1400" height="1100" frameborder="0">
  </iframe>
</div>

<div id="zone-5" class="map-frame" style="display:none;">
  <iframe
    src="../assets/skillspace/GreenSkillSpace_JobZone_5.html"
    width="1400" height="1100" frameborder="0">
  </iframe>
</div>

<script>
function switchMap() {
  var sel = document.getElementById('map-select').value;
  document.querySelectorAll('.map-frame').forEach(function(div){
    div.style.display = (div.id === sel) ? 'block' : 'none';
  });
}
// initialize on page load
switchMap();
</script>


 
 


[Back](../)