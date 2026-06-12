# CyberBench-LLM 2026 v1.0

## Benchmarking LLMs on Turkish Cybersecurity Audit and Cybersecurity Knowledge

This project evaluates modern Large Language Models (LLMs) using Turkish-language cybersecurity and audit-oriented benchmark datasets.

The objective is to measure how effectively frontier and open-source models understand, reason about, and answer professional cybersecurity and audit questions in Turkish.

## Evaluation Scope

The benchmark focuses on:

* Cybersecurity Audit
* Information Security Governance
* Risk Management
* Security Operations
* Incident Response
* Security Controls
* Cybersecurity Concepts
* Scenario-Based Security Decision Making

### Total Evaluation Size

| Dataset             | Questions |
| ------------------- | --------: |
| Cybersecurity Audit |       609 |
| Cybersecurity       |       173 |
| Total               |       782 |

---

# Methodology

* All models were evaluated using the same Turkish-language question sets.

* Cybersecurity Audit benchmark contains 609 multiple-choice questions.

* Cybersecurity benchmark contains 173 multiple-choice questions.

* Each model received the same questions.

* Answers were compared against predefined answer keys.

* Accuracy was calculated as:

  Correct Answers / Total Questions

* Results were scored automatically.

* No manual corrections were applied.

---

# Models Evaluated

## Open Models

| Model                           | Parameters |
| ------------------------------- | ---------: |
| Gemma 4 31B IT                  |        31B |
| Qwen 3.6                        |       ~32B |
| DeepSeek-R1-Distill-Qwen-32B    |        32B |
| Mistral Small 3.2 Instruct 2506 |        24B |
| GPT-OSS                         |        20B |

## Closed / Commercial Models

| Model        |
| ------------ |
| ChatGPT 5.5  |
| Gemini Flash |
| Claude Sonnet 4.6       |
| Grok 4       |
| Perplexity   |

---

# Cybersecurity Audit Benchmark Results (609 Questions)

| Rank | Model               | Correct | Total |   Accuracy |
| ---- | ------------------- | ------: | ----: | ---------: |
| 🥇   | Claude Sonnet 4.6   |     537 |   609 | **88.18%** |
| 🥈   | ChatGPT 5.5         |     501 |   609 | **82.27%** |
| 🥉   | Gemma 4 31B         |     494 |   609 | **81.12%** |
| 4    | Gemini Flash        |     469 |   609 |     77.01% |
| 5    | Qwen 3.6            |     463 |   609 |     76.03% |
| 6    | Perplexity          |     438 |   609 |     71.92% |
| 7    | Grok 4              |     434 |   609 |     71.26% |
| 8    | DeepSeek-R1 Distill |     417 |   609 |     68.47% |
| 9    | Mistral Small 3.2   |     385 |   609 |     63.22% |
| 10   | GPT-OSS             |     183 |   609 |     30.05% |

---

# Cybersecurity Benchmark Results (173 Questions)

| Rank | Model               | Correct | Total |   Accuracy |
| ---- | ------------------- | ------: | ----: | ---------: |
| 🥇   | Claude Sonnet 4.6   |     163 |   173 | **94.22%** |
| 🥈   | ChatGPT 5.5         |     160 |   173 | **92.49%** |
| 🥉   | Gemma 4 31B         |     155 |   173 | **89.60%** |
| 4    | Gemini Flash        |     150 |   173 |     86.71% |
| 5    | Qwen 3.6            |     149 |   173 |     86.13% |
| 6    | Grok 4              |     148 |   173 |     85.55% |
| 7    | DeepSeek-R1 Distill |     142 |   173 |     82.08% |
| 8    | Perplexity          |     139 |   173 |     80.35% |
| 9    | Mistral Small 3.2   |     133 |   173 |     76.88% |
| 10   | GPT-OSS             |      61 |   173 |     35.26% |

---

# Overall Results (782 Questions)

