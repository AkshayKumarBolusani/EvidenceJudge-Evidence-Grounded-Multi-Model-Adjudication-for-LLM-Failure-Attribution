# EvidenceJudge: Evidence-Grounded Multi-Model Adjudication for LLM Failure Attribution

## Overview

EvidenceJudge is a research project investigating whether multiple small language models can reliably adjudicate failures in LLM-based agent systems using supporting execution evidence.

The framework studies how language models attribute failures at two levels:

- **Agent-level attribution:** Identifying which agent or component is responsible for a failure.
- **Step-level attribution:** Identifying the specific execution step associated with the failure.

Rather than relying on a single model's judgment, EvidenceJudge uses a multi-model evaluation and adjudication process to examine disagreements, evidence use, and consistency across different language models.

## Research Purpose

The central objective is to evaluate the reliability and limitations of automated, evidence-grounded failure attribution.

The research investigates:

- Whether multi-model adjudication improves failure attribution.
- How model disagreements affect agent-level and step-level predictions.
- Whether evidence-grounding mechanisms produce more reliable judgments.
- How different evaluation conditions and ablations influence outcomes.
- Where automated adjudication succeeds, fails, or remains uncertain.

## Research Findings

The evaluation highlights an important distinction: reasonable agent-level attribution does not necessarily translate into reliable step-level attribution.

The experiments also identify limitations in the reliability of small-model adjudication, particularly when identifying the precise execution step responsible for a failure.

Importantly, the research reports negative as well as positive findings rather than presenting multi-model adjudication as an inherently reliable solution.

## Research Scope

EvidenceJudge is an empirical research project focused on LLM evaluation, failure attribution, evidence-grounded reasoning, and reproducible assessment of automated judgments.

It is not presented as a production-ready autonomous debugging system or as a replacement for human investigation.

## Publication

Research manuscript:

**EvidenceJudge: Evidence-Grounded Multi-Model Adjudication for LLM Failure Attribution**

Status: Research manuscript; publication pending.

## Author

**Akshay Kumar Bolusani** is an independent researcher and software engineer working at the intersection of Artificial Intelligence, Large Language Models (LLMs), multi-agent systems, and cybersecurity.

His research interests include LLM evaluation, evidence-grounded reasoning, AI reliability, automated failure attribution, multi-model adjudication, and trustworthy AI systems.

He is the author of *EvidenceJudge: Evidence-Grounded Multi-Model Adjudication for LLM Failure Attribution*, an empirical research project investigating the reliability and limitations of multi-model approaches to attributing failures in LLM-based agent systems.

His broader technical interests include machine learning, deep learning, retrieval-augmented generation (RAG), agentic AI, and applied AI research.

**Affiliation:** Independent Researcher  
**Research areas:** Artificial Intelligence, LLM Evaluation, Multi-Agent Systems, AI Reliability, Evidence-Grounded Reasoning.
