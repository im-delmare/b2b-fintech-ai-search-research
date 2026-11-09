# Initial findings

**Research ID:** B2B-FINTECH-AI-SEARCH-2026-11-09  
**Analysis date:** 9 November 2026  
**Status:** Exploratory descriptive analysis

## 1. Sample at a glance

The dataset contains 30 captured responses: 10 queries answered once each by ChatGPT, Gemini and Perplexity.

The 10 queries span four stages of a B2B fintech buying journey:

| Buyer-journey stage | Queries | Questions covered |
| --- | --- | --- |
| Problem recognition and diagnosis | Q01–Q02 | Cross-border payout failures; KYB onboarding failures |
| Solution discovery and technical fit | Q03–Q06 | Marketplace payment APIs; business banking APIs; SEPA Instant payouts; multi-currency payouts |
| Regulatory due diligence | Q07–Q08 | EMI authorisation; licensing for embedded payments |
| Commercial evaluation | Q09–Q10 | Processing fees at 50,000 monthly transactions; cross-border payment costs |

This classification is an analytical interpretation of the query wording, not a field collected from the platforms.

## 2. Provider names appearing in response text

A preliminary case-insensitive text scan found the following provider names in the captured responses:

| Provider | Responses containing the name |
| --- | ---: |
| Stripe | 16/30 |
| Adyen | 12/30 |
| Airwallex | 11/30 |
| Mollie | 10/30 |
| Swan | 8/30 |
| Wise | 8/30 |
| Modulr | 8/30 |
| Mangopay | 7/30 |
| ClearBank | 7/30 |
| Nium | 6/30 |

These are raw text-presence counts, not rankings, market shares, endorsements, citation counts or measures of provider quality. They have not yet undergone manual entity disambiguation. A provider appearing in a response does not mean the platform recommends it as the best option for every buyer.

## 3. Explicit URLs in the captured transcripts

The dataset contains 95 URL occurrences, representing 93 distinct URL strings across 70 hostnames.

| Platform | Responses with explicit URLs in transcript | URL occurrences |
| --- | ---: | ---: |
| Perplexity | 10/10 | 54 |
| ChatGPT | 6/10 | 41 |
| Gemini | 0/10 | 0 |
| **Total** | **16/30** | **95** |

The largest URL counts by query were Q04 (19), Q03 (16), Q05 (12), Q06 (10) and Q08 (9).

Important qualification: these counts describe URLs visible in the supplied text transcript. The absence of an explicit URL in a Gemini or ChatGPT transcript does not establish that the original interface displayed no citations or source cards. The transcript may not preserve every UI element. URL presence also does not establish source quality or factual accuracy.

The most frequently occurring hostnames in the captured URLs were stripe.com (5), connectpay.com (5), clear.bank (4) and paypal.com (3). These are URL occurrences, not unique citations to independently verified pages.

## 4. Platform output: what can and cannot be compared

The captured response text averages approximately 4,494 characters for Gemini, 5,804 for Perplexity and 5,725 for ChatGPT.

Perplexity included explicit URLs in all 10 captured responses. ChatGPT included explicit URLs in six. The Gemini text capture contained no explicit URLs.

These are observations about this particular transcript and sample. They should not be generalized to all product interfaces, model versions or future responses. Model versions and interface details were not recorded.

## 5. Strategic interpretation for B2B fintech GEO

The strongest editorial implication is that B2B fintech visibility should be designed around buyer questions across the evaluation journey, not only around broad category pages or generic provider comparisons.

The observed questions suggest five useful content groups:

1. **Operational problem pages:** explain failure modes, diagnostics, dependencies and remediation for payouts, reconciliation, onboarding and KYB.
2. **Technical capability pages:** specify supported payment rails, payout corridors, currencies, APIs, webhooks, limits and settlement conditions.
3. **Provider-fit and comparison pages:** explain which operating models and use cases a product supports, and where it is not a fit.
4. **Regulatory and licensing explanations:** identify the legal entity, regulator, authorisation, jurisdictions and division of responsibilities. Regulatory statements need current primary-source verification.
5. **Commercial evaluation resources:** explain pricing components, FX spreads, transaction bands, intermediary charges, settlement costs and the information needed for a realistic quote.

A page intended to support a qualified B2B enquiry should help a buyer establish fit before contacting sales. Useful qualification details may include geography, transaction volumes, payout corridors, currencies, required rails, licensing model, recipient types and integration requirements. This is a strategic recommendation inferred from the questions, not a measured finding about conversion behaviour.

## 6. What this study does not prove

The dataset does not measure:
- actual leads, sales conversations, pipeline or conversion rates;
- whether any mentioned provider received a qualified lead;
- whether GEO caused a provider to appear in an answer;
- how the platforms retrieve, rank or select information internally;
- repeatability across multiple runs;
- the factual accuracy of every generated claim or linked page.

The study supports an exploratory description of the questions and answer patterns in this sample. It does not demonstrate that GEO increases lead generation.

## 7. Recommended next research step

Before turning provider frequency into a stronger finding, manually code a subset of responses for:
- provider name and exact legal entity where stated;
- whether the provider is merely mentioned, shortlisted, recommended or ruled out;
- the use case attached to the mention;
- the reason or selection criteria given;
- whether the response links to an official provider page, regulator or third-party source;
- whether the statement requires fact-checking against a primary source.

For a future iteration, record model/version, interface, timestamp and repeated runs. To test lead-generation impact, connect content exposure and AI referral data to CRM-qualified enquiries; answer visibility alone is not a lead-generation metric.
