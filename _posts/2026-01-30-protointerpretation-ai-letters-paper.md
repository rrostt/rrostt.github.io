---
layout: post
title: "Proto-interpretation in ACM AI Letters"
date: 2026-01-30
author: Mattias Rost
---

I’m happy to share that my paper **“Proto-Interpretation: The Temporality of Large Language Model Inference”** is now available as *Just Accepted* in **ACM AI Letters**. The paper can be accessed via the [ACM Digital Library](https://dl.acm.org/doi/10.1145/3789666).

Large language models are often described as next-token predictors. This characterization accurately reflects their training objective, but says surprisingly little about what actually happens during inference. In practice, we tend to treat an LLM’s final output as a static artifact: a sentence, an answer, a solution. This perspective, however, obscures an important dimension of model behavior.

In this paper, I propose a different lens: **proto-interpretation** — a way of understanding LLM inference as a *temporally unfolding interpretive process*, rather than as a single act of prediction.

## So what is proto-interpretation?

Proto-interpretation foregrounds the **temporal structure** of inference. During generation, an LLM does not move directly from input to output. Instead:

- Multiple possible continuations are implicitly available early in generation.
- These alternatives coexist and compete as probability mass is redistributed across successive steps.
- Each generated token constitutes a *partial commitment*, progressively constraining future possibilities.

In this way, interpretive structure emerges through time, as some potential continuations are reinforced while others are pruned away. Seen this way, an LLM’s output is not the execution of a pre-existing interpretation, but the end point of a temporally structured selection process.

## Why this matters

Viewing inference through proto-interpretation has several implications:

- **Evaluation:** Final outputs are only snapshots of a deeper process. What matters is not just *what* was produced, but *how* the model arrived there.
- **Competence and meaning:** Model behavior should not be read as evidence of stored understanding or internal semantic representations, but as the outcome of an unfolding probabilistic process.
- **Theory and philosophy of AI:** Proto-interpretation offers a way to talk about meaning-related phenomena in LLMs without attributing agency, intention, or semantic understanding, while still taking inference dynamics seriously.

The paper illustrates this perspective using a minimal ambiguity case, designed to isolate the temporal dynamics through which commitment emerges during inference.

## Relation to broader work

Proto-interpretation connects to ongoing conceptual work on the nature of LLM inference and interpretation, and more broadly to research on [LLM-mediated computing](https://interactions.acm.org/archive/view/september-october-2025/reclaiming-the-computer-through-llm-mediated-computing). It complements - but is distinct from - accounts that frame LLMs primarily in terms of representations, internal states, or autonomous reasoning. Instead, it emphasizes **process over product**, and **temporal unfolding over static explanation**.

I see this paper as a conceptual building block rather than a conclusion—one that helps clarify what it means to take the temporal dynamics of LLM inference seriously, both technically and philosophically.