| Rank | Model               | Correct | Total |   Accuracy |
| ---- | ------------------- | ------: | ----: | ---------: |
| 🥇   | Claude Sonnet4.6    |     700 |   782 | **89.51%** |
| 🥈   | ChatGPT 5.5         |     661 |   782 | **84.53%** |
| 🥉   | Gemma 4 31B         |     649 |   782 | **82.99%** |
| 4    | Gemini Flash        |     619 |   782 |     79.16% |
| 5    | Qwen 3.6            |     612 |   782 |     78.26% |
| 6    | Grok 4              |     582 |   782 |     74.42% |
| 7    | Perplexity          |     577 |   782 |     73.79% |
| 8    | DeepSeek-R1 Distill |     559 |   782 |     71.48% |
| 9    | Mistral Small 3.2   |     518 |   782 |     66.24% |
| 10   | GPT-OSS             |     244 |   782 |     31.20% |

---

# Performance Analysis

| Model               | Avg Tokens / Question | Generation TPS | Avg Latency |
| ------------------- | --------------------: | -------------: | ----------: |
| Gemma 4 31B         |                   153 |            2.3 |         ~0s |
| Qwen 3.6            |                   170 |           14.0 |         ~0s |
| Mistral Small 3.2   |                   171 |            3.3 |       0.61s |
| DeepSeek-R1 Distill |                   663 |           3.83 |         ~0s |
| GPT-OSS             |                   482 |           10.4 |      20–25s |

---

# Key Findings

### Highest Overall Accuracy

🥇 Claude Sonnet4.6 — 89.51%

### Strongest Commercial Model

🥇 ChatGPT 5.5 — 84.53%

### Strongest Open-Weight Model

🥇 Gemma 4 31B — 82.99%

### Best Speed-to-Accuracy Ratio

🥇 Qwen 3.6

### Most Token-Efficient Model

🥇 Gemma 4 31B

### DeepSeek Observation

DeepSeek consumed approximately four times more tokens than Gemma and Qwen while achieving lower benchmark scores.

This benchmark suggests that longer reasoning traces do not necessarily translate into better Turkish cybersecurity performance.

---

# Implications for Security Teams

The results indicate that modern LLMs can already provide meaningful assistance for:

* SOC Level-1 investigations
* Alert triage
* Security monitoring
* Incident analysis
* Audit preparation
* Control validation
* Risk assessment support
* Security awareness activities

Among the open-weight models evaluated, Gemma demonstrated the strongest balance of accuracy, efficiency, and deployability.

---

# Limitations

This benchmark measures Turkish-language performance on cybersecurity audit and cybersecurity knowledge questions.

It does not evaluate:

* Penetration testing
* Malware reverse engineering
* Coding ability
* Long-context reasoning
* Tool usage
* Agentic workflows
* Real-world SOC operations

Results should therefore be interpreted as a measure of Turkish cybersecurity knowledge and reasoning performance rather than a complete assessment of model capabilities.

---

# Conclusion

This benchmark provides a snapshot of how modern LLMs perform on Turkish cybersecurity and audit-oriented questions.

Among all evaluated models, Claude achieved the highest overall accuracy.

Among open-weight models, Gemma delivered the strongest combination of accuracy, efficiency, and operational practicality.

As LLM adoption within SOC and security teams continues to grow, Turkish-language evaluations remain an important component for organizations operating in local environments and regulatory contexts.

**Disclaimer**

This study is an independent personal research project and reflects the performance of the evaluated models at a specific point in time (June 2026).

Results may vary depending on the prompts used, model versions, system configurations, inference settings, and testing environments. As AI models evolve rapidly, future performance may differ significantly from the results presented here.

The findings should not be interpreted as investment advice, a guarantee of accuracy, or an endorsement of any particular model, vendor, or product. The benchmark is intended solely for informational and educational purposes.

Any decisions, implementations, or business activities undertaken based on these results are the sole responsibility of the reader or organization. The authors assume no liability for any direct or indirect consequences arising from the use or interpretation of this analysis.

