---
# Leave the homepage title empty to use the site title
title: ''
summary: 'Pronob Sarker — AI researcher and PhD applicant working on agentic AI, robust machine learning, and human-centered AI systems.'
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/cv_pronob_sarker.pdf
      headings:
        about: 'Research Profile'
        education: 'Education'
        interests: 'Research Interests'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: lg # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

  - block: focus-areas
    content:
      title: Research Interests
      subtitle: Four connected themes — not ten buzzwords
      text: |-
        My research interests are still developing, but they share a common thread: **building AI systems that are capable, reliable, and designed to work effectively with people.**
      items:
        - name: Agentic AI
          description: Building LLM agents that reason, call tools, and act reliably in real workflows — from grounded question answering over documents to personalized assistants with structured tool execution.
          icon: hero/cpu-chip
          gradient: from-indigo-500 to-blue-600
          status: active
          topics:
            - LLM Agents
            - Tool Use
            - Retrieval-Augmented Generation
            - Multi-Agent Systems
        - name: Robust and Trustworthy ML
          description: Asking whether models actually work where it matters — comparative evaluation, misclassification analysis, and understanding generalization and deployment trade-offs.
          icon: hero/shield-check
          gradient: from-teal-500 to-emerald-600
          status: active
          topics:
            - Model Evaluation
            - Robustness
            - Reliability
            - Generalization
        - name: Human-Centered AI
          description: Designing AI that works effectively with people — decision-support systems, conversational interfaces, and technology that expands access to knowledge and opportunity.
          icon: hero/users
          gradient: from-sky-500 to-cyan-600
          status: active
          topics:
            - Human–AI Interaction
            - Decision Support
            - Conversational AI
            - AI for Social Good
        - name: Foundations — Reasoning, Search, and Optimization
          description: The formal backbone of my work — graph theory, combinatorial search, and optimization as tools for understanding structure in complex systems.
          icon: hero/variable
          gradient: from-violet-500 to-purple-600
          status: active
          topics:
            - Graph Theory
            - Combinatorial Optimization
            - Stochastic Search
            - Discrete Mathematics
    design:
      layout: cards

  - block: collection
    id: research
    content:
      title: Featured Research
      text: |-
        Research experiences where I investigated a question end-to-end — from problem formulation to empirical findings.
      filters:
        folders:
          - projects
        featured_only: true
    design:
      view: card
      columns: 2

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: |-
        Systems I have built — emphasizing the problem, the approach, and what I learned.
      filters:
        folders:
          - projects
        exclude_featured: true
    design:
      view: card
      columns: 2

  - block: markdown
    content:
      title: 'Currently'
      subtitle: ''
      text: |-
        I am a Computer Science senior at Gettysburg College, graduating in **December 2026**, and I am applying to PhD programs in Artificial Intelligence. I am looking for a research group where I can deepen my work on agentic AI and trustworthy ML — and where building real systems is part of doing good science.

        If my interests overlap with your lab, [I would love to talk](/contact/).
    design:
      columns: '1'

  - block: resume-awards
    content:
      title: Awards & Honors
      username: me
    design:
      columns: 2

  - block: cta-card
    content:
      title: Interested in collaborating?
      text: |-
        I am always happy to discuss research, PhD opportunities, or AI projects — especially at the intersection of agents, reliability, and human-centered systems.
      button:
        text: Get in touch
        url: /contact/
    design:
      card:
        css_class: 'bg-gradient-to-r from-indigo-600 to-blue-600 dark:from-indigo-800 dark:to-blue-800'
---
