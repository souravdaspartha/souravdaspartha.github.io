---
layout: archive
title: "Maps"
permalink: /maps/
author_profile: true
---

## Trip Desire Lines, Gazipur City Corporation

Desire lines from the gravity model developed for the Gazipur Comprehensive Transport Masterplan, produced within a four-step travel demand framework. Each line shows the straight-line demand between two zones, indicating where trips want to go rather than the route they take. Width and colour are scaled to trip volume.

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

<a id="desireLink" href="/images/desire-hbw-base.png" target="_blank">
<img id="desireMap" src="/images/desire-hbw-base.png" alt="Trip desire lines" style="max-width: 450px; width: 100%; border: 1px solid rgba(128,128,128,0.3);">
</a>

<p><em id="desireCaption">Home-based work desire lines, base year.</em></p>

<p style="font-size: 13px; color: #777;">
Each map is classified on its own volume range, so a thick line in the base year represents fewer trips than a thick line in 2044. The legend values offer a more reliable basis for comparison across years.
</p>

<p style="font-size: 13px; color: #777;">
HBW: home-based work &nbsp;|&nbsp; HBE: home-based education &nbsp;|&nbsp; HBO: home-based other &nbsp;|&nbsp; NHB: non-home-based
</p>

<style>
.purpose-btn, .year-btn {
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
.purpose-btn.active, .year-btn.active {
  background: #1F4E79;
  color: #fff;
  border-color: #1F4E79;
}
</style>

<script>
var currentPurpose = 'hbw';
var currentYear = 'base';

var purposeNames = {
  hbw: 'Home-based work',
  hbe: 'Home-based education',
  hbo: 'Home-based other',
  nhb: 'Non-home-based'
};
var yearNames = { base: 'base year', '2034': '2034 forecast', '2044': '2044 forecast' };

function refresh() {
  var path = '/images/desire-' + currentPurpose + '-' + currentYear + '.png';
  document.getElementById('desireMap').src = path;
  document.getElementById('desireLink').href = path;
  document.getElementById('desireCaption').innerText = purposeNames[currentPurpose] + ' desire lines, ' + yearNames[currentYear] + '.';
}

function setActive(group, btn) {
  document.querySelectorAll('.' + group).forEach(function (b) {
    b.classList.remove('active');
  });
  btn.classList.add('active');
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
  document.querySelector('.purpose-btn[data-val="hbw"]').classList.add('active');
  document.querySelector('.year-btn[data-val="base"]').classList.add('active');
});
</script>
