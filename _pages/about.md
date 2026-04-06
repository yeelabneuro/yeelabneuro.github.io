---
layout: about
title: about
permalink: /
subtitle: computation. affect. motivation. (neuro)psychiatry.

profile:
  align: right
  image: profile_heartbrain.png
  image_circular: false
  more_info: >
    <p>Department of Psychological and Brain Sciences</p>
    <p>University of Iowa</p>
    <p>Iowa City, IA</p>

selected_papers: false
social: false

announcements:
  enabled: true
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

## Questions we ask

<div class="hero-questions">
  &#8220;<span id="typewriter"></span><span class="cursor"></span>&#8221;
</div>

<script>
const questions = [
  "How does serotonin shape stress and mental effort?",
  "How does the brain represent motivation and affect?",
  "What computations underlie decision-making in the brain?",
  "Can neurocomputational models explain mental illness?",
  "How do therapeutics improve mental health across the lifespan?"
];

let qIndex = 0;
let charIndex = 0;
let deleting = false;
const el = document.getElementById('typewriter');
const speed = { type: 30, delete: 20, pause: 2000 };

function type() {
  const current = questions[qIndex];

  if (!deleting && charIndex <= current.length) {
    el.textContent = current.slice(0, charIndex++);
    setTimeout(type, speed.type);
  } else if (!deleting && charIndex > current.length) {
    deleting = true;
    setTimeout(type, speed.pause);
  } else if (deleting && charIndex >= 0) {
    el.textContent = current.slice(0, charIndex--);
    setTimeout(type, speed.delete);
  } else {
    deleting = false;
    qIndex = (qIndex + 1) % questions.length;
    setTimeout(type, 500);
  }
}

type();
</script>

The **CAMP Lab** at the [University of Iowa](https://psychology.uiowa.edu), directed by **Dr. Debbie Yee**, uses computational, neuroimaging, pharmacological, and neuromodulation approaches to understand how the brain generates **motivation, affect, and decisions** — and how these processes become dysregulated in **mental and neurological illness**.
