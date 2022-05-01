---
layout: about
title: about
permalink: /
description: <a href="https://www.kcl.ac.uk/people/maximilian-pietsch">King's College London</a>

profile:
  align: right
  image: prof_pic.jpg
  # address: >
  #   <p>555 your office number</p>
  #   <p>123 your address street</p>
  #   <p>Your City, State 12345</p>

news: false  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

<!-- Write your biography here. Tell the world about yourself. Link to your favorite [subreddit](http://reddit.com). You can put a picture in, too. The code is already in, just name your picture `prof_pic.jpg` and put it in the `img/` folder.

Put your address / P.O. box / other info right below your picture. You can also disable any these elements by editing `profile` property of the YAML header of your `_pages/about.md`. Edit `_bibliography/papers.bib` and Jekyll will render your [publications page](/al-folio/publications/) automatically.

Link to your social media connections, too. This theme is set up to use [Font Awesome icons](http://fortawesome.github.io/Font-Awesome/) and [Academicons](https://jpswalsh.github.io/academicons/), like the ones below. Add your Facebook, Twitter, LinkedIn, Google Scholar, or just disable all of them. -->

I use machine learning to extract patterns from medical imaging data.

In the weeks around birth, a baby's brain tissue undergoes drastic changes visible on routinely acquired grayscale magnetic resonance imaging scans. However, changes are spatially and temporally varied and it is challenging to extract information that is specific to the processes that are happening on a cellular and morphological level.

I develop methods to learn features from 6D medical imaging data (multi-shell high-angular resolution diffusion weighted magnetic resonance imaging). These data capture the movement of water molecules in and between brain cells which allows probing the orientation-resolved microscopical properties of the developing brain. I use data-driven methods to extract features that allow decomposing the images into interpretable components that are related to brain development. Using these, one can answer questions about normal and abnormal tissue maturation in terms of maturation patterns. With the associated orientation information, one can trace these components throughout white matter pathways of the brain and investigate brain maturation as an interconnected network over time. Applications of these tools facilitate the in-vivo study of normal development and the detection of brain-related abnormalities such as those associated with premature birth.

Another line of my work uses deep learning machine learning techniques to automatically detect and remove signatures of deteriorated data quality. We train a neural network to make the data more consistent — without having access to non-corrupted data. Medical data needs to be interpretable, so we constrain the algorithm's output to changes that are non-local and fully inspectable, increasing the trust in the modified data.

