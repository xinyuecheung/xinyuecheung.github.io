---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

<div class="research-intro" markdown="1">

My research asks how **morality, cognition, and AI systems jointly shape the production, diffusion, and governance of (mis)information**. I move between two lines of work:

- **Misinformation & moral psychology** — why people produce, share, and engage with false or distorted claims, and how moral expression amplifies these dynamics on social media.
- **AI as a communicative actor** — how large language models intervene in information ecosystems, from fact-checking and content moderation to retrieval-augmented annotation pipelines.

Methodologically, I combine **large-scale computational text analysis (LLM-as-judge, RAG, topic modeling)**, **experiments and surveys**, and **machine learning** for social inference. A secondary line of work applies these tools to **health risk communication**, particularly around adolescent and college-student well-being.

</div>

---

## I. Misinformation, Morality & AI Governance

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>When Morality Kidnaps Science</h3>
  <span class="status status-award">ICA Top Student Paper · Under Extension</span>
</div>
<p class="project-subtitle">How Moral Expressions Drive Engagement and Moral Contagion in Scientific Misinformation</p>

**Role.** First author (with Q. Qiu).

**Question.** When science gets reframed in moral language on social media, what happens to public engagement and to the deliberative quality of the discussion that follows?

**Approach.** Drawing on Moral Foundations Theory, I built a Weibo corpus of scientific misinformation and used LLM-assisted annotation to identify moral expressions across binding and individualizing foundations. I modeled the relationship between moral content and engagement (likes, comments, reposts), and then traced **moral contagion** in the comment threads each post generated.

**Findings.** Moralized scientific misinformation activates intuitive moral responses and substantially increases engagement, especially likes. In the Chinese context, content rooted in **collectivist (binding) foundations** elicits the strongest participation. But moral framing is double-edged: it triggers moral contagion in comments, **suppresses logical deliberation**, and narrows the discursive space for rational engagement with science.

**Status.** Accepted for oral presentation at ICA 2026 (Science Communication Division, Top Student Paper Award). Currently extending the study by enlarging the corpus, refining a **RAG pipeline for context-aware moral coding**, and incorporating **LLM-as-judge** validation.

</div>

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>Reviewing the Reviewers</h3>
  <span class="status status-progress">Working Paper · Submitted to AEJMC</span>
</div>
<p class="project-subtitle">Policy Framing and Error Trade-offs in LLM-Based Content Moderation</p>

**Role.** First author (with Y. Miao).

**Question.** Content moderation is usually evaluated as a technical classification problem. But when an LLM moderates speech, it is also enacting a governance choice. Whose harms get over-flagged, and whose get missed, when we change the policy framing in a prompt?

**Approach.** Using the multilingual **RTP-LX** benchmark, I evaluated two instruction-tuned LLMs across English and Chinese under three prompt regimes — **control, speech-first, and security-first**. Model–human agreement was measured with weighted Cohen's κ, complemented by an analysis of the *direction* of errors (false positives vs. false negatives) across harm categories.

**Findings.** Moderation discrepancies are unevenly distributed across harm types: alignment is high for overt categories (e.g., toxicity) but weak for context-dependent harms (e.g., bias, microaggression). Critically, **policy framing systematically shifts the model's decision boundary** — speech-first reduces false positives, security-first reduces false negatives — effectively redistributing communicative risk across speakers and targets. LLM moderation is therefore not a neutral filter; it encodes the governance choices written into its prompts.

**Status.** Manuscript complete; submitted to AEJMC. Reframing for a journal venue in communication / AI ethics.

</div>

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>Why We Share Falsehoods</h3>
  <span class="status status-conference">ICA 2026 · Computational Methods</span>
</div>
<p class="project-subtitle">Testing a Coalitional Account of Misinformation Sharing</p>

**Role.** Second author (with Y. Miao); led the statistical analysis and difference-in-differences design.

**Question.** The dominant explanation for misinformation sharing treats it as a cognitive failure that should fade when people pay closer attention to accuracy. But what if some sharing is *functional* — a way to coordinate attention, signal allegiance to allies, and project dominance toward rivals?

**Approach.** Large-scale computational study of **~130,000 tweets from 180 Twitter users**, linking individual-level moral foundations to longitudinal sharing behavior. We used the COVID-19 period as a natural variation in **collective threat** and tested whether coalitional incentives intensified under threat.

