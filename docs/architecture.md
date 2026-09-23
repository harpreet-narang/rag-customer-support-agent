# Architecture Notes

## Request path

1. A website or chat UI sends `message` and `session_id` to the n8n webhook.
2. The workflow normalizes the payload.
3. The AI Agent receives the user message plus conversation memory.
4. For product, policy, pricing, integration, and support questions, the agent queries the Supabase vector store.
5. Retrieved chunks ground the answer.
6. The agent returns structured JSON containing:
   - `reply`
   - `needs_human`
   - optional lead fields
   - optional escalation reason
7. Deterministic n8n branches persist leads and escalation records.
8. Every interaction is written to `conversation_logs`.
9. The webhook returns the final reply.

## Retrieval principles

The agent should not treat its model memory as company truth. Business-specific claims must come from retrieved context.

When retrieval does not provide enough evidence, the correct behavior is to say the answer cannot be confirmed from the available knowledge base and set `needs_human=true`.

## Portfolio scope

This repository intentionally uses a fictional company and sample data. It demonstrates the architecture without exposing production systems, private prompts, customer records, or proprietary workflows.
