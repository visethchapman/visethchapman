## Hi, I'm Viseth 👋

Data scientist working across the applied-ML stack: LLM systems, classical ML,
and experimentation.

The four projects below run on an open stack (Postgres, HuggingFace, PyTorch)
and are each reproducible from their README.

### Projects

**[energy-text2sql](https://github.com/visethchapman/energy-text2sql)** — LLM orchestration
Natural-language-to-SQL over US electricity-grid data. A 4-node LangGraph
pipeline (plan → synthesize → execute → summarize) with vector-routed schema
retrieval (pgvector + HuggingFace embeddings) and an SSE-streaming FastAPI UI.
Scores 12/12 on a result-equivalence eval harness.
`LangGraph · Claude · RAG · pgvector · FastAPI`

**[ercot-demand-forecast](https://github.com/visethchapman/ercot-demand-forecast)** — time-series ML
24-hour-ahead electricity demand forecasting: naive persistence vs LightGBM
with engineered features vs Amazon's Chronos-Bolt foundation model. The
zero-shot foundation model won (4.33% MAPE) with no feature engineering, plus
a calibration analysis of the prediction intervals.
`LightGBM · Chronos-Bolt · quantile regression · calibration`

**[text2sql-finetune](https://github.com/visethchapman/text2sql-finetune)** — LLM training
LoRA fine-tune of Qwen2.5-Coder-1.5B on ERCOT text-to-SQL, trained on Kaggle
and shipped to the [HuggingFace Hub](https://huggingface.co/visethchapman/ercot-text2sql-qwen-1.5b-lora).
Tripled the base model's eval score (2/12 → 6/12) at $0/query local inference.
Full pipeline: synthetic data generation → dedupe → SFT → eval.
`LoRA · PEFT · TRL · transformers · Kaggle GPU`

**[ab-testing-cuped](https://github.com/visethchapman/ab-testing-cuped)** — experimentation
A complete A/B test on MovieLens 25M with the techniques real experimentation
platforms use: CUPED variance reduction (30% tighter CI = 2× effective sample),
simulation-based power analysis, guardrail metrics with multiple-testing
correction, and sequential testing.
`CUPED · power analysis · guardrails · sequential testing`

### Stack

`Python · PyTorch · HuggingFace · LightGBM · statsmodels · pandas · Postgres · pgvector · FastAPI · Docker`

<sub>Open to applied-ML / data-science roles.</sub>
