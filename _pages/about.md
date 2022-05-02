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

I use machine learning to extract information from medical imaging data.

In the weeks around birth, a baby's brain tissue undergoes drastic changes visible on routinely acquired grayscale magnetic resonance imaging scans. However, changes are spatially and temporally varied and it is challenging to extract information that is specific to the processes that are happening on a cellular and morphological level.

I develop methods to learn features from 6D medical imaging data (multi-shell high-angular resolution diffusion-weighted magnetic resonance imaging). These data capture the movement of water molecules in and between brain cells which allows probing orientation-resolved microscopical properties of the developing brain. I use data-driven methods to extract features that allow decomposing the images into interpretable components that are related to brain development. Using these, one can answer questions about normal and abnormal tissue maturation in terms of maturation patterns. With the associated orientation information, one can trace these components throughout white matter pathways of the brain and investigate brain maturation as an interconnected network over time. Applications of these tools facilitate the in-vivo study of normal development and the detection of brain-related abnormalities such as those associated with premature birth.

Data were released in the form of a normative [atlas](https://gin.g-node.org/maxpietsch/dHCP_neonatal_HARDI_atlas/) of neonatal brain development from data acquired as part of the [developing Human Connectome Project](http://www.developingconnectome.org/). Images from this work were featured in news articles in [Wired](https://www.wired.co.uk/gallery/developing-human-connectome-project), [BBC](https://www.bbc.co.uk/news/health-39854654), [Guardian](https://www.theguardian.com/science/2017/may/10/project-to-map-human-brain-from-womb-to-birth-releases-stunning-images), and [Nature Outlook](https://www.nature.com/articles/d41586-019-02208-0) and are shown below:
<img src="assets/img/dhcp_neo.jpg" alt="Neonatal tissue matruation contrast" width="100%"/>

<!-- - [From womb to world: scans capture how our brains develop during pregnancy and beyond](https://www.wired.co.uk/gallery/developing-human-connectome-project) (Wired, 15 May 2017),
- [Project to map human brain from womb to birth releases stunning images](https://www.theguardian.com/science/2017/may/10/project-to-map-human-brain-from-womb-to-birth-releases-stunning-images) (Guardian, 10 May 2017)
- [Baby brain scans reveal trillions of neural connections](https://www.bbc.co.uk/news/health-39854654) (BBC, 10 May 2017)
- [How to map the brain](https://www.nature.com/articles/d41586-019-02208-0) (Nature Outlook, 24 July 2019) -->


Another line of my work uses deep learning to automatically detect and remove signatures of deteriorated data quality in diffusion MRI data. We train a convolutional neural network to make the data more consistent — without having access to non-corrupted data. Instead of supervised learning, we train the network using techniques based in statistical learning theory. Deep neural networks are powerful models but they can introduce artefacts into the images which is at odds with the need of medical data to be interpretable. We approach this problem by constraining the network to produce limited and well-defined changes that bound the scope of introducing local artefacts, therefore increasing the trust in the modified data. The code and pretrained neural network can be downloaded as Docker image from [github.com/maxpietsch/dStripe](https://github.com/maxpietsch/dStripe).
<img src="assets/img/dstripe.png" alt="dStripe" width="100%"/>

In recent work on placental health modelling, we predict health scores using a fast and clinical T2* weighted MRI scan. This work utilises placental mean T2* as an age-dependent biomarker for placental health. The method is clinically appealing as it is fast and fully automated and it operates in two stages with human-interpretable output: deep-learning-based organ segmentation and normative Bayesian modelling similar to growth charts. In our clinical cohort with MRI acquired at 3T, it can be used to identify early placental insufficiency with an AUC of 0.95. This work was also featured in the press in King's College London [Spotlight on Impact](https://www.kcl.ac.uk/news/health-of-placenta-can-be-predicted-in-30-second-mri-scan-say-researchers) (9 Aug 2021), [Healthcare in Europe](https://healthcare-in-europe.com/en/news/machine-learning-predicts-placenta-health-from-mri-scans.html) (30 Sep 2021), [the Imaging Wire](https://theimagingwire.com/news/hybrid-himss-handheld-alliance-incidental-follow-ups/) (16 Aug 2021), and [European Hospital](https://european-hospital.com/media/epaper/2/2021_3/#10) (Aug/Sept 2021).
<img src="assets/img/placenta.jpg" alt="Placental health prediction" width="100%"/>


<!-- [Machine learning predicts placenta health from MRI scans](https://healthcare-in-europe.com/en/news/machine-learning-predicts-placenta-health-from-mri-scans.html) (healthcare-in-europe.com, 30 Sep 2021), [the Imaging Wire](https://theimagingwire.com/news/hybrid-himss-handheld-alliance-incidental-follow-ups/) (16 Aug 2021), and [Detecting early signs of preeclampsia](https://european-hospital.com/media/epaper/2/2021_3/#10) (European Hospital, Aug/Sept 2021). -->


