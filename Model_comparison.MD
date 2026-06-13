# Model Comparison: Fable 5 vs Mythos 5 vs Opus 4.8 vs Sonnet 4.6

> Executive comparison sheet for Tekravio consulting engagements, solution architecture reviews, and AI platform selection decisions.

**Last Updated:** June 2026

---

# Executive Summary

Anthropic's model lineup now spans four distinct capability tiers.

```text
Sonnet 4.6
    ↓
Opus 4.8
    ↓
Fable 5
    ↓
Mythos 5
```

The key insight is that **Fable 5 and Mythos 5 are fundamentally the same underlying Mythos-class model**, while Sonnet and Opus belong to Anthropic's traditional Claude family.

For most organizations:

* Sonnet 4.6 = best value
* Opus 4.8 = best balanced enterprise model
* Fable 5 = best available capability
* Mythos 5 = restricted-access frontier capability

## June 2026: Access Restrictions Update

As of June 13, 2026, Reuters reported that a U.S. export-control directive required Anthropic to suspend Fable 5 and Mythos 5 access for foreign nationals pending resolution. Treat launch-era availability as historical and current access as jurisdiction-dependent.

---

# Model Positioning

```text
Capability
▲
│                Mythos 5
│                   ▲
│                   │
│                Fable 5
│                   ▲
│                   │
│               Opus 4.8
│                   ▲
│                   │
│              Sonnet 4.6
└────────────────────────────► Cost
```

---

# Complete Specification Table

| Category                   | Sonnet 4.6 | Opus 4.8   | Fable 5                       | Mythos 5             |
| -------------------------- | ---------- | ---------- | ----------------------------- | -------------------- |
| Model Family               | Claude     | Claude     | Mythos-Class                  | Mythos-Class         |
| Public Availability        | Yes        | Yes        | Restricted / Limited          | No                   |
| General API Access         | Yes        | Yes        | Restricted                    | No                   |
| Context Window             | Up to 1M   | Up to 1M   | 1M                            | 1M                   |
| Maximum Output             | 64K        | 128K       | 128K                          | 128K                 |
| Vision                     | Yes        | Yes        | Yes                           | Yes                  |
| Tool Use                   | Yes        | Yes        | Yes                           | Yes                  |
| Function Calling           | Yes        | Yes        | Yes                           | Yes                  |
| Prompt Caching             | Yes        | Yes        | Yes                           | Yes                  |
| Adaptive Thinking          | No         | Partial    | Always On                     | Always On            |
| Chain of Thought Access    | No         | No         | Summarized Only               | Summarized Only      |
| Raw Reasoning Access       | No         | No         | Never                         | Never                |
| Safety Classifiers         | Standard   | Standard   | Advanced External Classifiers | Reduced Restrictions |
| Cybersecurity Restrictions | Standard   | Standard   | Yes                           | Trusted Access Only  |
| Biology Restrictions       | Standard   | Standard   | Yes                           | Trusted Access Only  |
| Distillation Restrictions  | Standard   | Standard   | Yes                           | Trusted Access Only  |
| Data Retention Requirement | Optional   | Optional   | Mandatory 30 Days             | Mandatory 30 Days    |
| Zero Data Retention        | Available  | Available  | Not Available                 | Not Available        |
| Deployment Tier            | Production | Production | Frontier                      | Frontier             |
| Trusted Access Required    | No         | No         | No*                           | Yes                  |

*Subject to current availability restrictions.

Sources: Anthropic pricing and model documentation, June 2026.

---

# Pricing Comparison

## API Pricing

| Model      | Input Tokens (Per Million) | Output Tokens (Per Million) |
| ---------- | -------------------------- | --------------------------- |
| Sonnet 4.6 | $3                         | $15                         |
| Opus 4.8   | $5                         | $25                         |
| Fable 5    | $10                        | $50                         |
| Mythos 5   | Not Publicly Available     | See note below             |

Sources: Anthropic pricing documentation and launch materials.

Note: Anthropic publicly listed Mythos Preview participant pricing at $25 per million input tokens and $125 per million output tokens after usage credits. That pricing context is for Mythos Preview, not Mythos 5, but it is the closest public benchmark for expected Glasswing-style access pricing.

---

# Relative Cost Comparison

---

# Capability Comparison

## Software Engineering

| Capability          | Sonnet 4.6 | Opus 4.8  | Fable 5          | Mythos 5         |
| ------------------- | ---------- | --------- | ---------------- | ---------------- |
| Code Generation     | Excellent  | Excellent | State of the Art | State of the Art |
| Repository Analysis | Good       | Excellent | Exceptional      | Exceptional      |
| Autonomous Coding   | Limited    | Strong    | Industry Leading | Industry Leading |
| Large Refactoring   | Good       | Excellent | Exceptional      | Exceptional      |
| Migration Planning  | Good       | Excellent | Exceptional      | Exceptional      |

