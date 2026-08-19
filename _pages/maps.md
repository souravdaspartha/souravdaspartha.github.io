---
layout: archive
title: "Maps"
permalink: /maps/
author_profile: true
---

## Trip Production and Attraction, Gazipur City Corporation

<p style="text-align: justify;">
These maps present zonal trip production and attraction patterns for Gazipur City Corporation, derived from the trip generation step of the four-step travel demand model developed under the Gazipur Comprehensive Transport Masterplan. Production denotes trips originating from each zone, while attraction represents trips drawn to it, together forming the foundational input for subsequent distribution, mode choice, and assignment modelling stages.
</p>

<div style="margin: 18px 0 10px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Trip end</div>
  <button class="pa-btn" data-val="prod" onclick="pickPA(this)">Production</button>
  <button class="pa-btn" data-val="attr" onclick="pickPA(this)">Attraction</button>
</div>

<div style="margin: 12px 0 18px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Year</div>
  <button class="pa-year-btn" data-val="base" onclick="pickPAYear(this)">Base</button>
  <button class="pa-year-btn" data-val="2034" onclick="pickPAYear(this)">2034</button>
  <button class="pa-year-btn" data-val="2044" onclick="pickPAYear(this)">2044</button>
</div>

<a id="paLink" href="/images/pa-prod-base.png" target="_blank" title="Click to open full size">
<img id="paMap" class="mapframe" src="/images/pa-prod-base.png" alt="Trip production and attraction">
</a>

<p><em id="paCaption">Trip production by zone, base year.</em></p>

---

## Trip Desire Lines, Gazipur City Corporation

<p style="text-align: justify;">
Desire lines from the gravity model developed for the Gazipur Comprehensive Transport Masterplan, produced within a four-step travel demand framework. Each line shows the straight-line demand between two zones, indicating where trips want to go rather than the route they take. Width and colour are scaled to trip volume.
</p>

<div style="margin: 18px 0 10px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Trip purpose</div>
  <button class="purpose-btn" data-val="hbw" onclick="pickPurpose(this)">HBW</button>
  <button class="purpose-btn" data-val="hbe" onclick="pickPurpose(this)">HBE</button>
  <button class="purpose-btn" data-val="hbo" onclick="pickPurpose(this)">HBO</button>
  <button class="purpose-btn" data-val="nhb" onclick="pickPurpose(this)">NHB</button>
</div>

<div style="margin: 12px 0 18px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Year</div>
  <button class="year-btn" data-val="base" onclick="pickYear(this)">Base</button>
  <button class="year-btn" data-val="2034" onclick="pickYear(this)">2034</button>
  <button class="year-btn" data-val="2044" onclick="pickYear(this)">2044</button>
</div>

<a id="desireLink" href="/images/desire-hbw-base.png" target="_blank" title="Click to open full size">
<img id="desireMap" class="mapframe" src="/images/desire-hbw-base.png" alt="Trip desire lines">
</a>

<p><em id="desireCaption">Home-based work desire lines, base year.</em></p>

<p style="font-size: 13px; color: #777;">
HBW: home-based work &nbsp;|&nbsp; HBE: home-based education &nbsp;|&nbsp; HBO: home-based other &nbsp;|&nbsp; NHB: non-home-based
</p>

<p style="font-size: 13px; color: #777; text-align: justify;">
Each map is classified on its own volume range, so line widths are not directly comparable across years. Legend values give the actual volumes.
</p>

---

## Trip Length Distribution, Gazipur City Corporation

<p style="text-align: justify;">
Spatial distribution of trip lengths by purpose and forecast year, produced from the distribution step of the four-step travel demand model. Trips are expressed in number of trips, and travel time intervals in minutes. The pattern reflects how far trips travel from each zone, varying by purpose according to the deterrence function applied in the gravity model.
</p>

