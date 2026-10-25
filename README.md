# Abdul M.

AI engineer and researcher, working across the stack from neural network internals to LLM systems in production: deep learning, transformers, agents, retrieval, voice, and the evals and inference engineering that make them reliable and cheap to run.

Founder of [Agentimus](https://www.agentimus.io).

## Projects

- **[agent-harness](https://github.com/abdulm-ai/agent-harness):** a small, readable agent loop in TypeScript with the production parts: typed tools with model-actionable errors, idempotent side effects, approval gates, step/token/time budgets with a handoff, schema and domain checks on the output, confidence routing from real signals, and replayable traces. Runs on OpenAI or Anthropic, with a 12-case eval scored per field.
- **[context-graph](https://github.com/abdulm-ai/context-graph):** a Claude Code plugin that records a session as a graph and, after `/compact` or `/clear`, rebuilds the context by calculation instead of a model-written summary: Dijkstra on `-log p` edge weights for relevance (with heat diffusion as the alternative), exponential decay with rehearsal, an exact knapsack under a token budget, and constraints pinned word for word. Benchmarked against `/compact` on planted facts, token cost and the next task.
- **[endless-learner](https://github.com/abdulm-ai/endless-learner):** a game agent that learns from its own failures and trains for days on a laptop CPU, with the network, backprop, Adam and Double DQN written from scratch on NumPy. It has a solvable-level generator with no top tier, a death bank, prioritised replay, an endless curriculum, and continual backprop against plasticity loss. 226M steps and 15 ablation runs measured which of those helped: replaying old tiers mattered most, and two of the failure tricks made it worse.

## Areas

- **Deep learning:** neural network architectures, transformers and attention, embeddings and representation learning, optimisation and training dynamics
- **LLMs:** pre-training and fine-tuning (LoRA, QLoRA), instruction tuning, RLHF and DPO, tokenisation, context length, structured and constrained decoding
- **Inference efficiency:** quantisation, distillation, speculative decoding, KV-cache reuse, batching, prompt caching, routing between small and large models
- **Agents:** tool design, planning loops, state and retries, idempotent side effects, human approval on risky actions
- **Retrieval:** chunking, hybrid search, reranking, answers grounded in cited sources
- **Voice:** realtime speech pipelines, turn-taking, latency budgets, telephony
- **Reliability:** eval sets, regression tests for prompt and model changes, tracing, cost and latency tracking

## Research interests

- **Machine consciousness:** what current theories (global workspace, integrated information, higher-order theories) would predict for artificial systems, and what, if anything, could count as evidence
- **Cheaper inference:** getting the same quality for a fraction of the compute

## Elsewhere

[Medium](https://medium.com/@abdul-m) · [Substack](https://substack.com/@abdu1m) · [LinkedIn](https://www.linkedin.com/in/abdulm-ai)
