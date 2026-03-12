---
layout: about
title: about
permalink: /
subtitle: computation. affect. motivation. (neuro)psychiatry.

profile:
  align: right
  image: iowa_seal.jpeg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Dept of Psychological and Brain Sciences</p>
    <p>340 Iowa Ave</p>
    <p>Iowa City, IA 52242</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<div style="padding: 1em; border-left: 4px solid #EFBF04; margin: 1em 0; font-style: italic; font-size: 1.1em;">
  &#8220;<span id="typewriter"></span><span id="cursor" style="border-right: 2px solid #7c4dff; animation: blink 0.7s infinite;">&#8203;</span>&#8221;
</div>

<style>
@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}
</style>

<script>
const questions = [
  "What is the role of serotonin in stress and mental effort?",
  "How does the brain represent motivation and affect?",
  "What are the computations that underlie the neural signals of decision-making?",
  "How can we leverage neurocomputational frameworks to understand mental illness?"
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

Welcome to the Computational Affective Motivational Psychiatry (CAMP) Lab at the [University of Iowa](https://psychology.uiowa.edu), directed by Dr. Debbie Yee! 

We are a team of researchers using comptuational, neuroimaging, pharmacology, and neuromodulation techniques to investigate mechanisms of motivation, affect, and decision-making in humans across the developmental lifespan. Our mission is to leverage neurocomputational frameworks to better inform how these processes are dysregulated in mental and neurological illness.

We are actively recruiting for a full time research assistant / lab manager, graduate students, and postdocs to the join the team! If you are interested in joining the team, please reach out to Dr. Yee with a CV and a short letter of your research interests.