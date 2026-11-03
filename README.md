# EvidenceJudge: Evidence-Grounded Multi-Model Adjudication for LLM Failure Attribution

**Author:** Akshay Kumar Bolusani  
**Affiliation:** Independent Researcher  
**Status:** Research manuscript; publication pending

EvidenceJudge is an empirical research study investigating whether multiple small language models can adjudicate failures in LLM-based agent systems using supporting execution evidence.

The study examines failure attribution at two levels:

- **Agent-level attribution:** identifying the agent or component associated with a failure.
- **Step-level attribution:** identifying the execution step associated with a failure.

Rather than assuming that agreement among models establishes correctness, the study evaluates attribution performance, model disagreement, evidence use, and the limitations of automated adjudication.

## Research questions

The study investigates:

1. Whether multi-model adjudication can meet predefined criteria for agent-level and step-level failure attribution.
2. How disagreement among models affects attribution outcomes.
3. Whether evidence-grounding mechanisms are associated with more reliable judgments.
4. How evaluation conditions and ablations affect measured performance.
5. Where small-model adjudication succeeds, fails, or remains uncertain.

## Main evaluation outcome

**Overall result: NO-GO — none of the four primary evaluation cells met its predefined success criterion.**

The held-out evaluation comprised 160 traces: 108 algorithm-generated (AG) and 52 hand-crafted (HC).

| Evaluation cell | Correct | Accuracy | Predefined target | Outcome |
|---|---:|---:|---:|---|
| Agent-level, AG | 52/108 | 48.15% | 54.33% | Not met |
| Agent-level, HC | 29/52 | 55.77% | 55.17% | Not met under the criterion |
| Step-level, AG | 10/108 | 9.26% | 12.50% | Not met |
| Step-level, HC | 1/52 | 1.92% | 5.26% | Not met |

For the HC agent-level cell, the point estimate was above the target, but its confidence interval included the target; therefore it did not satisfy the predefined criterion. The step-level results were substantially weaker than the agent-level results.

These findings do **not** establish that multi-model adjudication is generally reliable, that it outperforms all alternatives, or that it can replace human investigation. The negative findings are central to the study.

## Method at a glance

The evaluation used a panel of four small language models:

- Qwen2.5-3B
- Llama-3.2-3B
- gemma-2-2b-it
- Falcon3-3B

The adjudicator was Llama-3.2-3B-Instruct (Q4_K_M), which was also a member of the panel. This overlap is a methodological limitation and should be considered when interpreting the results.

The study includes agent-level and step-level evaluations, disagreement analysis, ablations, and an independent scoring verification. It is an empirical evaluation of model judgments—not a validated autonomous debugging product.

## Limitations

Important limitations include:

- The hand-crafted held-out subset contains 52 traces, limiting precision.
- The adjudicator overlaps with the model panel.
- Step-level labels may be noisy and were not intervention-validated.
- The evaluation is GT-in only and does not establish performance in unrestricted deployment.
- No human-validation study was conducted.
- The evaluated models and context configuration are limited to the reported small-model setting.

## Data and artifact availability

This public repository is an overview of the research. It does **not** redistribute benchmark traces, trace text, labels, annotations, prompts, embeddings, or restricted derived datasets.

Third-party benchmark and data rights remain unresolved for some source materials. The absence of those artifacts is intentional. Do not infer permission to redistribute third-party data or derived artifacts from the presence of this repository.

The repository does not claim to be a self-contained reproducibility package. Reproduction of gold-label scoring requires access to materials that are not included here.

## Publication

**Manuscript:** *EvidenceJudge: Evidence-Grounded Multi-Model Adjudication for LLM Failure Attribution*  
**Publication status:** Pending  
**DOI:** Not yet assigned

The manuscript's publication status should be checked separately; this repository does not imply acceptance, peer review, or publication.

## Author

**Akshay Kumar Bolusani** is an independent researcher and software engineer working at the intersection of artificial intelligence, large language models, multi-agent systems, and cybersecurity.

His research interests include LLM evaluation, evidence-grounded reasoning, AI reliability, automated failure attribution, multi-model adjudication, and trustworthy AI systems.

**Affiliation:** Independent Researcher  
**Research areas:** Artificial Intelligence · LLM Evaluation · Multi-Agent Systems · AI Reliability · Evidence-Grounded Reasoning

## Citation

If you refer to this research, cite the manuscript by its title and author. A formal publication citation and DOI will be added only if and when they are assigned.

## Repository topics

`artificial-intelligence` · `large-language-models` · `llm-evaluation` · `multi-agent-systems` · `ai-reliability` · `failure-attribution` · `evidence-grounded-ai` · `llm-agents` · `automated-adjudication` · `trustworthy-ai` · `machine-learning` · `research`