**Findings.** **Binding moral foundations** (especially authority) positively predicted misinformation sharing, while **individualizing foundations** (especially care) predicted *less* sharing. These associations were moderated by collective threat: during the pandemic, users high in binding foundations reduced their misinformation sharing far less than others — consistent with persistent coalitional incentives. Misinformation sharing, in short, is not only an error; it can be an adaptive coalitional response.

**Status.** Accepted for ICA 2026 (Computational Methods Division). Manuscript in preparation.

</div>

---

## II. Health Risk Communication & Computational Social Science

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>When Platforms Enable Harm</h3>
  <span class="status status-review">Under Review</span>
</div>
<p class="project-subtitle">A Machine Learning Comparison of Risk Factors for Contact and Non-Contact Sexual Victimization Among Chinese College Students</p>

**Role.** Co-first author.

**Question.** Sexual victimization research typically aggregates contact and non-contact harms. Do they really share the same risk structure — or do online affordances generate a distinct set of vulnerabilities?

**Approach.** A nationally representative sample of **71,502 Chinese college students** analyzed using six machine learning algorithms grounded in a social-ecological framework. I used **SHAP** to extract interpretable, non-linear risk profiles for each victimization type.

**Findings.** XGBoost and Random Forest performed best. The two harm types share core **psychological vulnerability factors**, but **media-use affordances uniquely predict non-contact victimization**, suggesting platform features themselves shape exposure. The study contributes a reproducible ML-with-SHAP framework for studying complex, non-linear media effects in communication research.

**Status.** Under review at *Computers in Human Behavior* / *JMIR*.

</div>

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>Educated but Risky?</h3>
  <span class="status status-progress">Manuscript in Preparation</span>
</div>
<p class="project-subtitle">Pornography, Sexual Knowledge, and Condomless Sex Among Chinese College Students</p>

**Role.** First author.

**Question.** Does sexual knowledge mediate or *mask* the risk pathway from pornography to condomless sex — and do school, family, and peer-based sex education channels operate the same way?

**Approach.** Drawing on the **3AM model**, I analyzed survey data from **6,761 sexually experienced students across 500+ Chinese universities**, fitting a moderated-mediation model.

**Findings.** A **competitive mediation** pattern: pornography increases sexual knowledge (which lowers risk), but a stronger *direct* effect on condomless sex overwhelms this protective pathway. School-based sex education paradoxically **weakens** the knowledge pathway while **strengthening** the direct behavioral link; family education provides a marginal buffer; peer/social sources show no significant moderation. Implication: knowledge transmission alone is insufficient — sex education needs **procedural counter-script interventions**.

**Status.** Targeting *Health Communication* / *Journal of Adolescence*.

</div>

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>Guidance Misaligned?</h3>
  <span class="status status-published">Accepted · Mass Communication and Society</span>
</div>
<p class="project-subtitle">The Moderating Role of Perception Discrepancies in Parental Mediation Effects</p>

**Role.** Third author (with L. Chen, X. Tan); led data analysis and the Methods/Results sections.

**Question.** Parental mediation research usually relies on a single reporter. What changes when we measure the **gap between parent and child perceptions** of mediation, and treat that gap itself as a moderator?

**Approach.** Matched survey data from **494 parent–child dyads** in China; tested both *absolute* and *directional* perception discrepancies as moderators of mediation effects on content risk and learning outcomes.

**Findings.** Active mediation reduces content risk and supports cognitive development. **Absolute perception discrepancy** significantly moderates these effects — alignment matters as much as the strategy itself — while directional discrepancy does not.

**Status.** Accepted at *Mass Communication and Society* (SSCI Q1).

</div>

---

## What's Next

I am currently developing two extensions of this agenda: (1) a **RAG-based, context-aware annotation pipeline** for cross-cultural moral language in misinformation, and (2) a comparative study of how **prompt-level governance choices propagate** through downstream LLM moderation systems. Both are part of a longer-term research program on **AI as a communicative institution** — one that does not merely transmit information but increasingly governs it.

I am applying to PhD programs for Fall 2026 and am actively looking for **research assistant opportunities** that align with these themes. Please feel free to reach out at [xinyuez2@usc.edu](mailto:xinyuez2@usc.edu).
