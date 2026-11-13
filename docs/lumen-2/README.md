# Lumen-2 — Model Card and Serving Guide

**Aurelite Labs documentation · Lumen-2 · last updated 22 October 2025**

This page is the dedicated documentation for Lumen-2. It covers the model card, supported
input formats, recommended serving configuration and the evaluation protocol used for the
technical report.

## Model card

| Field | Value |
| --- | --- |
| Parameters | 7.4B |
| Modalities | image, text |
| Context | 8k text tokens, 16 images per request |
| License | Apache-2.0 |
| Release | Launch Cycle 2025 |

## Supported inputs

- PNG, JPEG and WebP images up to 4096x4096
- PDF pages rendered through the bundled preprocessing helper
- Interleaved image-text conversations

## Serving

Lumen-2 is served through the Aurelite Inference Stack 2.0. The reference configuration uses
one GPU per replica with chunked prefill enabled. See `examples/serving.yaml` in the code
repository for a starting point.

## Evaluation protocol

The technical report evaluates Lumen-2 on DocVQA, ChartQA and a held-out internal table
suite. Numbers are reproducible with the evaluation scripts in the official code repository:
`https://github.com/komal74784391-netizen/aurelite-code-lumen-2`
