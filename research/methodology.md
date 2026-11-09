# Research methodology

## Study

**Title:** B2B fintech questions in AI search  
**Research ID:** B2B-FINTECH-AI-SEARCH-2026-11-09  
**Research date:** 9 November 2026  
**Research type:** Exploratory snapshot

## Objective

To document how three AI answer engines respond to practical questions relevant to B2B fintech buyers, preserving the captured answers as traceable research records.

The study examines the information presented in responses, provider and entity mentions, cited sources where visible in the captured output, and the kinds of information that may be relevant to a buyer evaluating fintech infrastructure.

## Research question

How do ChatGPT, Gemini and Perplexity answer practical B2B fintech questions about payment infrastructure, embedded finance, banking APIs, compliance and pricing?

## Platforms and sample

- ChatGPT
- Gemini
- Perplexity

The source transcript contains **10 distinct queries** and **30 captured responses**: one response from each platform for each query. The dataset therefore contains one recorded run per platform-query combination.

The questions cover:
1. Cross-border B2B payout failures.
2. KYB onboarding failures in embedded finance.
3. Payment APIs for EU marketplaces.
4. Business banking APIs for European fintech startups.
5. SEPA Instant payouts via API.
6. Multi-currency payouts to 50 countries.
7. EMI-licensed payment providers in the EU.
8. Licensing requirements for embedded payments in the EU.
9. Payment processor fees at 50,000 monthly B2B transactions.
10. Cross-border B2B payment fee comparisons.

The exact query text and captured answers are preserved in [the observations dataset](../data/observations.jsonl).

## Collection and recording

The responses were supplied in a transcript dated 9 November 2026. The dataset preserves the response text as captured in that source transcript. URLs explicitly present in each response are recorded in the `cited_sources` field.

No model version or interface identifier was recorded in the source material. These fields are therefore null rather than inferred. The dataset records one captured response for each platform-query pair; it does not imply repeated trials or statistical sampling.

## Data structure

Each JSONL record includes:
- `test_id`: unique identifier for the platform-query observation.
- `research_id`: identifier for this study.
- `test_date`: date recorded in the source transcript.
- `platform`: ChatGPT, Gemini or Perplexity.
- `model_version`: null where not recorded.
- `interface`: null where not recorded.
- `query_id` and `exact_query`: the question and its identifier.
- `run_number`: 1, representing the single captured response in this dataset.
- `raw_response`: captured response text.
- `mentioned_entities`: empty because entities have not yet been separately coded.
- `cited_sources`: URLs explicitly present in the captured response.
- `own_domain_cited` and `citation_position`: null because this was not a brand-domain citation test.
- `observations`: null pending a separate analytical coding pass.
- `limitations`: missing metadata and coding caveats.

## Limitations

This is an exploratory snapshot, not a controlled benchmark.

- The sample contains 10 selected questions, not a representative sample of all B2B fintech buyer searches.
- Only one captured response is available for each platform-query combination. The study cannot measure response consistency or variability across repeated runs.
- Model versions and interface details were not recorded, so platform-level comparisons should not be interpreted as controlled model comparisons.
- AI-generated answers can change over time and may vary with query wording, account context, product settings, retrieval conditions and other factors not controlled here.
- The presence of a provider or URL in an answer is an observation. It does not establish endorsement, accuracy, commercial preference, buyer intent or lead generation.
- URLs are transcribed from the supplied response text; this dataset does not independently verify every cited page or claim.
- Mentioned entities and analytical observations have not yet been independently coded. Empty or null fields should not be interpreted as absence.

## Interpretation

The records can support qualitative analysis of how these systems frame B2B fintech questions and which providers or sources appear in the captured answers. They cannot establish how the platforms work internally, which providers receive qualified leads, whether GEO increases conversions, or whether the same answers will recur.

Keep three layers distinct in any analysis:
1. Original platform output, preserved in `raw_response`.
2. Structured fields extracted from that output.
3. Researcher interpretation, which should be documented separately and clearly labelled.

## Reproducibility

This repository documents the captured sample and its limitations. It does not claim that the original platform sessions can be reproduced exactly. Future updates should record the exact interface, model/version information when available, timestamps, repeated runs and any changes to query wording.
