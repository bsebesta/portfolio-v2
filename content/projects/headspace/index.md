---
slug: "headspace-voice-app"
title: Creating a Voice-First Channel for Guided Meditations
description: Building a voice UI for Headspace's massive library of guided meditations on both Amazon Alexa and Google Assistant
intro:
    client: Headspace
    company: RAIN
    sector: Mental Health
    platform: Voice UI on Amazon Alexa & Google Assistant Smart Speakers
    roles:
    - Something
    - Something
    - Something
assetPath: 'https://portfolio-v2.s3.us-west-004.backblazeb2.com/projects/headspace/'
layoutDetails:
    headerImage: thumbnail-headspace-hero.png
    #previewPartialPath: "projects/headspace/preview.html"
    #resultsPartialPath: "projects/headspace/results.html"
    #audioFileClasses:
fpgallery:
    galleryShow: true
    galleryTitle: Headspace
    galleryDesc: Guided meditations without touching your phone
    galleryThumbnail: https://bsebesta-portfolio.s3.us-west-004.backblazeb2.com/case-studies/thumbnail_headspace_1.png
    galleryClass: workgallery-headspace
weight: 4
head: |
  <style>
    :root {
      --color-accent-900: hsl(23, 87%, 30%);
      --color-accent-800: hsl(23, 80%, 41%);
      --color-accent-700: hsl(23, 72%, 48%);
      --color-accent-600: hsl(23, 83%, 54%);
      --color-accent-500: hsl(23, 90%, 57%);
      --color-accent-400: hsl(23, 90%, 61%);
      --color-accent-300: hsl(23, 88%, 66%);
      --color-accent-200: hsl(23, 87%, 76%);
      --color-accent-100: hsl(23, 85%, 87%);
      --color-accent-000: hsl(23, 33%, 99%);
      /*--color-accent-000: hsl(60, 25%, 98%);
      --color-accent-100: hsl(60, 67%, 96%);
      --color-accent-150: hsl(60, 63%, 94%);
      --color-accent-200: hsl(60, 32%, 90%);*/
      --color-bannernav-logotype: var(--color-accent-700);
      --color-bannernav-link: var(--color-accent-700);
      --color-bannernav-link-hover: var(--color-neutral-900);
      --color-bannernav-link-active: var(--color-accent-900);
      --color-bannernav-link-underline: var(--color-accent-400);
      --color-bannernav-link-underline-active: var(--color-accent-400);
    }
    main { margin-block-start: 0; }
    .casestudy__fullheader_wrapper,
    .casestudy__contactcard {
      background-color: #FFCE00;
    }
    .casestudy__fullheader_text {
      color: #473E39;
    }
  .casestudy__minorheader {
    color: var(--color-accent-800);
  }
  </style>
---

A designer I follow, Pablo Sanchez, has said that the “ultimate challenge for the current generation of interaction designers is to create a cohesive ecosystem of devices, webconnected objects and cloud services.”

Our collaboration with Headspace was a great opportunity to confront this challenge head-on. Given that meditation aims to rid the mind of distractions, and given that Headspace’s massive library of guided meditations were (mostly) a purely audible experience, we were tasked to find ways to make it easy to jump in and start meditating for anyone with a Google or Amazon smart speaker.