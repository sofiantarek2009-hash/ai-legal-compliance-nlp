# AI and Compliance Systems (Public Showcase)

> **Public Runnable Proof Gist:** [**Execute & Inspect Live Proof Gist ->**](https://gist.github.com/sofiantarek2009-hash/66bcce759395d549fa402d0ee4411cd8)  
> **Visibility Policy:** Client production weights, contracts, and raw medical/financial datasets stay **private** under NDA. The linked public Gist publishes zero-dependency reproducible Python modules for each capability below.

---

## Run the Reproducible Proof Locally (Zero Dependencies)

Requires **Python 3.9+ standard library only**:

```bash
gh gist clone 66bcce759395d549fa402d0ee4411cd8 legal-compliance-nlp-proof
cd legal-compliance-nlp-proof
python3 legal_compliance_nlp_pipeline.py --test
```

## Verified Public Proof Suite + Private Client Impact

### 1. AI Legal & Compliance NLP Pipeline
- **Implementation in Public Gist:** Sublinear TF-IDF (word unigrams/bigrams + character 5-grams) trained with L2-regularized Multinomial Softmax SGD + deterministic statutory red-flag character-span extractor.
- **Verified Gist Benchmark:** **`87.50%` Accuracy** and **`0.8615` Macro-F1** across strict Stratified 5-Fold CV (`72` sanitized synthetic MSA/DPA clauses, `6` risk classes, `0` train/test fold overlap) + **`3/3` exact statutory red-flag character spans matched**.
- **Production Client Impact (Private Repo):** Deployed for business clients, **cutting manual review time by ~50% at human-level accuracy**.

### 2. Custom Client AI Models (Biotech & Financial Forecasting)
- **Biotech — Genetic Risk Pattern QC & PRS (Public Gist):** Exact Pearson `chi^2` Hardy-Weinberg Equilibrium gate cleanly rejects corrupted callset `rs999_CORRUPTED` (`(90, 2, 8)`, `p < 1e-4`) while scoring passing alleles into calibrated Bayesian posterior log-odds risk (**`26.89%`**).
- **Financial Forecasting — Walk-Forward Holt-Winters (Public Gist):** Damped double exponential smoothing over `8`-period holdout achieves **`RMSE = 1.21` (`MAPE = 0.47%`)** vs. seasonal naive baseline **`RMSE = 23.55` (`MAPE = 10.10%`)**.

## Proof Bundles & Related Systems

- **Alpha Genesis (EGX Trading Engine):** [Showcase Repo](https://github.com/sofiantarek2009-hash/alpha-genesis-overview) · [Runnable Proof Gist](https://gist.github.com/sofiantarek2009-hash/a342d001d6ee81478a3e33519afaed29)
- **Polymarket Statistical Models:** [Showcase Repo](https://github.com/sofiantarek2009-hash/polymarket-prediction-models) · [Runnable Proof Gist](https://gist.github.com/sofiantarek2009-hash/9b62a1b39b175a7574452c393e16f71f)
- **AI Legal NLP, Biotech & Forecasting:** [Showcase Repo](https://github.com/sofiantarek2009-hash/ai-legal-compliance-nlp) · [Runnable Proof Gist](https://gist.github.com/sofiantarek2009-hash/66bcce759395d549fa402d0ee4411cd8)
- **Autonomous Fixed-Wing UAV (SIL):** [Showcase Repo](https://github.com/sofiantarek2009-hash/autonomous-fixed-wing-uav) · [Runnable Proof Gist](https://gist.github.com/sofiantarek2009-hash/5a2fe80e4b6eb7809202c54b7a337255)
- **Apodictic Public Verification Harness (10 Proof Bundles + CI):** [apodictic-verified-proofs](https://github.com/sofiantarek2009-hash/apodictic-verified-proofs)
- **Live Explorer & AI Agent Specs:** [www.apodictic.dev/proofs](https://www.apodictic.dev/proofs) · [`llms.txt`](https://www.apodictic.dev/llms.txt) · [`.well-known/agent.json`](https://www.apodictic.dev/.well-known/agent.json) · [GitHub Profile](https://github.com/sofiantarek2009-hash)
---

**Author:** Sofian Mousa · **Contact:** `sofianmousa@apodictic.dev`
