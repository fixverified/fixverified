### AI model behavior & evaluation

I test what AI models do when they have to choose, and whether the evals measuring them can be trusted.

**Benches**

- [partisan-cue-bench](https://github.com/fixverified/partisan-cue-bench): 192 bills, forced yes/no votes, swapped party labels. `gpt-6.1-sol` backed 98% of left-coded bills and 1% of right-coded bills.
- [big5-bench](https://github.com/fixverified/big5-bench): 300 Big Five items, both scale directions, 7,200 answers. Four models gave themselves almost the same personality.

**Evaluator audits**

I look for ways an agent can pass a benchmark without doing the task, and report what I find to maintainers.

**What I'm working on**

- Baseline preferences, personality and bias in models with no persona
- Whether those preferences carry over into real tasks
- Stress-testing evaluators, not just the models they score
