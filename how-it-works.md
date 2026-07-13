# How Defacta works

Defacta takes a piece of text - typically AI-generated - and returns a structured verdict on how trustworthy it is.

## The pipeline

1. **Submit text.** Send the content you want checked to Defacta through the REST API, an MCP call, or the browser extension.
2. **Claim extraction.** Defacta breaks the text into individual factual claims that can be checked independently.
3. **Verification against sources.** Each claim is evaluated against credible sources to see whether it is supported, contradicted, or unverifiable.
4. **Signal detection.** Alongside factual accuracy, Defacta flags bias, manipulation, and deception patterns in the text.
5. **Structured result.** You get back a JSON payload summarizing which claims held up, which did not, and what was flagged.

## Structured output

Because results are returned as JSON, you can gate an AI response on them, log them for audit, or surface them inline in a UI - without parsing free text.

> Endpoint names and exact response fields are approximated for this demo preview. See the official Defacta docs for the real API contract.
