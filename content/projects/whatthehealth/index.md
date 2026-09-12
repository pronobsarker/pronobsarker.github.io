---
title: "WhatTheHealth — AI-Powered Healthcare Decision Support"
date: '2024-10-01'
summary: "An end-to-end AI application combining NLP and supervised machine learning to predict health risk from free-text symptom descriptions. Built at HackUMBC 2024."
tags:
  - Human-Centered AI
  - NLP
  - Machine Learning
  - Healthcare
featured: false
# TODO: add code repository link
---

## Overview

WhatTheHealth is an AI-powered healthcare decision-support system built at **HackUMBC 2024**. It takes free-text symptom descriptions — the way real people actually describe how they feel — and produces risk predictions to help users make more informed decisions about seeking care.

## Motivation

Healthcare is a domain where AI must be both capable *and* trustworthy: predictions inform real decisions about real people. I was interested in the full problem — not just training a classifier, but bridging the gap between messy human language and structured prediction, and delivering it through an interface people can actually use.

## Approach

- **NLP feature extraction:** a spaCy pipeline converts unstructured symptom descriptions into structured features, handling the noise and variability of natural language.
- **Supervised risk prediction:** machine-learning models trained on curated medical datasets map the extracted features to risk estimates.
- **Full-stack delivery:** Python inference services are integrated with a Next.js frontend through REST APIs, with voice-to-text input so users can describe symptoms by speaking.

## My Contribution

I built the NLP pipeline (spaCy-based feature extraction from unstructured text), trained the supervised models on curated medical datasets, and wired the Python inference services into the Next.js frontend via REST APIs, including the voice-to-text flow.

## Results

A complete, working decision-support application: speak or type symptoms, get a structured risk assessment. The project sharpened my interest in **human-centered AI** — systems where model quality, interface design, and user trust have to be solved together.

## Technologies

Python · spaCy · scikit-learn · Next.js · REST APIs
