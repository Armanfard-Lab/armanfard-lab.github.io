---
title: "SeeVita — Data Recording"
layout: page
excerpt: "How to record data for SeeVita (guidelines, privacy, consent)"
permalink: /seevita/data-recording/
sitemap: true
---

<div style="margin: 8px 0 20px 0;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/ismart.png" alt="iSMART / SeeVita" style="max-width: 220px; height: auto;">
</div>

### Overview

SeeVita estimates vital signs from a standard camera, contact‑free. Follow the steps below to capture high‑quality recordings safely and consistently.

<div class="alert alert-info" role="alert" style="margin-top: 8px;">
  By proceeding, you acknowledge that SeeVita is for research, wellness, and screening contexts and is not a medical device. It does not diagnose, treat, or cure any condition.
</div>

### 1) Quick start

1. Ensure even lighting on your face (avoid backlight and harsh shadows).
2. Sit 40–80 cm from the camera at eye level; center your face.
3. Keep still, breathe normally, and avoid talking during capture.
4. Record for 30–60 seconds; longer windows improve stability.
5. Use a modern browser and allow camera permissions when prompted.

### 2) Before you begin

- Eligibility: use when you are seated, calm, and able to remain still for 30–60 seconds.
- Health context: not intended for emergency or critical care use.
- Medical decisions: do not make clinical decisions based on these estimates alone.

### 3) Setup checklist

- Camera: laptop/desktop/phone at 720p or higher, stabilized on a surface
- Environment: steady seat, quiet room, no bright window behind you
- Visibility: remove masks; keep hair clear from forehead/cheeks
- Network: reliable internet to avoid frame drops

### 4) Environment & framing

- Lighting: face a light source; avoid strong backlight or side‑lighting that casts shadows.
- Background: neutral background helps the camera adjust exposure.
- Framing: keep your full face within the frame, forehead and cheeks clearly visible.
- Glasses/makeup: acceptable, but avoid reflective lenses and heavy face coverings.

### 5) Do and don’t

- Do face the camera directly; keep head within frame
- Do maintain a neutral expression and steady posture
- Don’t talk or move excessively during the recording
- Don’t record in low light or high‑contrast lighting

### 6) Recording window

- Duration: at least 30 seconds; 45–60 seconds improves stability for blood pressure and respiration estimates.
- Multiple attempts: if results look unstable, record a second window after resting for 1–2 minutes.

### 7) Privacy and consent

Participate only if you understand and agree to the purpose of recording. For research or clinical use, follow your local consent procedures. We prioritize privacy with minimal retention and de‑identification where feasible. Your data should only be used for the stated purpose. For enterprise integrations, a data processing agreement may be required. Questions? Use our <a href="{{ site.url }}{{ site.baseurl }}/contact/">Contact</a> page.

### 8) Start recording

<p>
  <a class="btn btn-primary" href="{{ site.seevita_demo_url }}" target="_blank" rel="noopener">Launch Demo</a>
  <a class="btn btn-default" href="{{ site.url }}{{ site.baseurl }}/seevita/">Back to SeeVita</a>
</p>

{% if site.seevita_demo_url contains '.mp4' %}
<div class="embed-responsive embed-responsive-16by9" style="margin-top: 16px;">
  <video class="embed-responsive-item" src="{{ site.seevita_demo_url }}" controls preload="metadata"></video>
  <!-- The embedded video illustrates the demo flow. -->
</div>
{% endif %}

### 9) Troubleshooting

- Exposure issues: brighten the room or face a lamp; avoid windows behind you.
- Focus issues: sit still for a moment to let the camera autofocus; clean the lens.
- Performance: close other apps using the camera and reduce background CPU usage.
- Permissions: in browser settings, grant camera access to this site and refresh.

### 10) Disclaimer

SeeVita provides estimates for informational purposes. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of a qualified health provider with any questions you may have regarding a medical condition.