<div style="margin: 18px 0 10px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Trip purpose</div>
  <button class="tld-btn" data-val="hbw" onclick="pickTld(this)">HBW</button>
  <button class="tld-btn" data-val="hbe" onclick="pickTld(this)">HBE</button>
  <button class="tld-btn" data-val="hbo" onclick="pickTld(this)">HBO</button>
  <button class="tld-btn" data-val="nhb" onclick="pickTld(this)">NHB</button>
</div>

<div style="margin: 12px 0 18px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Year</div>
  <button class="tld-year-btn" data-val="base" onclick="pickTldYear(this)">Base</button>
  <button class="tld-year-btn" data-val="2034" onclick="pickTldYear(this)">2034</button>
  <button class="tld-year-btn" data-val="2044" onclick="pickTldYear(this)">2044</button>
</div>

<a id="tldLink" href="/images/tld-hbw-base.png" target="_blank" title="Click to open full size">
<img id="tldMap" class="tldframe" src="/images/tld-hbw-base.png" alt="Trip length distribution">
</a>

<p><em id="tldCaption">Home-based work trip length distribution, base year.</em></p>

<p style="font-size: 13px; color: #777;">
HBW: home-based work &nbsp;|&nbsp; HBE: home-based education &nbsp;|&nbsp; HBO: home-based other &nbsp;|&nbsp; NHB: non-home-based
</p>

---

## Highway Assignment, Gazipur City Corporation

<p style="text-align: justify;">
Assigned link volumes from the traffic assignment step of the four-step travel demand model. Forecast years are presented under three scenarios: Do Nothing, retaining the existing network without intervention; Business as Usual, reflecting committed schemes already in the pipeline; and Masterplan, incorporating the full set of proposed network and demand management measures.
</p>

<div style="margin: 18px 0 10px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Year</div>
  <button class="as-year-btn" data-val="base" onclick="pickAsYear(this)">Base</button>
  <button class="as-year-btn" data-val="2034" onclick="pickAsYear(this)">2034</button>
  <button class="as-year-btn" data-val="2044" onclick="pickAsYear(this)">2044</button>
</div>

<div id="scenarioRow" style="margin: 12px 0 18px; display: none;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">Scenario</div>
  <button class="as-sc-btn" data-val="donothing" onclick="pickScenario(this)">Do Nothing</button>
  <button class="as-sc-btn" data-val="bau" onclick="pickScenario(this)">Business as Usual</button>
  <button class="as-sc-btn" data-val="masterplan" onclick="pickScenario(this)">Masterplan</button>
</div>

<a id="asLink" href="/images/assign-base.png" target="_blank" title="Click to open full size">
<img id="asMap" class="mapframe" src="/images/assign-base.png" alt="Highway assignment">
</a>

<p><em id="asCaption">Assigned link volumes, base year.</em></p>

---

## Road Crash Density, Gazipur City Corporation

<p style="text-align: justify;">
Animated mapping of 332 road crashes across Gazipur City Corporation Area, playing year by year. The density surface is weighted by severity, with fatal crashes carrying five times the influence of a damage-only collision. The colour scale is held fixed across all years, so intensity is comparable between frames rather than rescaled within each one. Dashed circles mark the five highest-concentration locations identified by Density-Based Spatial Clustering of Applications with Noise (DBSCAN) at a 500 m threshold: Board Bazar, Vogra, Tongi, Salna and Konabari. These clusters are derived from the full study period, not individual years, so their positions and crash counts remain constant as the animation plays.
</p>

<iframe class="mapembed"
        src="/assets/maps/crash-hotspot/accident_hotspot_embed.html?v=2"
        title="Animated road crash density map, Gazipur"
        loading="lazy" frameborder="0">
</iframe>

<p><em>Severity-weighted crash density by year, [2020]&ndash;[2024].</em></p>

<p style="font-size: 13px; color: #777;">
Built in Python with pandas, scikit-learn and folium. &nbsp;|&nbsp;
<a href="/assets/maps/crash-hotspot/accident_hotspot_animated.html" target="_blank">Open full size</a>
</p>

---

## Nighttime Light Expansion, Bangladesh 2013&ndash;2024

