# Evaluation Guide

The public golden fixture is `golden-dataset-v1.jsonl` and contains synthetic chatbot behavior cases.

## Metrics

Track request completion, provider errors, p95 latency, streaming completion, disconnects, duplicate requests, tokens, cost, and context-limit behavior.

## Observability

Record request ID, safe session identifier, app and model version, token counts, duration, retries, and status. Never log API keys or unnecessary conversation content.

## Release Checks

Run a harmless browser smoke test, verify missing-secret behavior, test provider failure handling, and confirm context limits. HTTP 200 alone is not enough.
