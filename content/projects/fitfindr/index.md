---
title: "FitFindr — AI Agent with Tool Use"
date: '2026-03-01'
summary: "An LLM-powered agent that dynamically selects and executes tools to generate personalized responses, with a structured tool-calling loop and an interactive interface."
tags:
  - Agentic AI
  - Large Language Models
  - Tool Use
featured: false
links:
  - type: code
    url: https://github.com/pronobsarker/ai201-project2-fitfindr-starter
---

## Overview

FitFindr is an AI-agent application built around **LLM function calling**: instead of answering from parametric knowledge alone, the agent dynamically selects tools, executes them in a structured loop, and composes personalized responses from the results.

## Motivation

Language models become far more useful when they can *act* — look things up, run computations, and gather context before responding. I wanted to understand the mechanics of agentic behavior first-hand: how does an LLM decide which tool to call, how should tool outputs feed back into reasoning, and where does the loop break down?

## Approach

- **Tool-calling loop:** the LLM receives a registry of available tools, selects among them based on the user's request, and iterates — calling tools, observing outputs, and refining its plan.
- **Structured tool execution:** tool calls are validated and executed through a consistent interface, keeping the agent's actions predictable and debuggable.
- **Interactive interface:** a Gradio front end exposes the agent's reasoning and tool activity, making the otherwise opaque loop inspectable.

## My Contribution

I designed and built the full application: the tool registry and execution layer, the agent's reasoning loop over LLM function-calling, and the interactive Gradio interface for agent-based workflows.

## Results

A working agent that dynamically selects tools per request and produces personalized, tool-grounded responses — a concrete, hands-on foundation for my broader interest in agentic AI systems.

## Technologies

Python · LLM function calling · Gradio