<p style="text-align: justify;">
Annual composites of VIIRS Day/Night Band imagery, showing observed nighttime radiance across Bangladesh from 2013 to 2024. Monthly cloud-free composites were reduced to an annual median per pixel and clipped to the national boundary, with the radiance stretch held fixed across every frame so that years are directly comparable. Mean radiance rose nationally from about 0.19 to 0.80 nW/cm&sup2;/sr over the period, concentrating around Dhaka and the Dhaka&ndash;Chattogram corridor while filling in across the western and northern districts.
</p>

<a id="ntlLink" href="/images/bgd_ntl.gif" target="_blank" title="Click to open full size">
<img id="ntlMap" class="ntlframe" src="/images/bgd_ntl.gif" alt="Animated nighttime lights map of Bangladesh, 2013 to 2024">
</a>

<p><em>Annual median nighttime radiance, 2013&ndash;2024.</em></p>

<p style="font-size: 13px; color: #777;">
Processed in Google Earth Engine; cartography and frame export in ArcGIS Pro via arcpy. &nbsp;|&nbsp;
<a href="https://eogdata.mines.edu/products/vnl/" target="_blank">Data: Earth Observation Group</a>
</p>

---

## Bus Route Overlap, Dhaka City

<p style="text-align: justify;">
Route overlap across the 98 active bus routes operating in Dhaka. Each corridor is weighted by the number of routes running along it, with line width scaled to that count. Route alignments were digitised from the published network and simplified into 222 corridor segments, so that each stretch of road carries a single readable value rather than a count that changes block by block. The busiest corridor carries 26 of the 98 routes, concentrated on the north&ndash;south spine through Gulistan and Sayedabad, while much of the network beyond it is served by four routes or fewer. The animated view builds the network up one class at a time, showing how little of the city is reached before the heaviest corridors appear.
</p>

<div style="margin: 18px 0 18px;">
  <div style="font-size: 13px; font-weight: 600; margin-bottom: 6px;">View</div>
  <button class="bro-btn" data-val="static" onclick="pickBro(this)">Static</button>
  <button class="bro-btn" data-val="animated" onclick="pickBro(this)">Animated</button>
</div>

<a id="broLink" href="/images/dhaka-city-bus-route-overlap.png" target="_blank" title="Click to open full size">
<img id="broMap" class="broframe" src="/images/dhaka-city-bus-route-overlap.png" alt="Bus route overlap map of Dhaka City">
</a>

<p><em id="broCaption">Number of bus routes per corridor, all classes.</em></p>

<p style="font-size: 13px; color: #777;">
Route dizitization, corridor network, analysis and frame export in ArcGIS Pro via arcpy.
</p>

---

## Intersection Design, Dhaka South City Corporation

<p style="text-align: justify;">
Conceptual intersection layouts prepared for locations across Dhaka South City Corporation. Each design responds to observed turning movements, pedestrian demand and capacity constraints at the site, developed in Civil 3D alongside traffic, delay and parking survey analysis.
</p>

<div style="display: flex; align-items: center; gap: 12px; margin: 18px 0;">
  <button class="nav-btn" onclick="stepIx(-1)" title="Previous">&#8592;</button>
  <span id="ixCount" style="font-size: 13px; color: #888;">1 / 7</span>
  <button class="nav-btn" onclick="stepIx(1)" title="Next">&#8594;</button>
</div>

<a id="ixLink" href="/images/ix-tatibazar.png" target="_blank" title="Click to open full size">
<img id="ixMap" class="mapframe" src="/images/ix-tatibazar.png" alt="Intersection design">
</a>

<p><em id="ixCaption">Tati Bazar intersection, conceptual design.</em></p>