Fable 5 was specifically designed for long-horizon software engineering and autonomous coding workflows.

---

## Knowledge Work

| Capability               | Sonnet 4.6 | Opus 4.8  | Fable 5     | Mythos 5    |
| ------------------------ | ---------- | --------- | ----------- | ----------- |
| Research                 | Good       | Excellent | Exceptional | Exceptional |
| Technical Writing        | Excellent  | Excellent | Exceptional | Exceptional |
| Document Analysis        | Good       | Excellent | Exceptional | Exceptional |
| Multi-Document Reasoning | Good       | Excellent | Exceptional | Exceptional |

---

## Scientific Reasoning

| Capability          | Sonnet 4.6 | Opus 4.8  | Fable 5     | Mythos 5       |
| ------------------- | ---------- | --------- | ----------- | -------------- |
| Biology             | Good       | Excellent | Restricted  | Trusted Access |
| Chemistry           | Good       | Excellent | Restricted  | Trusted Access |
| Research Assistance | Good       | Excellent | Exceptional | Exceptional    |

Fable 5 intentionally restricts some biology and chemistry workflows through classifier systems.

---

## Cybersecurity

| Capability              | Sonnet 4.6 | Opus 4.8  | Fable 5             | Mythos 5        |
| ----------------------- | ---------- | --------- | ------------------- | --------------- |
| Secure Coding           | Good       | Excellent | Exceptional         | Exceptional     |
| Vulnerability Discovery | Good       | Strong    | Restricted Publicly | Full Capability |
| Attack Chain Reasoning  | Limited    | Moderate  | Restricted          | Advanced        |
| Security Review         | Good       | Excellent | Exceptional         | Exceptional     |

Mythos 5 remains restricted because of its unusually strong cybersecurity capabilities.

---

# Safety Architecture Comparison

## Sonnet 4.6

Traditional Claude alignment approach.

```text
User
 ↓
Model
 ↓
Response
```

---

## Opus 4.8

Enhanced alignment and reasoning.

```text
User
 ↓
Model
 ↓
Response
```

---

## Fable 5

Classifier-driven architecture.

```text
User
 ↓
Safety Classifier
 ↓
Fable 5
 ↓
Fallback
 ↓
Opus 4.8
```

---

## Mythos 5

Trusted-access architecture.

```text
User
 ↓
Safety Controls
 ↓
Mythos 5
```

---

# Availability Comparison

| Platform          | Sonnet 4.6 | Opus 4.8 | Fable 5    | Mythos 5 |
| ----------------- | ---------- | -------- | ---------- | -------- |
| Claude API        | Yes        | Yes      | Restricted | No       |
| Claude.ai         | Yes        | Yes      | Restricted | No       |
| Amazon Bedrock    | Yes        | Yes      | Limited    | No       |
| Vertex AI         | Yes        | Yes      | Limited    | No       |
| Microsoft Foundry | Yes        | Yes      | Limited    | No       |
| Project Glasswing | No         | No       | No         | Yes      |

Sources: Anthropic launch documentation and partner announcements.

---

# Which Model Should a Client Choose?

| Customer Type                        | Recommended Model         |
| ------------------------------------ | ------------------------- |
| Individual Developer                 | Sonnet 4.6                |
| Startup                              | Sonnet 4.6 or Opus 4.8    |
| SaaS Company                         | Opus 4.8                  |
| Enterprise Engineering Team          | Opus 4.8                  |
| Advanced AI Research Team            | Fable 5 (if available)    |
| Cybersecurity Organization           | Mythos 5 (Trusted Access) |
| Government / Critical Infrastructure | Mythos 5 (Trusted Access) |

---

# Tekravio Recommendation

## Studio

Primary Recommendation:

**Opus 4.8**

Reason:

Best balance of capability, availability, compliance, and cost.

---

## Academy

Primary Recommendation:

**Sonnet 4.6**

Reason:

Lowest cost for high-volume educational workloads.

---

## Labs

Primary Recommendation:

**Opus 4.8**

Future Upgrade:

**Fable 5**

Reason:

Strong autonomous engineering capabilities without dependence on restricted-access models.

---

# Final Verdict

If Fable 5 and Mythos 5 were universally available, they would clearly represent the most capable tier in Anthropic's lineup. However, availability constraints, safety restrictions, and data-retention requirements currently make Opus 4.8 the most practical enterprise choice.

For most production systems today:

1. Sonnet 4.6 = best cost-performance ratio.
2. Opus 4.8 = best enterprise model.
3. Fable 5 = highest public capability (where available).
4. Mythos 5 = restricted frontier model reserved for trusted-access programs.

---

## Sources

* Anthropic Pricing Documentation
* Claude Fable 5 Launch Materials
* Claude Opus 4.8 Documentation
* Claude Sonnet 4.6 Documentation
* Project Glasswing Documentation
* Public benchmark and launch reporting (June 2026)
