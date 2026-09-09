---
permalink: /
title: "Welcome!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Qiaoyi, a fifth-year PhD student in Political Science at the University of Illinois at Urbana-Champaign. My broader research interests lie in American politics, with a primary focus on political behavior and political psychology. Specifically, I study the psychological foundations of political attitudes and behavior. I am particularly interested in how social identities, such as race and gender, shape individuals' perceptions of and interactions with in-group and out-group members. I also examine how the lived experiences of minority group members influence their political views and actions.

You can reach me by email at [qiaoyin2@illinois.edu](mailto:qiaoyin2@illinois.edu). See my [CV](/cv/), [Research](/research/), and [Teaching](/teaching/) for more.

Education
======
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin="" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
<style>
.edu-emblem { background:#fff; border:2px solid #002147; border-radius:50%; box-shadow:0 1px 4px rgba(0,0,0,.35); object-fit:contain; padding:2px; }
#edu-map .leaflet-popup-content { font-size:.85em; line-height:1.4; }
</style>

<div id="edu-map" style="height:420px; border:1px solid #ddd; border-radius:8px; margin:1em 0;"></div>
<script>
(function(){
  function init(){
    var map = L.map('edu-map', { scrollWheelZoom:false });
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 18, attribution: '&copy; OpenStreetMap contributors'
    }).addTo(map);
    function emblem(url){ return L.icon({ iconUrl:url, iconSize:[46,46], iconAnchor:[23,23], popupAnchor:[0,-22], className:'edu-emblem' }); }
    var schools = [
      { lat:40.1020, lng:-88.2272, icon:'/images/logo-uiuc.png',
        html:'<strong>University of Illinois at Urbana-Champaign</strong><br>Ph.D. in Political Science (2022 &ndash; Present)<br>M.A. in Political Science (2022 &ndash; 2024)' },
      { lat:39.9469, lng:116.3047, icon:'/images/logo-bfsu.png',
        html:'<strong>Beijing Foreign Studies University</strong><br>M.A. in English, American Studies (2019 &ndash; 2022)' },
      { lat:29.5847, lng:106.4267, icon:'/images/logo-sisu.png',
        html:'<strong>Sichuan International Studies University</strong><br>B.A. in English Language and Literature (2015 &ndash; 2019)' }
    ];
    var markers = schools.map(function(s){
      return L.marker([s.lat, s.lng], { icon: emblem(s.icon) }).addTo(map).bindPopup(s.html);
    });
    map.fitBounds(L.featureGroup(markers).getBounds().pad(0.3));
  }
  if (window.L) { init(); } else { window.addEventListener('load', init); }
})();
</script>

- <img src="/images/logo-uiuc.png" alt="University of Illinois" style="height:22px; vertical-align:middle; margin-right:8px;"> **Ph.D. in Political Science**, University of Illinois at Urbana-Champaign, 2022 – Present
- <img src="/images/logo-uiuc.png" alt="University of Illinois" style="height:22px; vertical-align:middle; margin-right:8px;"> **M.A. in Political Science**, University of Illinois at Urbana-Champaign, 2022 – 2024
- <img src="/images/logo-bfsu.png" alt="Beijing Foreign Studies University" style="height:22px; vertical-align:middle; margin-right:8px;"> **M.A. in English (American Studies)**, Beijing Foreign Studies University, 2019 – 2022
- <img src="/images/logo-sisu.png" alt="Sichuan International Studies University" style="height:22px; vertical-align:middle; margin-right:8px;"> **B.A. in English Language and Literature**, Sichuan International Studies University, 2015 – 2019

Research Interests
======
<div style="display:grid; grid-template-columns:repeat(2, 1fr); gap:1.2em; margin-top:1em;">

  <figure style="margin:0; text-align:center;">
    <img src="/images/racial-ethnic-politics.jpg" alt="Racial and Ethnic Politics" style="width:100%; aspect-ratio:16/10; object-fit:cover; border-radius:8px; border:1px solid #ddd;">
    <figcaption style="margin-top:.5em; font-weight:700; color:#002147;">Racial and Ethnic Politics</figcaption>
  </figure>

  <figure style="margin:0; text-align:center;">
    <img src="/images/political-behavior.jpg" alt="Political Participation" style="width:100%; aspect-ratio:16/10; object-fit:cover; border-radius:8px; border:1px solid #ddd;">
    <figcaption style="margin-top:.5em; font-weight:700; color:#002147;">Political Participation</figcaption>
  </figure>

  <figure style="margin:0; text-align:center;">
    <img src="/images/political-psychology.jpg" alt="Political Psychology (Stereotypes and Biases)" style="width:100%; aspect-ratio:16/10; object-fit:cover; border-radius:8px; border:1px solid #ddd;">
    <figcaption style="margin-top:.5em; font-weight:700; color:#002147;">Political Psychology (Stereotypes and Biases)</figcaption>
  </figure>

  <figure style="margin:0; text-align:center;">
    <img src="/images/survey-experimental.jpg" alt="Survey Design and Experimental Research" style="width:100%; aspect-ratio:16/10; object-fit:cover; border-radius:8px; border:1px solid #ddd;">
    <figcaption style="margin-top:.5em; font-weight:700; color:#002147;">Survey Design and Experimental Research</figcaption>
  </figure>

</div>
