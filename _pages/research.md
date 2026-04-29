---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

<div class="research-intro" markdown="1">

My research centers on **misinformation**: how it is produced, why it spreads, and what happens when AI systems attempt to govern it. I move between two lines of work:

- **Misinformation dynamics** — what drives people to produce, share, and engage with false or distorted claims, and what features of misinformation, such as moral language and coalitional cues, amplify these dynamics on social media.
- **AI as a communicative actor** — how large language models intervene in information ecosystems, from fact-checking and content moderation to retrieval-augmented annotation pipelines.

Methodologically, I combine **large-scale computational text analysis** (LLM-as-judge, RAG, topic modeling), **experiments and surveys**, and **machine learning** for social inference. A secondary line of work applies these tools to **health risk communication**, particularly around adolescent and college-student well-being.

</div>

---

## I. Misinformation, Morality & AI Governance

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>When Morality Kidnaps Science</h3>
  <span class="status status-award">ICA Top Student Paper · Under Extension</span>
</div>
<p class="project-subtitle">Moral Expressions, Public Engagement, and Moral Contagion in Scientific Misinformation</p>

**Role.** First author (with Q. Qiu).

**Question.** Science is provisional, evolving, and uncertain by nature, yet public discourse demands clarity and moral resolution. What happens when scientific controversies get rewritten in moral language? Do moralized claims travel further, and at what cost to deliberation?

**Approach.** I built a Weibo corpus of 1,263 posts and 20,389 comments on GMO debates and measured moral expression using a hybrid pipeline combining the C-MFD 2.0 dictionary with Word2Vec-based cosine similarity, capturing both explicit and implicit moral cues. Deliberative quality of comment threads was scored via GPT-4o-assisted classification. The analysis integrated negative binomial regressions, linear regressions, and zero-inflated Poisson models.

**Findings.** A dual effect: moralized misinformation amplifies engagement, particularly through likes, and especially when grounded in binding foundations such as authority and loyalty. But this reach comes at a cost. Moral framing triggers contagion in the comments and suppresses logical justification. Moral language is therefore not just a stylistic feature of misinformation; it is a mechanism that trades discursive scale for discursive quality, narrowing the space for reasoned engagement with science.

**Status.** Top Student Paper Award at ICA 2026 (Science Communication Division); oral presentation. Currently extending the corpus and refining a RAG-based moral coding pipeline with LLM-as-judge validation for the journal submission.

</div>

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>Reviewing the Reviewers</h3>
  <span class="status status-progress">Working Paper · Submitted to AEJMC</span>
</div>
<p class="project-subtitle">Policy Framing and Error Trade-offs in LLM-Based Content Moderation</p>

**Role.** First author (with Y. Miao).

**Question.** Content moderation is usually framed as a classification problem: how accurately can a model detect harm? But every moderation decision also enacts a governance choice, deciding whose speech is suppressed and whose harm is tolerated. When LLMs become the moderators, that choice gets quietly compressed into the prompt. Can changing the normative framing of a prompt, without touching the model, the data, or the rubric, systematically redistribute who gets over-flagged and who gets missed?

**Approach.** Using the multilingual RTP-LX benchmark, I evaluated two instruction-tuned LLMs (Llama-3-8B-Instruct and Qwen2.5-7B) across English and Chinese under three prompt regimes: control, speech-first, and security-first. Weighted Cohen's κ measured ordinal alignment with human annotations; paired Wilcoxon tests captured within-item shifts; and a removal-oriented analysis tracked false-positive and false-negative rates by harm category.

**Findings.** Two results define the contribution. First, model–human alignment is highly uneven: strong on overt categories like toxicity and insult, near-zero on context-dependent ones like bias and microaggression, the very categories most consequential for marginalized speakers. Second, policy framing systematically moves the decision boundary along a Pareto frontier: speech-first reduces false positives at the cost of more false negatives; security-first does the opposite. There is no neutral setting. LLM moderation does not classify harm; it redistributes communicative risk according to whichever governance logic is written into the prompt.

