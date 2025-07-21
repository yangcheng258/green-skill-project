---
layout: default
title: Green Skill Dissimilarity
description: "Interactive green skill dissimilarity heatmaps by job zone."
permalink: /green-skill-based-recommendation-system/green-skill-dissimilarity/
---


## Interactive Green Skill Dissimilarity

This interactive heatmap shows the green skill dissimilarity between any two occupations, with detailed comparisons of individual green skill differences. Please choose the [Job Zone](https://www.onetonline.org/help/online/zones) and skill group you’re interested in:

<!-- <select id="zone-select"
        onchange="switchZone()"
        style="font-size: 1.5rem;
               padding: 0.5rem 0.75rem;
               width: 540px;">
  <option value="1">Job Zone 1 – Little or no preparation</option>
  <option value="2">Job Zone 2 – Some preparation</option>
  <option value="3">Job one 3 – Medium preparation</option>
  <option value="4">Job Zone 4 – Considerable preparation</option>
  <option value="5">Job Zone 5 – Extensive preparation</option>
</select>


 
{% raw %}
<div id="zone-1" class="heatmap-frame">
  <iframe src="../assets/heatmaps/heatmap_jobzone_1.html"
          width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-2" class="heatmap-frame" style="display:none;">
  <iframe src="../assets/heatmaps/heatmap_jobzone_2.html"
          width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-3" class="heatmap-frame" style="display:none;">
  <iframe src="../assets/heatmaps/heatmap_jobzone_3.html"
          width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-4" class="heatmap-frame" style="display:none;">
  <iframe src="../assets/heatmaps/heatmap_jobzone_4.html"
          width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-5" class="heatmap-frame" style="display:none;">
  <iframe src="../assets/heatmaps/heatmap_jobzone_5.html"
          width="1200" height="900" frameborder="0"></iframe>
</div>

<script>
function switchZone() {
  var sel = document.getElementById('zone-select').value;
  document.querySelectorAll('.heatmap-frame').forEach(function(div){
    div.style.display = (div.id === 'zone-' + sel) ? 'block' : 'none';
  });
}
// initialize on page load
switchZone();
</script>
{% endraw %}

[Back to home](../)
Add more content here if needed -->
 
Select a **Job Zone** and a **Feature Group** to view the corresponding heatmap:

<div style="margin-bottom:1rem;">
  <select
    id="zone-select"
    onchange="updateHeatmap()"
    style="font-size: 1.25rem; padding: 0.5rem; width: 260px; margin-right: 1rem;"
  >
    <option value="1">Job Zone 1 – Little or no preparation</option>
    <option value="2">Job Zone 2 – Some preparation</option>
    <option value="3">Job Zone 3 – Medium preparation</option>
    <option value="4">Job Zone 4 – Considerable preparation</option>
    <option value="5">Job Zone 5 – Extensive preparation</option>
  </select>

  <select
    id="group-select"
    onchange="updateHeatmap()"
    style="font-size: 1.25rem; padding: 0.5rem; width: 260px;"
  >
    <option value="skills">Skills</option>
    <option value="knowledge">Knowledge</option>
    <option value="workactivities">Work Activities</option>
  </select>
</div>

{% raw %}
<!-- Skills -->
<div id="zone-1-skills" class="heatmap-frame">
  <iframe src="./assets/heatmaps/heatmap_skills_jobzone_1.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-2-skills" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_skills_jobzone_2.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-3-skills" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_skills_jobzone_3.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-4-skills" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_skills_jobzone_4.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-5-skills" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_skills_jobzone_5.html" width="1200" height="900" frameborder="0"></iframe>
</div>

<!-- Knowledge -->
<div id="zone-1-knowledge" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_knowledge_jobzone_1.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-2-knowledge" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_knowledge_jobzone_2.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-3-knowledge" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_knowledge_jobzone_3.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-4-knowledge" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_knowledge_jobzone_4.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-5-knowledge" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_knowledge_jobzone_5.html" width="1200" height="900" frameborder="0"></iframe>
</div>

<!-- Work Activities -->
<div id="zone-1-workactivities" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_workactivities_jobzone_1.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-2-workactivities" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_workactivities_jobzone_2.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-3-workactivities" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_workactivities_jobzone_3.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-4-workactivities" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_workactivities_jobzone_4.html" width="1200" height="900" frameborder="0"></iframe>
</div>
<div id="zone-5-workactivities" class="heatmap-frame" style="display:none;">
  <iframe src="./assets/heatmaps/heatmap_workactivities_jobzone_5.html" width="1200" height="900" frameborder="0"></iframe>
</div>
{% endraw %}

<script>
function updateHeatmap() {
  const zone = document.getElementById('zone-select').value;
  const group = document.getElementById('group-select').value;
  document.querySelectorAll('.heatmap-frame').forEach(div => {
    div.style.display = (div.id === `zone-${zone}-${group}`) ? 'block' : 'none';
  });
}
// initialize on load
document.addEventListener('DOMContentLoaded', updateHeatmap);
</script>

[Back](../)
