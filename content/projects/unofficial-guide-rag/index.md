---
title: "Unofficial Guide — Retrieval-Augmented Generation System"
date: '2026-02-01'
summary: "A grounded question-answering system over institutional documents: PDF processing, dense retrieval with ChromaDB, and LLM inference constrained to retrieved context."
tags:
  - Retrieval-Augmented Generation
  - Large Language Models
  - NLP
featured: false
links:
  - type: code
    url: https://github.com/pronobsarker/ai201-project1-unofficial-guide-starter
---

## Overview

Unofficial Guide is a **retrieval-augmented generation (RAG)** application that answers questions over institutional documents and guides. Rather than relying on an LLM's parametric memory, every answer is grounded in retrieved passages from the organization's own documents.

## Motivation

LLMs hallucinate, and institutional knowledge — policies, guides, handbooks — is exactly the kind of long-tail content they get wrong. Grounding generation in retrieved context is one of the most practical paths toward *reliable* language-model systems, and I wanted to build the full pipeline myself to understand where it succeeds and where it fails.

## Approach

- **Document processing:** institutional PDFs are parsed and chunked with `pdfplumber`, preserving usable text structure.
- **Dense retrieval:** chunks are embedded with sentence-transformer models and indexed in ChromaDB for semantic search.
- **Grounded generation:** at query time, the top retrieved passages are fed to the LLM as context, and answers are generated *from* that context.
- **Interactive interface:** a Gradio UI lets users ask questions and inspect the grounded answers.

## My Contribution

I built the end-to-end system: the document-processing pipeline, the embedding and retrieval layer (sentence-transformers + ChromaDB), the LLM inference integration, and the interactive Gradio interface.

## Results

A working RAG system that answers questions over real institutional documents with answers traceable to retrieved sources — a small but complete exercise in making LLM outputs more trustworthy.

## Technologies

Python · pdfplumber · sentence-transformers · ChromaDB · Gradio