**Status.** Submitted to AEJMC; reframing for a journal venue in communication / AI ethics.

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

**Question.** Sexual victimization research typically aggregates contact and non-contact harms into a single outcome. But the digital era has generated a distinct ecology of non-contact victimization, including image-based abuse, sextortion, and platform-facilitated harassment, that may be governed by fundamentally different risk architectures. Do contact and non-contact victimization share the same predictors, or does treating them as one phenomenon obscure the very differences that prevention needs to address?

**Approach.** Using a nationally representative survey of **71,502 Chinese college students** across all 31 provinces, I trained six machine learning algorithms (lasso-regularized logistic regression, naive Bayes, decision tree, random forest, XGBoost, and k-nearest neighbors) within a social-ecological framework spanning individual, relational, community, and societal levels. SHAP main-effect analyses identified the direction and non-linear shape of each predictor's contribution; SHAP interaction analyses further decomposed non-additive combinations of top-ranked features for non-contact victimization.

**Findings.** XGBoost and random forest consistently outperformed the other algorithms, with complementary strengths in sensitivity and precision. A shared core of psychological vulnerability (loneliness, depression, suicidality) and digital exposure predicts both forms, but the architectures diverge beyond that core: clinical mental-health burden and family disruption are distinctively salient for contact victimization, while sex, region, and platform-use patterns matter more for non-contact victimization. SHAP interaction analyses reveal that loneliness and heavy online self-media use combine multiplicatively rather than additively, and, most strikingly, that **male students who are heavy digital-media users face the highest predicted risk of non-contact victimization**, a finding that challenges the dominant female-victim framing and mandates gender-inclusive prevention design.

**Status.** Under review at *Computers in Human Behavior*.

</div>

<div class="project-card" markdown="1">

<div class="project-header">
  <h3>Educated but Risky?</h3>
  <span class="status status-review">Under Review</span>
</div>
<p class="project-subtitle">Pornography, Sexuality Education, and Condomless Sex Among Chinese College Students</p>

**Role.** First author.

**Question.** Online pornography routinely depicts unprotected sex as normative, reaching an estimated 37.6 million underage internet users in China despite strict censorship. Yet young adults encounter this risk-normalizing content within a culture of silence: family discussion of sexuality remains restricted, and formal education is unevenly distributed. The result is a script competition. Pornography supplies one behavioral template; sexuality education, where it exists, supplies another. Which script wins, and does the answer depend on *who* is teaching?

**Approach.** Drawing on the Acquisition-Activation-Application (3AM) model, I analyzed **6,761 sexually active students** from a national survey spanning 500+ universities across all 31 provinces of mainland China. Pornography consumption and condomless sex were linked through a moderated mediation framework, with SRH knowledge as mediator and three channels of sexuality education (school, family, social) as competing moderators of both the direct and indirect pathways.

**Findings.** A suppression pattern: pornography increases sexual knowledge (which lowers risk), but a stronger direct pathway to condomless sex overwhelms the protective indirect effect. The moderating role of education depends critically on which script it equips students to deploy. School-based sexuality education **attenuates the knowledge pathway** (reducing students' reliance on pornography as a knowledge source) yet paradoxically **strengthens the direct behavioral link**, suggesting that factual knowledge alone cannot displace risk-promoting scripts. Family-based education shows a marginal buffering effect; social channels show none. The implication is that sexuality education needs to move beyond knowledge transmission toward **procedural counter-script interventions** that teach students to interrupt pornography-derived behavioral templates at the point of application.

**Status.** Under review at *Journal of Medical Internet Research*.

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

I am currently developing two extensions of this agenda: (1) a **RAG-based, context-aware annotation pipeline** for cross-cultural moral language in misinformation, and (2) a comparative study of how **prompt-level governance choices propagate** through downstream LLM moderation systems. Both are part of a longer-term research program on **AI as a communicative institution**, one that does not merely transmit information but increasingly governs it.
