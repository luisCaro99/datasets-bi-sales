# HelixCore — Evaluator Notes (Do not send to candidate)

This file documents some of the patterns intentionally embedded in the synthetic dataset.

## Hidden patterns intentionally embedded

### 1. The funnel has a “stage inflation” problem
`Working` is often driven by `bot` or `system` activity, not necessarily by meaningful human progression.
Strong candidates should question whether that stage belongs in the core executive funnel.

### 2. Contactability is overstated if you only count attempts
There is a meaningful gap between:
- total attempts
- attempts in local business hours
- actual connected calls

The dataset rewards candidates who normalize to local time and define “true contactability” more carefully.

### 3. There is a low-quality phone cluster
Mexico + AccountantFirm + Webinar leads have unusually poor phone quality.
This is not directly exposed in the candidate-facing tables and should be inferred from outcomes.

### 4. The March discount initiative improves gross conversion, but quality is mixed
The experiment can appear positive if evaluated on booked / closed revenue only.
However, quality deteriorates especially in discounted SMB cohorts and certain country-channel combinations.
Strong candidates should test downstream quality through `subscriptions.csv`.

### 5. AI bot impact is heterogeneous
Periskope-A tends to help after-hours SMB motion more than Periskope-B.
Periskope-B underperforms for accountant firms in Mexico and Dominican Republic, especially due to handoff delays.

### 6. Product signals matter
Higher `pql_score` and onboarding completion genuinely improve progression probability.
Strong candidates may combine product and sales signals instead of analyzing them in isolation.

### 7. KAM sizing should not be based on account count alone
Partner portfolios are intentionally unbalanced.
The best answer usually uses a weighted concept such as:
- managed client companies
- managed MRR
- support load
- or a blended workload score

### 8. Activity volume is not the same as productivity
Candidates who only count calls / touches may miss efficiency and quality.
Better answers connect activity data, capacity data and funnel outcomes.

## What a strong answer usually does

- Defines two funnel views:
  - executive funnel
  - operating funnel
- Redefines contactability with timing and outcome logic
- Evaluates the March discount push using revenue quality, not just wins
- Segments AI effect by motion, geography and use case
- Proposes weighted KAM coverage instead of raw account count
- Separates “interesting dashboard” from “decision-ready dashboard”