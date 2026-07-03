# Anthony Rodrigues

AI engineer at [Keeper](https://github.com/Keeper-Dating). I build agent-eval systems: failure prediction, hallucination detection, RAG benchmarking.

[Resume](https://drive.google.com/file/d/1ZRjLjk-h8DamBCQ9mfD9ETSNH19p6ARv/view) · [LinkedIn](https://linkedin.com/in/anthonyrodrigues443) · [Portfolio](https://anthonyrodrigues443.github.io/portfolio/) · [anthonyrodrigues443@gmail.com](mailto:anthonyrodrigues443@gmail.com)

## Flagship work

<table>
<tr>
<td width="50%" valign="top">

### [AI-Agent-Failure-Predictor](https://github.com/anthonyrodrigues443/AI-Agent-Failure-Predictor)

Every agent-observability dashboard alerts on context usage. I built a causal simulator of 20k agent runs to test that rule: **the context>80% alert misses 84% of agent failures**. The shipped model, a 1 MB calibrated CatBoost, out-ranks zero-shot Claude Opus on the same runs (**AUPRC 0.833 vs 0.738**) at roughly 32 µs per prediction.

</td>
<td width="50%" valign="top">

### [AI-Agent-Conversation-Quality-Scorer](https://github.com/anthonyrodrigues443/AI-Agent-Conversation-Quality-Scorer)

Hallucination detection on HaluEval-QA. **A 13-feature CPU tree beats zero-shot Claude Opus 4.8, Claude Haiku 4.5 and Codex GPT-5.5** at catching ungrounded answers (**0.9808 length-matched macro-F1**, about $0.0001 per 1k messages). The twist: ablation shows it is a 1-feature model in disguise, and the one slice it cannot catch is exactly where frontier models win.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [RAG-Pipeline-Optimizer](https://github.com/anthonyrodrigues443/RAG-Pipeline-Optimizer)

Measured each standard RAG lever on BEIR corpora with a harness validated against published BM25 numbers. **All four cross-encoder rerankers tested made retrieval worse** on a strong dense first stage. The final pipeline **ties the gold-context oracle on answer correctness (0.604)** with no reranker at all.

</td>
<td width="50%" valign="top">

### [iterate](https://github.com/anthonyrodrigues443/Autonomous-ML-And-LLM-Iteration-Agent) · `pip install iterate-ai`

An autonomous agent that proposes, runs, scores and remembers ML experiments, so shipped models and prompts don't rot. **v0.1.3 on PyPI** runs the full propose-run-score-remember loop on tabular ML, with sandboxed code-gen and prompt iteration next on the roadmap.

</td>
</tr>
</table>

## Earlier work

| Project | The one number |
|---|---|
| [Legal-Contract-Analyzer](https://github.com/anthonyrodrigues443/Legal-Contract-Analyzer) | TF-IDF + LightGBM blend beats published RoBERTa-large on CUAD clause classification (0.716 vs 0.650 macro-F1) at 12 ms per contract |
| [Deepfake-Audio-Detection](https://github.com/anthonyrodrigues443/Deepfake-Audio-Detection) | 2.41% EER in-domain, benchmarked against the ASVspoof literature |
| [RAG-Noah](https://github.com/anthonyrodrigues443/RAG-Noah-Multi-Modal-LLM-Assistant) | Multi-modal RAG assistant with document Q&A and real-time vision, [live demo](https://rag-noah.streamlit.app/) |

All repositories: [github.com/anthonyrodrigues443](https://github.com/anthonyrodrigues443?tab=repositories)

## Stack

Python · PyTorch · scikit-learn · XGBoost / CatBoost / LightGBM · sentence-transformers · FAISS · FastAPI · Docker · GitHub Actions
