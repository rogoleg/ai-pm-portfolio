# AI Product Manager Portfolio

Working artifacts from AI product work: prompt libraries, evaluation harnesses and case studies. The point of this repo is to show how I think about AI features, not just to talk about them.

## Structure

- `prompt-library/` — versioned prompts with intent, constraints and known failure modes
- `eval-harness/` — test sets, scoring logic and pass rates for model/prompt changes
- `case-studies/` — problem → approach → measured result, one folder per feature

## How I work with AI features

1. Define the user job and the failure that actually matters (not “accuracy”).
2. Write the eval set before writing the prompt.
3. Treat prompts like code: diff, review, roll back.
4. Measure cost, latency and failure rate together.
5. Always ship with a fallback path.

## Status

Early build — content landing week by week.
