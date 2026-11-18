# Case Studies

One folder per AI feature. Fixed structure so cases are comparable rather than storytelling exercises:

```
case-name/
  README.md      problem, users, constraints, decision, result
  evidence/      eval runs, screenshots, latency or cost numbers
  decision.md    what we shipped, what we cut, what would change our mind
```

## The five questions every case study answers

1. **What job** was the user trying to do, and what did they do instead today?
2. **Why AI** — what makes a deterministic solution worse here?
3. **What failure** would hurt most, and how was it measured?
4. **What shipped**, with numbers: pass rate, latency, cost per call.
5. **What we cut** and why — scope discipline is the actual signal.

## Planned cases

- [ ] Support triage assistant — classification + routing, measured by misroute rate
- [ ] Document Q&A over a product catalogue — RAG with citation accuracy as the metric
- [ ] Agentic workflow with a human approval step — measured by completion rate vs manual baseline