<style>
.mapframe {
  width: 100%;
  max-width: 550px;
  height: 550px;
  object-fit: contain;
  border: 1px solid rgba(0,0,0,0.25);
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  border-radius: 4px;
  background: #fff;
}
.tldframe {
  max-width: 100%;
  border: 1px solid rgba(0,0,0,0.25);
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  border-radius: 4px;
  background: #fff;
}
.ntlframe {
  width: 100%;
  max-width: 450px;
  border: 1px solid rgba(255,255,255,0.6);
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  border-radius: 4px;
  background: #000;
  display: block;
}
.broframe {
  width: 100%;
  max-width: 450px;
  border: 1px solid rgba(0,0,0,0.25);
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  border-radius: 4px;
  background: #fff;
  display: block;
}
.mapembed {
  width: 100%;
  max-width: 780px;
  height: 900px;
  display: block;
  border: 1px solid rgba(0,0,0,0.25);
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  border-radius: 4px;
  background: #fff;
}
@media (max-width: 700px) {
  .mapembed { height: 600px; }
}
.nav-btn {
  padding: 6px 14px;
  cursor: pointer;
  border: 1px solid rgba(128,128,128,0.4);
  border-radius: 4px;
  background: transparent;
  color: inherit;
  font-size: 16px;
  line-height: 1;
}
.nav-btn:hover {
  background: #1F4E79;
  color: #fff;
  border-color: #1F4E79;
}
.purpose-btn, .year-btn, .pa-btn, .pa-year-btn,
.tld-btn, .tld-year-btn, .as-year-btn, .as-sc-btn, .bro-btn {
  padding: 7px 16px;
  margin-right: 6px;
  margin-bottom: 6px;
  cursor: pointer;
  border: 1px solid rgba(128,128,128,0.4);
  border-radius: 4px;
  background: transparent;
  color: inherit;
  font-size: 14px;
}
.purpose-btn.active, .year-btn.active, .pa-btn.active, .pa-year-btn.active,
.tld-btn.active, .tld-year-btn.active, .as-year-btn.active, .as-sc-btn.active,
.bro-btn.active {
  background: #1F4E79;
  color: #fff;
  border-color: #1F4E79;
}
</style>

<script>
var currentPA = 'prod';
var currentPAYear = 'base';
var currentPurpose = 'hbw';
var currentYear = 'base';
var currentTld = 'hbw';
var currentTldYear = 'base';
var currentAsYear = 'base';
var currentScenario = 'donothing';

var paNames = { prod: 'Trip production by zone', attr: 'Trip attraction by zone' };
var purposeNames = {
  hbw: 'Home-based work',
  hbe: 'Home-based education',
  hbo: 'Home-based other',
  nhb: 'Non-home-based'
};
var yearNames = { base: 'base year', '2034': '2034 forecast', '2044': '2044 forecast' };
var scenarioNames = {
  donothing: 'Do Nothing scenario',
  bau: 'Business as Usual scenario',
  masterplan: 'Masterplan scenario'
};

var broViews = {
  static: {
    ext: 'png',
    caption: 'Number of bus routes per corridor, all classes.'
  },
  animated: {
    ext: 'gif',
    caption: 'Corridors added by route count, 1&ndash;4 through 20&ndash;26.'
  }
};

var ixList = [
  { file: 'ix-tatibazar',        caption: 'Tati Bazar' },
  { file: 'ix-sayedabad-closed', caption: 'Sayedabad (closed intersection)' },
  { file: 'ix-sayedabad-open',   caption: 'Sayedabad (open intersection)' },
  { file: 'ix-maniknagar',       caption: 'Maniknagar' },
  { file: 'ix-atishdipankar',    caption: 'Atish Dipankar' },
  { file: 'ix-khilgaon',         caption: 'Khilgaon Railgate' },
  { file: 'ix-policefari',       caption: 'Police Fari' }
];
var ixIndex = 0;

function setActive(group, btn) {
  document.querySelectorAll('.' + group).forEach(function (b) {
    b.classList.remove('active');
  });
  btn.classList.add('active');
}

function paRefresh() {
  var path = '/images/pa-' + currentPA + '-' + currentPAYear + '.png';
  document.getElementById('paMap').src = path;
  document.getElementById('paLink').href = path;
  document.getElementById('paCaption').innerText = paNames[currentPA] + ', ' + yearNames[currentPAYear] + '.';
}

