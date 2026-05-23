---
marp: true
theme: default
paginate: true
size: 16:9
title: Exploring Potential Pathways to Accelerate ePIC Detector Simulation
description: CHEP 2026 deck on acceleration pathways for ePIC detector simulation.
---

<style>
section {
  font-family: Arial, Helvetica, sans-serif;
  color: #1f2933;
  background: #ffffff;
  justify-content: flex-start;
  padding: 18px 56px 28px;
}
h1 {
  color: #123f6d;
  font-size: 42px;
  margin-top: 0;
  margin-bottom: 0.35em;
}
h2 {
  color: #123f6d;
  font-size: 32px;
  margin-top: 0;
  margin-bottom: 0.25em;
}
h3 {
  color: #2f6f8f;
  font-size: 22px;
  margin-top: 0.45em;
  margin-bottom: 0.2em;
}
ul {
  font-size: 22px;
  line-height: 1.35;
}
li {
  margin: 8px 0;
}
strong {
  color: #123f6d;
}
code {
  background: #e8eef3;
  border-radius: 4px;
  padding: 1px 5px;
}
section.title {
  background: #f7fafc;
  padding: 30px 46px 28px;
  overflow: hidden;
}
section.title h1 {
  font-size: 38px;
  line-height: 1.1;
}
.title-layout {
  display: grid;
  grid-template-columns: 0.82fr 1.18fr;
  gap: 26px;
  align-items: center;
  min-height: 420px;
}
.title-copy {
  display: flex;
  flex-direction: column;
  gap: 12px;
}
.title-copy p {
  margin: 0;
}
.nowrap {
  white-space: nowrap;
}
.detector-hero {
  text-align: center;
  align-self: stretch;
  display: flex;
  align-items: center;
  justify-content: center;
}
.detector-hero img {
  width: 112%;
  max-height: 455px;
  object-fit: contain;
  opacity: 0.86;
  mix-blend-mode: multiply;
  filter: saturate(0.96) contrast(1.04);
  -webkit-mask-image: radial-gradient(ellipse at center, #000 55%, rgba(0, 0, 0, 0.72) 72%, transparent 100%);
  mask-image: radial-gradient(ellipse at center, #000 55%, rgba(0, 0, 0, 0.72) 72%, transparent 100%);
}
.title-top {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 26px;
  align-items: center;
  margin-bottom: 14px;
  min-height: 96px;
}
.title-top img {
  max-width: 100%;
  max-height: 86px;
  object-fit: contain;
  justify-self: center;
}
.title-top img:first-child {
  justify-self: start;
}
.two {
  display: grid;
  grid-template-columns: 1.05fr 0.95fr;
  gap: 28px;
  align-items: center;
}
.three {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 18px;
}
.grid-2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 28px;
  align-items: start;
}
.grid-3 {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 18px;
}
.stat {
  border-top: 5px solid #2f6f8f;
  padding-top: 10px;
}
.stat .value {
  font-size: 42px;
  font-weight: 700;
  color: #123f6d;
}
.figure {
  text-align: center;
}
.figure img {
  max-width: 100%;
  max-height: 410px;
  object-fit: contain;
}
section.compact {
  font-size: 23px;
}
.muted {
  color: #5f6b7a;
}
.card {
  background: #ffffff;
  border: 1px solid #d7e1e8;
  border-left: 6px solid #2c7da0;
  border-radius: 6px;
  padding: 16px 18px;
}
.card h3 {
  margin-top: 0;
}
.card ul {
  font-size: 18px;
  padding-left: 22px;
}
.callout {
  background: #e7f2f6;
  border-left: 7px solid #2c7da0;
  border-radius: 4px;
  padding: 14px 18px;
  font-size: 22px;
  line-height: 1.35;
}
.callout strong { display:block; color:#123f6d; margin-bottom:4px; font-size:110%; }
.placeholder {
  background: #fff8e6;
  border-left: 7px solid #c5851c;
  border-radius: 4px;
  padding: 14px 18px;
  font-size: 21px;
}
.small {
  font-size: 17px;
  color: #4a5b66;
}
.img {
  width: 100%;
  max-height: 430px;
  object-fit: contain;
}
.img-small {
  width: 100%;
  max-height: 310px;
  object-fit: contain;
}
table {
  border-collapse: collapse;
  width: 100%;
  font-size: 18px;
}
th, td {
  border: 1px solid #c9d6df;
  padding: 8px 10px;
}
th {
  background: #dfeef4;
  color: #104b73;
}
a {
  color: #1E5BA8;
  text-decoration: underline !important;
}
</style>

<!-- _class: title -->

<p style="position:absolute;bottom:14px;left:46px;font-size:13px;color:#a0aab4;margin:0;">Slide template generated with Claude Sonnet 4.6</p>

<div class="title-top">
  <img src="assets/epic_logo.png" alt="ePIC logo">
  <img src="assets/bnl_logo.png" alt="Brookhaven National Laboratory logo">
  <img src="assets/jefferson_lab_logo.png" alt="Jefferson Lab logo">
  <img src="assets/office_of_science_logo.png" alt="Office of Science logo">
</div>

<div class="title-layout">
<div class="title-copy">

# Exploring Potential Pathways to Accelerate ePIC Detector Simulation</span>

<p style="color:#2f6f8f;font-size:28px;">Sakib Rahman<br>
<span class="nowrap" style="font-size:20px;">on behalf of the ePIC Collaboration</span><br>
<span class="nowrap" style="font-size:20px;">Brookhaven National Laboratory</span></p>

<p style="color:#5f6b7a;font-size:28px;"><span class="nowrap">Computing in High Energy and Nuclear Physics (CHEP)</span><br>
<span class="nowrap">Chulalongkorn University, Bangkok, Thailand</span><br>
<span class="nowrap">26 May 2026</span></p>

</div>

<div class="detector-hero">
  <img src="assets/detector.jpg" alt="ePIC detector rendering">
</div>
</div>

---

## The ePIC Experiment at the Electron-Ion Collider

<div class="grid-3">
  <div class="stat"><div class="value">1157</div><div>Members</div></div>
  <div class="stat"><div class="value">183</div><div>Institutions</div></div>
  <div class="stat"><div class="value">26</div><div>Countries</div></div>
</div>

<div class="grid-2" style="align-items:stretch;">
<div style="display:flex;flex-direction:column;gap:7px;">
<div style="background:#eef4fb;border-left:5px solid #1E5BA8;border-radius:4px;padding:8px 12px;font-size:18px;">
ePIC will be the first detector at the future Electron-Ion Collider. Data taking planned for the <strong>early 2030s</strong>
</div>
<div style="background:#f0f5f9;border-left:5px solid #2f6f8f;border-radius:4px;padding:8px 12px;font-size:18px;">
Being realized through a partnership between host labs: <strong>Brookhaven National Laboratory (BNL)</strong> and <strong>Jefferson Lab (JLab)</strong>
</div>
<div style="flex-grow:1;display:flex;flex-direction:column;justify-content:flex-end;text-align:center;margin-top:7px;">
  <img src="assets/image4.jpg" alt="EIC beam specifications" style="width:100%;object-fit:contain;flex-grow:1;">
  <p class="muted" style="font-size:24px;margin-top:4px;font-weight:bold;">EIC Beam Specifications</p>
</div>
</div>
<div style="display:flex;flex-direction:column;gap:7px;">
<div style="background:#eaf4ea;border-left:5px solid #1E8449;border-radius:4px;padding:8px 12px;font-size:18px;min-height:82px;display:flex;align-items:center;">
Will enable precision studies of nucleons and nuclei at the scale of sea quarks and gluons
</div>
<div style="flex-grow:1;display:flex;flex-direction:column;justify-content:flex-end;text-align:center;margin-top:7px;">
  <img src="assets/image5.png" alt="ePIC collaboration map" style="width:100%;object-fit:contain;flex-grow:1;">
  <p class="muted" style="font-size:24px;margin-top:4px;font-weight:bold;">ePIC: A Global Collaboration</p>
</div>
</div>
</div>

---

## The ePIC Physics & Detector Simulations Working Group

<style>
.orgchart { width:100%; border-collapse:collapse; font-size:14px; }
.orgchart th { background:#2f6f8f; color:#fff; padding:6px 4px; text-align:center; font-size:13px; border:1px solid #2f6f8f; }
.orgchart .spox { background:#123f6d; color:#fff; text-align:center; font-weight:bold; padding:6px; font-size:14px; border:1px solid #123f6d; }
.orgchart td { border:1px solid #c0cdd8; padding:5px 4px; text-align:center; color:#1f2933; vertical-align:middle; }
.orgchart tr:nth-child(even) td { background:#f0f5f9; }
.orgchart tr:nth-child(odd) td { background:#ffffff; }
.orgchart .highlight { background:#e8f4e8 !important; color:#1a5c1a; font-weight:bold; border:2px solid #2a8a2a !important; font-size:15px; }
.resp-boxes { display:grid; grid-template-columns:repeat(3,1fr); gap:12px; margin-top:12px; }
.resp-box { background:#f0f5f9; border-left:4px solid #2f6f8f; border-radius:4px; padding:10px 12px; font-size:19px; line-height:1.35; }
.resp-box strong { display:block; color:#123f6d; margin-bottom:4px; font-size:21px; }
</style>

<div class="grid-2" style="margin-bottom:8px;">
<div style="font-size:21px;">
<ul style="margin:0;padding-left:20px;">
<li>Sits within the <strong>Software &amp; Computing</strong> branch of the ePIC collaboration</li>
<li>Embrace <strong>streaming readout</strong> as data format (<a href="https://indico.cern.ch/event/1471803/contributions/6967323/">See Takuya's talk</a>)</li>
<li>Enable seamless and efficient detector design and integration in simulation, including validation with engineering design</li>
<li>Implement background timing structure</li>
<li>Deliver accurate MC sim with <strong>Geant4</strong> and <strong>DD4hep</strong></li>
<li>Coordinate with User Learning to inform the collaboration about our detector simulation tools (<a href="https://indico.cern.ch/event/1471803/contributions/6968308/">See Alexandr's talk</a>)</li>
</ul>
</div>
<div>
<table class="orgchart">
  <tr><td colspan="3" class="spox" style="background:#123f6d;color:#ffffff;text-align:center;font-weight:bold;padding:6px;font-size:14px;"><a href="https://www.epic-eic.org/collaboration/overview.html" style="color:#ffffff;text-decoration:underline;">SPOKESPERSON'S OFFICE</a></td></tr>
  <tr>
    <th>TECHNICAL<br>COORDINATION</th>
    <th>SOFTWARE &amp;<br>COMPUTING</th>
    <th>ANALYSIS<br>COORDINATORS</th>
  </tr>
  <tr><td>Tracking</td><td class="highlight">⭐ Physics &amp; Detector Simulations</td><td>BSM &amp; Precision EW</td></tr>
  <tr><td>Electronics, Readout &amp; DAQ</td><td>Reconstruction</td><td>Exclusive, Diffraction &amp; Tagging</td></tr>
  <tr><td>AC-LGAD</td><td>Streaming Computing</td><td>Jets &amp; Heavy Flavor</td></tr>
  <tr><td>Calorimetry</td><td>User Learning</td><td>Inclusive Physics</td></tr>
  <tr><td>PID</td><td>Production</td><td>Semi-Inclusive Physics</td></tr>
  <tr><td></td><td>Validation</td><td></td></tr>
</table>
</div>
</div>

<div class="resp-boxes">
  <div class="resp-box"><strong>Explore Acceleration Pathways</strong>Multithreading, sub-event parallelism, and <b>GPU offload</b> to scale simulations across heterogeneous resources in the <b>ePIC Computing Model</b> (<a href="https://indico.cern.ch/event/1471803/contributions/6967120/">See Holly's talk</a>)</div>
  <div class="resp-box"><strong>ML-based Fast Simulation</strong>Rapid iteration across detector configurations and reconstruction algorithms</div>
  <div class="resp-box"><strong>Tractable Background Simulations</strong>Acceleration reduces per-event cost to make large-scale background production and background-inclusive simulations tractable (<a href="https://indico.cern.ch/event/1471803/contributions/6967109/">See my other talk</a>)</div>
</div>

---

## Accelerating ePIC with Multithreading: Physics Validation <span style="font-size:13px;font-weight:bold;color:#c0392b;float:right;letter-spacing:0.04em;">⚠ PRELIMINARY</span>

<div class="callout" style="font-weight:normal;">Tracking η distributions compared across thread counts using 1000 realistic deep inelastic scattering events. Generated charged particles, real-seeded and truth-seeded tracks show consistent agreement.</div>

<p style="font-size:20px;color:#5f6b7a;margin:6px 0 8px;">Enabled by <a href="https://github.com/AIDASoft/DD4hep/pull/1240">DD4hep#1240</a> — multithreading support added to DD4hep.</p>

<div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px;align-items:start;">
  <div style="text-align:center;">
    <div style="font-size:15px;font-weight:600;color:#104b73;margin-bottom:4px;">8 Threads</div>
    <img src="assets/tracking_overlay_8threads_cropped.png" style="width:100%;max-height:500px;object-fit:contain;">
  </div>
  <div style="text-align:center;">
    <div style="font-size:15px;font-weight:600;color:#104b73;margin-bottom:4px;">64 Threads</div>
    <img src="assets/tracking_overlay_64threads_cropped.png" style="width:100%;max-height:500px;object-fit:contain;">
  </div>
  <div style="text-align:center;">
    <div style="font-size:15px;font-weight:600;color:#104b73;margin-bottom:4px;">128 Threads</div>
    <img src="assets/tracking_overlay_128threads_cropped.png" style="width:100%;max-height:500px;object-fit:contain;">
  </div>
</div>
<div style="background:#eef4fb;border-left:4px solid #b3cfe8;border-radius:4px;padding:8px 12px;margin-top:6px;display:flex;justify-content:center;">
  <table style="border-collapse:collapse;width:auto;font-size:13px;color:#5f6b7a;">
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Geometry</td><td style="padding:1px 4px;"><a href="https://github.com/eic/epic/releases/tag/26.04.1" style="color:#5f6b7a;">epic_craterlake 26.04.1</a></td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Container</td><td style="padding:1px 4px;"><a href="https://github.com/eic/containers/pkgs/container/eic_dev_cuda" style="color:#5f6b7a;">eic_dev_cuda:unstable-mr-249</a></td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">CPU</td><td style="padding:1px 4px;">1 × AMD EPYC 7763, 64 physical cores</td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Site</td><td style="padding:1px 4px;">Perlmutter</td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Input</td><td style="padding:1px 4px;"><code style="font-size:9px;word-break:break-all;">root://dtn-eic.jlab.org//volatile/eic/EPIC/EVGEN/DIS/pythia8.316-1.0/NC/noRad/ep/18x275/q2_1to10/pythia8.316-1.0_NC_noRad_ep_18x275_q2_1to10_run000.hepmc3.tree.root</code></td></tr>
  </table>
</div>

---

## Accelerating ePIC with Multithreading: Performance <span style="font-size:13px;font-weight:bold;color:#c0392b;float:right;letter-spacing:0.04em;">⚠ PRELIMINARY</span>

<div class="callout">npsim wall time and memory scaling across thread counts for 1000 realistic deep inelastic scattering events. Either 32 or 64 threads could be optimal running condition.</div>

<div style="display:grid;grid-template-columns:22% 78%;gap:12px;align-items:start;margin-top:8px;">
<div style="background:#f0f5f9;border-radius:4px;padding:8px 10px;">
  <table style="border-collapse:collapse;width:100%;font-size:13px;color:#5f6b7a;">
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Geometry</td><td style="padding:1px 4px;"><a href="https://github.com/eic/epic/releases/tag/26.04.1" style="color:#5f6b7a;">epic_craterlake 26.04.1</a></td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Container</td><td style="padding:1px 4px;"><a href="https://github.com/eic/containers/pkgs/container/eic_dev_cuda" style="color:#5f6b7a;">eic_dev_cuda:unstable-mr-249</a></td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">CPU</td><td style="padding:1px 4px;">1 × AMD EPYC 7763, 64 physical cores</td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Site</td><td style="padding:1px 4px;">Perlmutter</td></tr>
    <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Input</td><td style="padding:1px 4px;"><code style="font-size:9px;word-break:break-all;">root://dtn-eic.jlab.org//volatile/eic/EPIC/EVGEN/DIS/pythia8.316-1.0/NC/noRad/ep/18x275/q2_1to10/pythia8.316-1.0_NC_noRad_ep_18x275_q2_1to10_run000.hepmc3.tree.root</code></td></tr>
  </table>
</div>
<div>
  <img src="assets/walltime_cut.png" style="width:90%;display:block;margin:0 auto;object-fit:contain;">
</div>
</div>

---

## Understanding the Life of ePIC Events

<div style="background:#e7f2f6;border-left:5px solid #2c7da0;border-radius:4px;padding:10px 14px;font-size:21px;color:#104b73;margin-bottom:12px;line-height:1.5;">
  Central, far-forward, and far-backward subsystems provide broad pseudorapidity coverage, enabling the study of many different physics processes. We profile the lifetime of ePIC events to improve our computational efficiency.
</div>

<div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;font-size:20px;color:#1f2933;line-height:1.5;margin-bottom:10px;">
  <div style="background:#f0f5f9;border-radius:6px;padding:10px 14px;">
    <strong style="color:#123f6d;display:block;margin-bottom:4px;">Current Validation</strong>
    Pythia8 NC DIS, 18×275 GeV, Q² = 1–10 GeV², no radiative corrections
  </div>
  <div style="background:#f0f5f9;border-radius:6px;padding:10px 14px;">
    <strong style="color:#123f6d;display:block;margin-bottom:4px;">Future Work</strong>
    Extend to all relevant physics processes. Time budget and acceleration targets vary by dataset
  </div>
</div>
<div style="text-align:center;">
  <img src="assets/lifeOfEpicEvent.png" alt="Life of an ePIC event" style="width:100%;max-height:260px;object-fit:contain;">
  <div style="font-size:17px;color:#5f6b7a;margin-top:4px;"><a href="https://eic.github.io/firebird/">ePIC Detector in the Firebird Event Display</a></div>
</div>

---

## Acceleration Potential: Identify Simulation Time Sinks <span style="font-size:13px;font-weight:bold;color:#c0392b;float:right;letter-spacing:0.04em;">⚠ PRELIMINARY</span>

<div style="display:grid;grid-template-columns:30% 70%;gap:16px;align-items:start;margin-top:0;">
  <div>
    <div style="background:#e7f2f6;border-left:5px solid #2c7da0;border-radius:4px;padding:10px 12px;font-size:20px;color:#104b73;margin-bottom:10px;">Time profiling of single-threaded run with realistic deep inelastic scattering events. The step density plot shows where stepping activity and simulation time is concentrated.</div>
    <div style="background:#f0f5f9;border-radius:6px;padding:8px 12px;display:flex;justify-content:center;">
      <table style="border-collapse:collapse;width:auto;font-size:16px;color:#1f2933;">
        <thead>
          <tr style="border-bottom:2px solid #b3cfe8;">
            <th style="padding:3px 6px;text-align:center;font-weight:700;color:#104b73;">#</th>
            <th style="padding:3px 6px;text-align:left;font-weight:700;color:#104b73;">Subsystem</th>
            <th style="padding:3px 6px;text-align:right;font-weight:700;color:#104b73;">Step %</th>
          </tr>
        </thead>
        <tbody>
          <tr><td style="padding:2px 6px;text-align:center;">1</td><td style="padding:2px 6px;">Far Forward (Other)</td><td style="padding:2px 6px;text-align:right;color:#888;">43.4%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">2</td><td style="padding:2px 6px;">dRICH</td><td style="padding:2px 6px;text-align:right;color:#888;">9.5%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">3</td><td style="padding:2px 6px;">hpDIRC</td><td style="padding:2px 6px;text-align:right;color:#888;">9.0%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">4</td><td style="padding:2px 6px;">Far Forward (ZDC)</td><td style="padding:2px 6px;text-align:right;color:#888;">8.1%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">5</td><td style="padding:2px 6px;">Forward EM+Hadron Cal</td><td style="padding:2px 6px;text-align:right;color:#888;">7.7%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">6</td><td style="padding:2px 6px;">Tracker / Beampipe</td><td style="padding:2px 6px;text-align:right;color:#888;">6.3%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">7</td><td style="padding:2px 6px;">EEEMCal</td><td style="padding:2px 6px;text-align:right;color:#888;">6.1%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">8</td><td style="padding:2px 6px;">Barrel Imaging+SciFi Cal</td><td style="padding:2px 6px;text-align:right;color:#888;">3.6%</td></tr>
          <tr><td style="padding:2px 6px;text-align:center;">9</td><td style="padding:2px 6px;">Barrel HCal</td><td style="padding:2px 6px;text-align:right;color:#888;">1.5%</td></tr>
        </tbody>
      </table>
    </div>
    <div style="background:#e7f2f6;border-left:5px solid #2c7da0;border-radius:4px;padding:7px 10px;font-size:19px;color:#104b73;margin-top:12px;">
      Focuses on stepping time only — track-level actions and other overhead not captured
    </div>
  </div>
  <div style="display:flex;flex-direction:column;gap:6px;margin-top:-20px;">
    <div style="font-size:15px;font-weight:600;color:#1f2933;text-align:center;margin-bottom:2px;">Time-weighted Step Density</div>
    <img src="assets/histos_20260521_205726_93697555_zr_annotated.png" alt="Step density timing heatmap of ePIC detector" style="width:100%;max-height:290px;object-fit:contain;">
    <div style="position:relative;display:inline-block;width:100%;">
      <img src="assets/TotalWalltimePerEvent.jpg" alt="Wall time per event" style="width:100%;max-height:290px;object-fit:contain;">
      <div style="position:absolute;top:6%;left:26%;background:white;padding:3px 32px;border-radius:4px;font-size:16px;font-weight:600;color:#104b73;line-height:1.8;">
        Initialization Time: 58 (s)<br>
        Wall Time/Event: 7.5 (s) 
      </div>
      <div style="position:absolute;bottom:50px;right:-12px;background:#eef4fb;border-left:3px solid #b3cfe8;border-radius:4px;padding:5px 8px;font-size:11px;color:#5f6b7a;max-width:38%;">
        <table style="border-collapse:collapse;width:100%;font-size:11px;color:#5f6b7a;">
          <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">npsim</td><td style="padding:1px 4px;"><a href="https://github.com/eic/npsim/pull/60" style="color:#5f6b7a;">npsim#60</a> @ <code>0c316b6</code></td></tr>
          <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Geometry</td><td style="padding:1px 4px;"><a href="https://github.com/eic/epic/releases/tag/26.05.0" style="color:#5f6b7a;">epic_craterlake 26.05.0</a></td></tr>
          <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Container</td><td style="padding:1px 4px;"><a href="https://github.com/eic/containers/pkgs/container/eic_xl" style="color:#5f6b7a;">eic_xl:26.05.0-stable</a></td></tr>
          <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Input</td><td style="padding:1px 4px;"><code style="font-size:9px;word-break:break-all;">root://dtn-eic.jlab.org//volatile/eic/EPIC/EVGEN/DIS/pythia8.316-1.0/NC/noRad/ep/18x275/q2_1to10/pythia8.316-1.0_NC_noRad_ep_18x275_q2_1to10_run000.hepmc3.tree.root</code></td></tr>
        </table>
      </div>
    </div>
  </div>
</div>

---

## Acceleration Potential: Central Detectors <span style="font-size:13px;font-weight:bold;color:#c0392b;float:right;letter-spacing:0.04em;">⚠ PRELIMINARY</span>

<div style="display:grid;grid-template-columns:75% 25%;gap:12px;align-items:start;margin-top:4px;">
<div style="text-align:center;">
  <div style="font-size:16px;font-weight:600;color:#104b73;margin-bottom:4px;">Central Detectors — 43.6% of stepping time</div>
  <img src="assets/histos_20260521_205726_93697555_heatmap_central.png" alt="Central detector step-density timing heatmap" style="width:100%;max-height:420px;object-fit:contain;">
</div>
<div style="display:flex;flex-direction:column;gap:8px;">
  <div style="background:#eaf4ea;border-left:5px solid #1E8449;border-radius:4px;padding:10px 12px;font-size:19px;color:#1f2933;line-height:1.6;">
    <strong>Subsystem / PID tuning</strong>
    <ul style="margin:4px 0 0;padding-left:18px;font-size:19px;">
      <li>Optical-only acceleration sufficient for hpDIRC and dRICH</li>
      <li>Central-only production: theoretical max <strong>~1.4×</strong> speedup</li>
    </ul>
  </div>
  <div style="background:#f0f5f9;border-radius:4px;padding:8px 10px;">
    <table style="border-collapse:collapse;width:100%;font-size:11px;color:#5f6b7a;">
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">npsim</td><td style="padding:1px 4px;"><a href="https://github.com/eic/npsim/pull/60" style="color:#5f6b7a;">npsim#60</a> @ <code>0c316b6</code></td></tr>
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Geometry</td><td style="padding:1px 4px;"><a href="https://github.com/eic/epic/releases/tag/26.05.0" style="color:#5f6b7a;">epic_craterlake 26.05.0</a></td></tr>
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Container</td><td style="padding:1px 4px;"><a href="https://github.com/eic/containers/pkgs/container/eic_xl" style="color:#5f6b7a;">eic_xl:26.05.0-stable</a></td></tr>
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Input</td><td style="padding:1px 4px;"><code style="font-size:9px;word-break:break-all;">root://dtn-eic.jlab.org//volatile/eic/EPIC/EVGEN/DIS/pythia8.316-1.0/NC/noRad/ep/18x275/q2_1to10/pythia8.316-1.0_NC_noRad_ep_18x275_q2_1to10_run000.hepmc3.tree.root</code></td></tr>
    </table>
  </div>
</div>
</div>

---

## Acceleration Potential: Far Forward Detectors <span style="font-size:13px;font-weight:bold;color:#c0392b;float:right;letter-spacing:0.04em;">⚠ PRELIMINARY</span>

<div style="display:grid;grid-template-columns:75% 25%;gap:12px;align-items:start;margin-top:4px;">
<div style="text-align:center;">
  <div style="font-size:16px;font-weight:600;color:#104b73;margin-bottom:4px;">Far Forward Detectors — 51.5% of stepping time</div>
  <img src="assets/histos_20260521_205726_93697555_heatmap_farfwd.png" alt="Far Forward step-density timing heatmap" style="width:100%;max-height:420px;object-fit:contain;">
</div>
<div style="display:flex;flex-direction:column;gap:8px;">
  <div style="background:#e7f2f6;border-left:5px solid #2c7da0;border-radius:4px;padding:10px 12px;font-size:19px;color:#1f2933;line-height:1.6;">
    <strong>Full ePIC production</strong>
    <ul style="margin:4px 0 0;padding-left:18px;font-size:19px;">
      <li>Far Forward dominates stepping time</li>
      <li>Must accelerate both EM and optical transport for meaningful gains</li>
    </ul>
  </div>
  <div style="background:#f0f5f9;border-radius:4px;padding:8px 10px;">
    <table style="border-collapse:collapse;width:100%;font-size:11px;color:#5f6b7a;">
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">npsim</td><td style="padding:1px 4px;"><a href="https://github.com/eic/npsim/pull/60" style="color:#5f6b7a;">npsim#60</a> @ <code>0c316b6</code></td></tr>
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Geometry</td><td style="padding:1px 4px;"><a href="https://github.com/eic/epic/releases/tag/26.05.0" style="color:#5f6b7a;">epic_craterlake 26.05.0</a></td></tr>
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Container</td><td style="padding:1px 4px;"><a href="https://github.com/eic/containers/pkgs/container/eic_xl" style="color:#5f6b7a;">eic_xl:26.05.0-stable</a></td></tr>
      <tr><td style="padding:1px 4px;white-space:nowrap;font-weight:600;">Input</td><td style="padding:1px 4px;"><code style="font-size:9px;word-break:break-all;">root://dtn-eic.jlab.org//volatile/eic/EPIC/EVGEN/DIS/pythia8.316-1.0/NC/noRad/ep/18x275/q2_1to10/pythia8.316-1.0_NC_noRad_ep_18x275_q2_1to10_run000.hepmc3.tree.root</code></td></tr>
    </table>
  </div>
</div>
</div>

---

## Simphony: GPU Acceleration for Optical Photons

<p style="font-size:22px;margin:0 0 10px;"><a href="https://github.com/BNLnpps/simphony">Simphony</a> (prev. EIC-Opticks) is a fork developed at BNL of <a href="https://github.com/simoncblyth/opticks">Opticks</a> (Simon Blyth). During full Geant4 Monte Carlo simulation, optical photon transport is accelerated using the GPU-based NVIDIA OptiX framework.</p>

<p style="font-size:18px;font-weight:700;color:#1E5BA8;margin:0 0 4px;letter-spacing:0.04em;text-transform:uppercase;">Experiment-agnostic Improvements</p>
<div style="display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-bottom:10px;">
<div style="background:#eef4fb;border:1px solid #b3cfe8;border-left:6px solid #1E5BA8;border-radius:6px;padding:16px 18px;">
<h3 style="color:#1E5BA8;margin-top:0;">Ease of Deployment</h3>

- [Spack package](https://github.com/eic/eic-spack/blob/1569098e2b9c7f88948f74416938a458d0386632/spack_repo/eic/packages/simphony/package.py#L11)
- [Tagged containers](https://github.com/eic/containers/pkgs/container/eic_dev_cuda)

</div>
<div style="background:#eef4fb;border:1px solid #b3cfe8;border-left:6px solid #1E5BA8;border-radius:6px;padding:16px 18px;">
<h3 style="color:#1E5BA8;margin-top:0;">Additional Core Functionality</h3>

- Wavelength shifting
- External JSON configuration (in place of environment variables)

</div>
</div>
<div style="display:grid;grid-template-columns:repeat(2,1fr);gap:12px;">
<div style="background:#eaf4ea;border:1px solid #a8d5a8;border-left:6px solid #1E8449;border-radius:6px;padding:16px 18px;">
<h3 style="color:#1E8449;margin-top:0;">Examples of New Use Cases</h3>

- Event batching — improves GPU efficiency for ePIC-like low-to-moderate photon yields per event
- Monte Carlo truth propagation
- Maximize CPU and GPU utilization through overlapping execution
- DD4hep integration

</div>
<div style="background:#eaf4ea;border:1px solid #a8d5a8;border-left:6px solid #1E8449;border-radius:6px;padding:16px 18px;">
<h3 style="color:#1E8449;margin-top:0;">Geometry-specific Parameter Tuning</h3>

- Max photon steps per kernel launch — prevents long-lived stragglers stalling threads
- Ray offset tuning for better fidelity

</div>
</div>

---

## Simphony Use Case: Standalone ePIC Subsystem Design Simulations

<div style="display:grid;grid-template-columns:22% 56% 22%;gap:10px;align-items:center;margin-top:4px;">

<div style="display:flex;flex-direction:column;gap:8px;">
  <div style="background:white;border:2px solid #b3cfe8;border-radius:4px;padding:3px;">
    <img src="assets/PFRICHdetector.jpg" alt="pfRICH" style="width:100%;object-fit:contain;">
    <p style="text-align:center;font-size:11px;font-weight:700;color:#1E5BA8;margin:2px 0 1px;">pfRICH · <a href="https://arxiv.org/abs/2512.14598" style="font-weight:400;font-size:10px;color:#5f6b7a;">Dongwi et al. (2025)</a></p>
  </div>
  <div class="callout" style="font-size:20px;padding:10px 12px;line-height:1.5;">
    Optical photon transport dominates simulation time for PID detectors: hpDIRC, pfRICH and dRICH.<br>
    <span style="font-size:15px;color:#5f6b7a;"><a href="https://arxiv.org/abs/2410.20410" style="color:#5f6b7a;">C. Chatterjee et al. (2024)</a></span>
  </div>
</div>

<div style="display:flex;flex-direction:column;gap:6px;">
  <img src="assets/ePICCentralDetector.jpg" alt="ePIC Central Detector" style="width:100%;object-fit:contain;">
  <div style="background:white;border:2px solid #b3cfe8;border-radius:4px;padding:3px;">
    <img src="assets/HPDIRCDetector.jpg" alt="hpDIRC" style="width:50%;display:block;margin:0 auto;object-fit:contain;">
    <p style="text-align:center;font-size:11px;font-weight:700;color:#1E5BA8;margin:2px 0 1px;">hpDIRC · <a href="https://indico.bnl.gov/event/26584/contributions/102777/attachments/62225/107677/20250612-hpDIRC-DACmeeting_GK.pdf" style="font-weight:400;font-size:10px;color:#5f6b7a;">G. Kalicy (2025)</a></p>
  </div>
</div>

<div style="display:flex;flex-direction:column;justify-content:flex-start;gap:8px;">
  <div style="background:white;border:2px solid #b3cfe8;border-radius:4px;padding:3px;">
    <img src="assets/drich-detector.jpg" alt="dRICH" style="width:100%;object-fit:contain;">
    <p style="text-align:center;font-size:11px;font-weight:700;color:#1E5BA8;margin:2px 0 1px;">dRICH · <a href="https://indico.bnl.gov/event/31228/contributions/118734/attachments/67379/115790/rich2025-contalbrigo_2col.pdf" style="font-weight:400;font-size:10px;color:#5f6b7a;">Contalbrigo et al. (2026)</a></p>
  </div>
</div>

</div>

---

## Simphony: Validation and Performance for ePIC Use Cases

<div style="display:grid;grid-template-columns:1fr 1fr;gap:18px;align-items:start;">
<div>
<p style="font-size:19px;font-weight:700;color:#123f6d;margin:0 0 6px;">Physics Validation — pfRICH</p>
<ul style="font-size:18px;line-height:1.5;margin:0 0 8px;">
  <li>50,000 electrons · p = 5 MeV/c · ~44M optical photons</li>
  <li>Recorded hits agree within statistical uncertainties:<br>
    Geant4: 8.693 ± 0.003 M<br>
    Simphony: 8.694 ± 0.003 M</li>
</ul>
  <div style="overflow:hidden;position:relative;">
    <img src="assets/SimphonyPFrichHitmap.jpg" alt="pfRICH hit map comparison" style="width:100%;margin-top:-1.4px;object-fit:contain;">
    <div style="position:absolute;top:0;left:0;right:0;display:flex;font-size:15px;font-weight:700;color:#1f2933;background:#ffffff;padding:2px 0;">
      <span style="width:50%;text-align:center;padding-left:12%;">Geant4</span><span style="width:50%;text-align:center;padding-right:12%;">Simphony</span>
    </div>
  </div>
</div>
<div>
<p style="font-size:19px;font-weight:700;color:#123f6d;margin:0 0 4px;">Performance — pfRICH</p>
<p style="font-size:15px;color:#5f6b7a;margin:0 0 6px;">GPU: NVIDIA GeForce RTX 4090 · CPU: Intel Xeon w7-3445</p>
<div style="position:relative;display:flex;align-items:center;">
  <div style="display:flex;flex-direction:column;align-items:center;margin-right:4px;">
    <span style="writing-mode:vertical-rl;transform:rotate(180deg);font-size:18px;font-weight:700;color:#1f2933;white-space:nowrap;">G4 time / Simphony time</span>
  </div>
  <div style="position:relative;flex:1;">
    <img src="assets/PerformanceSimphony.jpg" alt="Simphony speedup versus Geant4 threads" style="width:100%;max-height:360px;object-fit:contain;">
    <div style="position:absolute;top:0;left:0;width:60px;bottom:0;background:#ffffff;"></div>
    <span style="position:absolute;top:18%;left:34px;font-size:14px;color:#1f2933;">10²</span>
    <span style="position:absolute;top:78%;left:34px;font-size:14px;color:#1f2933;">10¹</span>
    <span style="position:absolute;top:40px;right:60px;font-size:16px;color:#5f6b7a;"><a href="https://arxiv.org/abs/2512.06061" style="color:#5f6b7a;">G. Galgoczi et al. (2025) arXiv:2512.06061</a></span>
  </div>
</div>
</div>
</div>

<div style="text-align:center;margin-top:8px;">
<div style="display:inline-block;background:#e7f2f6;border-left:7px solid #2c7da0;border-radius:4px;padding:10px 18px;font-size:18px;line-height:1.5;text-align:left;">
<ul style="margin:0;padding-left:18px;">
<li>Validation and performance studies for dRICH and hpDIRC ongoing</li>
<li>Preliminary hpDIRC result: <strong>~260× speedup</strong> vs single-thread Geant4 with 10M optical photons</li>
<li>We hope to reproduce these studies across a range of heterogeneous resources</li>
</ul>
</div>
</div>


---

## AdePT and Celeritas: EM GPU Acceleration

<div class="callout" style="font-size:23px;margin:0 0 10px;"><a href="https://github.com/apt-sim/AdePT" style="font-weight:700;">AdePT</a> and <a href="https://github.com/celeritas-project/celeritas" style="font-weight:700;">Celeritas</a> both offload EM shower transport to GPU by leveraging the Geant4 Tracking Manager, and can potentially enable GPU-accelerated ePIC simulation.</div>

<div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px;">

<div style="background:#fff8e6;border-left:4px solid #b07d00;border-radius:4px;padding:10px 14px;font-size:23px;">
<strong>Exploring Celeritas in ePIC</strong>
<ul style="margin:8px 0 0;padding-left:18px;font-size:22px;">
<li>Added <a href="https://github.com/celeritas-project/celeritas/tree/develop/example/ddceler">DD4hep plugin</a></li>
<li>Added support for realistic ePIC 3D RZ field maps</li>
<li>Partial MC truth propagation</li>
<li><em>Work in progress:</em>
  <ul style="margin:4px 0 0;padding-left:18px;">
  <li>Optical photon support in DD4hep plugin for comparisons with Simphony</li>
  <li>Benchmarks with realistic DIS events on simple pre-shower geometry</li>
  <li>Benchmarks on standalone calorimeter subsystem</li>
  </ul>
</li>
</ul>
</div>

<div class="callout" style="font-size:23px;">
<strong>Exploring AdePT in ePIC</strong>
<ul style="margin:8px 0 0;padding-left:18px;font-size:22px;">
<li>Added <a href="https://github.com/AIDASoft/DD4hep/pull/1606">DD4hep plugin</a></li>
<li>End-to-end pipeline with MC truth propagation</li>
<li>Example SiD geometry: fully working, initial benchmarking done</li>
<li><em>Work in progress:</em>
  <ul style="margin:4px 0 0;padding-left:18px;">
  <li>Implementing solution for tessellated regions in ePIC geometry</li>
  <li>Detailed ePIC simulation benchmarking</li>
  </ul>
</li>
</ul>
</div>

</div>

---

## Accelerated Simulations: hpDIRC Example and Beyond

<div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:14px;align-items:stretch;">

<div>
<div style="background:#f0f5f9;border-left:4px solid #2f6f8f;border-radius:4px;padding:14px 16px;font-size:19px;line-height:1.5;">
<strong style="display:block;color:#123f6d;font-size:21px;margin-bottom:8px;">Foundation Model for DIRC Detectors</strong>
<ul style="margin:0;padding-left:18px;">
<li>Transformer-based Foundation Model with a Mixture-of-Experts (MoE) architecture developed for DIRC detectors [<a href="https://iopscience.iop.org/article/10.1088/2632-2153/ae3d81">1</a>,<a href="https://arxiv.org/abs/2604.24775">4</a>]</li>
<li>Single pre-trained FM supports multiple downstream applications via fine-tuning:
  <ul style="margin:4px 0 0 0;padding-left:16px;">
    <li>High-fidelity, fast simulations (topology + photon yield)</li>
    <li>Near real-time PID / Classification</li>
    <li>Noise Filtering</li>
  </ul>
</li>
<li>Demonstrated on the ePIC hpDIRC and the GlueX DIRC at Jefferson Lab [<a href="https://iopscience.iop.org/article/10.1088/2632-2153/ae3d81">1</a>,<a href="https://iopscience.iop.org/article/10.1088/2632-2153/ada8f4">2</a>,<a href="https://arxiv.org/abs/2504.19042">3</a>,<a href="https://arxiv.org/abs/2604.24775">4</a>], and now being extended to calorimetry [<a href="https://arxiv.org/abs/2603.28804">5</a>]</li>
</ul>
</div>

<div style="margin-top:10px;font-size:14px;color:#5f6b7a;line-height:1.6;">
[<a href="https://iopscience.iop.org/article/10.1088/2632-2153/ae3d81">1</a>] J. Giroux, C. Fanelli, <em>MLST</em> 7.1 (2026): 015031 &nbsp;
[<a href="https://iopscience.iop.org/article/10.1088/2632-2153/ada8f4">2</a>] C. Fanelli et al., <em>MLST</em> 6.1 (2025): 015028 &nbsp;
[<a href="https://arxiv.org/abs/2504.19042">3</a>] J. Giroux et al., <em>MLST</em> 6 (2025): 040501 &nbsp;
[<a href="https://arxiv.org/abs/2604.24775">4</a>] C. Fanelli et al., arXiv:2604.24775 (2026) &nbsp;
[<a href="https://arxiv.org/abs/2603.28804">5</a>] C. Cardona et al., arXiv:2603.28804 (2026)
</div>
</div>

<div style="display:flex;flex-direction:column;align-items:center;gap:8px;height:100%;">
<div style="width:100%;text-align:center;flex:1;">
<img src="assets/MOdelingResponse_sharp.jpg" alt="Foundation Model for ePIC" style="width:100%;max-height:260px;object-fit:contain;border-radius:4px;">
<p style="font-size:16px;font-weight:600;color:#2f6f8f;margin:3px 0 0;">Foundation Model for ePIC</p>
</div>
<div style="width:100%;text-align:center;flex:1;">
<img src="assets/ModelingResponseGluex_sharp.jpg" alt="Foundation Model for GlueX" style="width:100%;max-height:260px;object-fit:contain;border-radius:4px;">
<p style="font-size:16px;font-weight:600;color:#2f6f8f;margin:3px 0 0;">Foundation Model for GlueX</p>
</div>
</div>

</div>


---

## Acceleration Challenges

<div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-top:8px;">
  <div style="background:#e7f2f6;border-left:7px solid #2c7da0;border-radius:4px;padding:14px 18px;font-size:22px;line-height:1.35;"><strong style="display:block;color:#123f6d;margin-bottom:4px;font-size:110%;">CUDA Architecture Portability</strong>GPU payloads and all dependencies must be built against the CUDA arch of the destination hardware; mismatched builds cause runtime crashes</div>
  <div style="background:#fff8e6;border-left:7px solid #b07d00;border-radius:4px;padding:14px 18px;font-size:22px;line-height:1.35;"><strong style="display:block;color:#7a5500;margin-bottom:4px;font-size:110%;">GPU Parameter Tuning</strong>GPU-specific parameters must be tuned to event topology per dataset and available hardware resources</div>
  <div style="background:#f0f5f9;border-left:7px solid #2f6f8f;border-radius:4px;padding:14px 18px;font-size:22px;line-height:1.35;"><strong style="display:block;color:#123f6d;margin-bottom:4px;font-size:110%;">Workflow Integration</strong>PanDA WMS adaptive brokerage will match containers to GPU resources, but the container build matrix grows with each new arch target</div>
  <div style="background:#eaf4ea;border-left:7px solid #1E8449;border-radius:4px;padding:14px 18px;font-size:22px;line-height:1.35;"><strong style="display:block;color:#1a5c1a;margin-bottom:4px;font-size:110%;">Physics Validation Fidelity</strong>GPU-offloaded transport must reproduce Geant4 reference within analysis-level tolerances across all relevant observables</div>
  <div style="background:#f5eef8;border-left:7px solid #7d3c98;border-radius:4px;padding:14px 18px;font-size:22px;line-height:1.35;"><strong style="display:block;color:#5b2c6f;margin-bottom:4px;font-size:110%;">ML Model Generalization</strong><ul style="margin:6px 0 0 0;padding-left:18px;"><li>Models must be trained to take into account different beam conditions, physics processes and kinematic ranges</li><li>Retraining is needed when geometry changes as well</li></ul></div>
  <div style="background:#fdecea;border-left:7px solid #c0392b;border-radius:4px;padding:14px 18px;font-size:22px;line-height:1.35;"><strong style="display:block;color:#922b21;margin-bottom:4px;font-size:110%;">Event Batching and Sub-event Level Parallelism</strong><ul style="margin:6px 0 0 0;padding-left:18px;"><li>Address GPU under-utilization due to simplistic ePIC event topology</li><li>Integration challenges yet to be carefully studied</li></ul></div>
</div>


---

## Summary and Near-Term Work

<div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-top:4px;align-items:start;">

<div style="background:#f0f5f9;border-left:4px solid #2f6f8f;border-radius:4px;padding:12px 16px;font-size:20px;line-height:1.5;">
<strong style="display:block;color:#123f6d;font-size:21px;margin-bottom:6px;">What We Showed</strong>
<ul style="margin:0;padding-left:18px;">
<li>Multithreading enabled in DD4hep
  <ul><li>Physics-validated, optimal at 32–64 threads</li></ul>
</li>
<li>Preliminary profiling shows that optical photons and EM showers dominate simulation cost</li>
<li>Simphony:
  <ul>
  <li>GPU acceleration for optical photons in ePIC PID detectors</li>
  <li>Order-of-magnitude speedup vs 20 Geant4 threads, validated on pfRICH</li>
  </ul>
</li>
</ul>
</div>

<div style="background:#e8f4e8;border-left:4px solid #1E8449;border-radius:4px;padding:12px 16px;font-size:20px;line-height:1.5;">
<strong style="display:block;color:#1a5c1a;font-size:21px;margin-bottom:6px;">What We Are Exploring</strong>
<ul style="margin:0;padding-left:18px;">
<li>AdePT and Celeritas:
  <ul>
  <li>GPU acceleration for EM tracks</li>
  <li>Integration and benchmarking in progress</li>
  </ul>
</li>
<li>ML-based fast simulation/Foundation models
  <ul>
  <li>hpDIRC example</li>
  <li>Large-scale training data generation with Simphony</li>
  </ul>
</li>
<li>Event batching and sub-event level parallelism</li>
</ul>
</div>

</div>

<div style="text-align:center;margin-top:12px;">
<img src="assets/ePICevent.jpg" style="width:90%;border-radius:6px;object-fit:contain;">
</div>

---

<!-- _class: compact -->

## Related ePIC Talks at CHEP 2026

<div class="title-top" style="margin-bottom:8px;">
  <img src="assets/epic_logo.png" alt="ePIC logo">
  <img src="assets/bnl_logo.png" alt="Brookhaven National Laboratory logo">
  <img src="assets/jefferson_lab_logo.png" alt="Jefferson Lab logo">
  <img src="assets/office_of_science_logo.png" alt="Office of Science logo">
</div>

<div style="display:flex;flex-direction:column;gap:12px;margin-top:8px;font-size:20px;">

<div style="background:#eef4fb;border-left:5px solid #1E5BA8;border-radius:4px;padding:10px 16px;">
<strong style="color:#1E5BA8;"><a href="https://indico.cern.ch/event/1471803/contributions/6967120/" style="color:#1E5BA8;text-decoration:underline;">The ePIC Streaming Computing Model</a></strong><br>
<span class="muted">Holly Szumila-Vance</span>
</div>

<div style="background:#eaf4ea;border-left:5px solid #1E8449;border-radius:4px;padding:10px 16px;">
<strong style="color:#1E8449;"><a href="https://indico.cern.ch/event/1471803/contributions/6967109/" style="color:#1E8449;text-decoration:underline;">Scaling ePIC Simulation Production: Distributed Workflow and Data Management</a></strong><br>
<span class="muted">Sakib Rahman</span>
</div>

<div style="background:#f3eef8;border-left:5px solid #7B3FA0;border-radius:4px;padding:10px 16px;">
<strong style="color:#7B3FA0;"><a href="https://indico.cern.ch/event/1471803/contributions/6967323/" style="color:#7B3FA0;text-decoration:underline;">Development of Streaming Data Reconstruction for ePIC Experiment at EIC</a></strong><br>
<span class="muted">Takuya Kumaoka</span>
</div>

<div style="background:#fdf6e3;border-left:5px solid #b07d00;border-radius:4px;padding:10px 16px;">
<strong style="color:#b07d00;"><a href="https://indico.cern.ch/event/1471803/contributions/6968308/" style="color:#b07d00;text-decoration:underline;">ePIC User Learning Training and Documentation Strategies</a></strong><br>
<span class="muted">Alexandr Prozorov</span>
</div>

</div>
