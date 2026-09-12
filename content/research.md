---
title: Research
summary: "Pronob Sarker's research: agentic AI, robust machine learning, human-centered AI systems, and theoretical foundations — organized by theme rather than chronology."
date: 2026-09-11
type: page
toc: true
---

My work is organized around one question: **how do we build AI systems that are capable, reliable, and designed to work effectively with people?** Below, my experiences are grouped by research theme — each following the arc from question, to investigation, to findings, to what it motivated next.

---

## Agentic AI — LLM Systems That Act

**The question:** Language models are most useful when they can *do* things — call tools, retrieve knowledge, and carry out multi-step workflows. How do we build agents whose behavior is structured, inspectable, and reliable?

**What I built:**

- [**FitFindr**](/projects/fitfindr/) — an AI agent using LLM function calling to dynamically select tools and generate personalized responses, with structured tool execution and an interactive Gradio interface.
- [**Unofficial Guide**](/projects/unofficial-guide-rag/) — a retrieval-augmented generation system over institutional documents: `pdfplumber` processing, sentence-transformer embeddings, ChromaDB retrieval, and LLM inference grounded in retrieved context.
- **Admission chatbot** (Nextive Solutions, 2022) — a Messenger-based college admission chatbot serving 5,000+ students, automating frequently asked questions through interactive workflows.

**What I learned:** The agent loop — decide, act, observe, refine — is conceptually simple and devilishly hard to make robust. Grounding outputs in retrieved context is the most practical lever I have found for trustworthiness, and inspectability (seeing *what the agent did and why*) is as important as capability.

**What it motivates next:** I want to go deeper on agentic systems — tool-use reasoning, multi-agent coordination, and evaluation of agents in realistic workflows. This is the theme I most want to pursue in a PhD.

---

## Robust & Trustworthy ML — Do Models Actually Work?

**The question:** Aggregate metrics hide systematic failures. How do we evaluate models on the hard cases, understand where they break, and reason honestly about deployment?

**What I investigated:**

- [**Fine-grained apple image classification**](/projects/apple-classification/) (Gettysburg College & Rice Fruit Company, Spring 2025; advisors: Dr. Kim Spayd, Dr. Eatai Roth) — a comparative study of KNN, SVM, Random Forest, and ResNet-50 on Fruit-360. ResNet-50 reached macro-F1 0.99, but the real contribution was the misclassification analysis: characterizing exactly which visually similar classes confused which models, and what that implies for deployment trade-offs.
- [**WhatTheHealth**](/projects/whatthehealth/) (HackUMBC 2024) — NLP + supervised ML for health-risk prediction from free-text symptoms, where a wrong prediction has real consequences for a real person.

**What I learned:** Evaluation is a research contribution in itself. Choosing the right metrics (macro-F1 and confusion matrices, not just accuracy), analyzing failures by class, and connecting results to deployment constraints is what separates a demo from evidence.

**What it motivates next:** I am drawn to research on evaluation methodology, robustness under distribution shift, and reliability guarantees for ML systems deployed in the wild.

---

## Human-Centered AI — AI That Works With People

**The question:** The best model is useless if people cannot use it, trust it, or access it. How do we design AI systems around human needs?

**What I built and led:**

- [**WhatTheHealth**](/projects/whatthehealth/) — a healthcare decision-support system with a full interface: type or *speak* symptoms, get a structured risk assessment. Model quality, interface design, and user trust had to be solved together.
- **Admission chatbot** — conversational AI that reduced repetitive inquiries for 5,000+ students.
- **Bridging the Digital Divide** (Davis Projects for Peace, 2023) — led a $10,000-funded digital-literacy initiative serving 500+ students in Bogura, Bangladesh (plus $2,000 raised to expand it). Not an ML project — but the reason I care about who technology serves.

**What I learned:** Working with real users changes what "good" means. Latency, clarity, and trust matter as much as model quality — and the most important AI problems are often about the human on the other side of the screen.

**What it motivates next:** Human–AI interaction, human-in-the-loop systems, and AI for social good remain central to how I choose problems.

---

## Foundations — Reasoning, Search & Optimization

**The question:** Beneath the systems work sits formal structure. Can I reason precisely about complex systems — and prove it?

**What I investigated:**

- [**Firecracker & Tollbooth graphs**](/projects/graph-theory/) (Spring 2024; advisor: Prof. Nathan Shank) — defined two novel parametric graph families and proved closed-form results on domination number, Eulerian properties, diameter, and independence number. Written up as the undergraduate manuscript *"Firecrackers and Tollbooth Graphs: Properties of Novel Graph Structures"* (2024).
- [**Combinatorial puzzle generation**](/projects/game-ai-puzzles/) (Summer 2023; advisor: Prof. Todd W. Neller) — Monte Carlo sampling and stochastic local search for generating and evaluating puzzles, scaled to 1M+ solvable instances with empirical analysis of diversity and difficulty.

**What I learned:** Precise definitions and rigorous argument are habits that transfer everywhere. When I work on search, optimization, or reasoning in AI systems today, I draw on the same discipline: formalize the structure first, then establish what follows.

**What it motivates next:** A continuing appetite for the theoretical side of AI — reasoning, combinatorial optimization, and the mathematics of intelligent systems.

---

## Research Outputs

I do not yet have peer-reviewed publications. My scholarly output to date is:

- *Firecrackers and Tollbooth Graphs: Properties of Novel Graph Structures* — undergraduate research manuscript, Gettysburg College, 2024.

My code is on [GitHub](https://github.com/pronobsarker), and my full history is in my [CV](/uploads/cv_pronob_sarker.pdf).
