Here's the complete _pages/maps.md with justified paragraphs:

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
<img id="paMap" src="/images/pa-prod-base.png" alt="Trip production and attraction" style="max-width: 550px; width: 100%; border: 1px solid rgba(128,128,128,0.3);">
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
<img id="desireMap" src="/images/desire-hbw-base.png" alt="Trip desire lines" style="max-width: 550px; width: 100%; border: 1px solid rgba(128,128,128,0.3);">
</a>

<p><em id="desireCaption">Home-based work desire lines, base year.</em></p>

<p style="font-size: 13px; color: #777; text-align: justify;">
Each map is classified on its own volume range, so line widths are not directly comparable across years. Legend values give the actual volumes.
</p>

<p style="font-size: 13px; color: #777;">
HBW: home-based work &nbsp;|&nbsp; HBE: home-based education &nbsp;|&nbsp; HBO: home-based other &nbsp;|&nbsp; NHB: non-home-based
</p>

<style>
.purpose-btn, .year-btn, .pa-btn, .pa-year-btn {
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
.purpose-btn.active, .year-btn.active, .pa-btn.active, .pa-year-btn.active {
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

var paNames = { prod: 'Trip production by zone', attr: 'Trip attraction by zone' };
var purposeNames = {
  hbw: 'Home-based work',
  hbe: 'Home-based education',
  hbo: 'Home-based other',
  nhb: 'Non-home-based'
};
var yearNames = { base: 'base year', '2034': '2034 forecast', '2044': '2044 forecast' };

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

document.addEventListener('DOMContentLoaded', function () {
  document.querySelector('.pa-btn[data-val="prod"]').classList.add('active');
  document.querySelector('.pa-year-btn[data-val="base"]').classList.add('active');
  document.querySelector('.purpose-btn[data-val="hbw"]').classList.add('active');
  document.querySelector('.year-btn[data-val="base"]').classList.add('active');
});
</script>
