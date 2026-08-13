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

## Road Crash Density, Gazipur

<p style="text-align: justify;">
Animated mapping of [N] road crashes across Gazipur, playing year by year. The density surface is weighted by severity, with fatal crashes carrying five times the influence of a damage-only collision. The colour scale is held fixed across all years, so intensity is comparable between frames rather than rescaled within each one. Dashed circles mark the five highest-concentration locations identified by DBSCAN clustering at a 500 m threshold: Board Bazar, Vogra, Tongi, Salna and Konabari.
</p>

<iframe class="mapembed"
        src="/assets/maps/crash-hotspot/accident_hotspot_animated.html"
        title="Animated road crash density map, Gazipur"
        loading="lazy" frameborder="0">
</iframe>

<p><em>Severity-weighted crash density by year, [year]&ndash;[year].</em></p>

<p style="font-size: 13px; color: #777;">
Built in Python with pandas, scikit-learn and folium. &nbsp;|&nbsp;
<a href="/assets/maps/crash-hotspot/accident_hotspot_animated.html" target="_blank">Open full size</a>
</p>

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

.mapembed {
  width: 100%;
  height: 620px;
  border: 1px solid rgba(0,0,0,0.25);
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
  border-radius: 4px;
  background: #fff;
}
@media (max-width: 700px) {
  .mapembed { height: 460px; }
}
  
.purpose-btn, .year-btn, .pa-btn, .pa-year-btn,
.tld-btn, .tld-year-btn, .as-year-btn, .as-sc-btn {
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
.tld-btn.active, .tld-year-btn.active, .as-year-btn.active, .as-sc-btn.active {
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

document.addEventListener('DOMContentLoaded', function () {
  document.querySelector('.pa-btn[data-val="prod"]').classList.add('active');
  document.querySelector('.pa-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.purpose-btn[data-val="hbw"]').classList.add('active');
  document.querySelector('.year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.tld-btn[data-val="hbw"]').classList.add('active');
  document.querySelector('.tld-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.as-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.as-sc-btn[data-val="donothing"]').classList.add('active');
});
</script>
