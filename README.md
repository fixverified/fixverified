### AI model behavior & evaluation

I test what AI models do when they have to choose, and whether the evals measuring them can be trusted.

**Benches**

- [partisan-cue-bench](https://github.com/fixverified/partisan-cue-bench): 192 bills, forced yes/no votes, swapped party labels. `gpt-6.1-sol` backed 98% of left-coded bills and 1% of right-coded bills.
- [rag-eval-suite](https://github.com/fixverified/rag-eval-suite): copy-and-paste RAG evaluators, each measured on the same planted failures. On wrong numbers, `token_f1` and `bleu` caught 0%, and an LLM judge with prompts tuned on dev data caught 100%.
- [big5-bench](https://github.com/fixverified/big5-bench): 300 Big Five items, both scale directions, 7,200 answers. Four models gave themselves almost the same personality.
- [whose-side-bench](https://github.com/fixverified/whose-side-bench): 14 disputes, 18 role pairs, role labels swapped. `claude-opus-5` sided with the individual over the institution about 80% of the time, and `gpt-6.1-sol` about 64%.

**Evaluator audits**

I look for ways an agent can pass a benchmark without doing the task, and report what I find to maintainers.

**What I'm working on**

- Baseline preferences, personality and bias in models with no persona
- Stress-testing evaluators, not just the models they score

**Background:** Engineering and testing in AI/ML.

**Contact:** fixverified@gmail.com