function pickPA(btn) {
  currentPA = btn.dataset.val;
  setActive('pa-btn', btn);
  paRefresh();
}

function pickPAYear(btn) {
  currentPAYear = btn.dataset.val;
  setActive('pa-year-btn', btn);
  paRefresh();
}

function refresh() {
  var path = '/images/desire-' + currentPurpose + '-' + currentYear + '.png';
  document.getElementById('desireMap').src = path;
  document.getElementById('desireLink').href = path;
  document.getElementById('desireCaption').innerText = purposeNames[currentPurpose] + ' desire lines, ' + yearNames[currentYear] + '.';
}

function pickPurpose(btn) {
  currentPurpose = btn.dataset.val;
  setActive('purpose-btn', btn);
  refresh();
}

function pickYear(btn) {
  currentYear = btn.dataset.val;
  setActive('year-btn', btn);
  refresh();
}

function tldRefresh() {
  var path = '/images/tld-' + currentTld + '-' + currentTldYear + '.png';
  document.getElementById('tldMap').src = path;
  document.getElementById('tldLink').href = path;
  document.getElementById('tldCaption').innerText = purposeNames[currentTld] + ' trip length distribution, ' + yearNames[currentTldYear] + '.';
}

function pickTld(btn) {
  currentTld = btn.dataset.val;
  setActive('tld-btn', btn);
  tldRefresh();
}

function pickTldYear(btn) {
  currentTldYear = btn.dataset.val;
  setActive('tld-year-btn', btn);
  tldRefresh();
}

function asRefresh() {
  var path, caption;
  if (currentAsYear === 'base') {
    path = '/images/assign-base.png';
    caption = 'Assigned link volumes, base year.';
    document.getElementById('scenarioRow').style.display = 'none';
  } else {
    path = '/images/assign-' + currentAsYear + '-' + currentScenario + '.png';
    caption = 'Assigned link volumes, ' + currentAsYear + ' ' + scenarioNames[currentScenario] + '.';
    document.getElementById('scenarioRow').style.display = 'block';
  }
  document.getElementById('asMap').src = path;
  document.getElementById('asLink').href = path;
  document.getElementById('asCaption').innerText = caption;
}

function pickAsYear(btn) {
  currentAsYear = btn.dataset.val;
  setActive('as-year-btn', btn);
  asRefresh();
}

function pickScenario(btn) {
  currentScenario = btn.dataset.val;
  setActive('as-sc-btn', btn);
  asRefresh();
}

function pickBro(btn) {
  var view = broViews[btn.dataset.val];
  setActive('bro-btn', btn);
  var path = '/images/dhaka-city-bus-route-overlap.' + view.ext;
  document.getElementById('broMap').src = path;
  document.getElementById('broLink').href = path;
  document.getElementById('broCaption').innerHTML = view.caption;
}

function stepIx(direction) {
  ixIndex = (ixIndex + direction + ixList.length) % ixList.length;
  var item = ixList[ixIndex];
  var path = '/images/' + item.file + '.png';
  document.getElementById('ixMap').src = path;
  document.getElementById('ixLink').href = path;
  document.getElementById('ixCount').innerText = (ixIndex + 1) + ' / ' + ixList.length;
  document.getElementById('ixCaption').innerText = item.caption + ' intersection, conceptual design.';
}

document.addEventListener('DOMContentLoaded', function () {
  document.querySelector('.pa-btn[data-val="prod"]').classList.add('active');
  document.querySelector('.pa-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.purpose-btn[data-val="hbw"]').classList.add('active');
  document.querySelector('.year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.tld-btn[data-val="hbw"]').classList.add('active');
  document.querySelector('.tld-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.as-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.as-sc-btn[data-val="donothing"]').classList.add('active');
  document.querySelector('.bro-btn[data-val="static"]').classList.add('active');
});
</script>
