# Sable-13B: Long Context Without the Long Wait

**Aurelite Labs — model announcement · 15 October 2025**

Sable-13B is a 13.2B-parameter dense decoder with a 128k-token context window. It extends
Aurelite's long-context line with a new position-encoding scheme and a training curriculum
that mixes long-document summarisation with retrieval-augmented generation.

## Highlights

- 13.2B parameters, 128k context
- New position-encoding scheme for stable long-context attention
- Apache-2.0 weights and inference code
- Accepted at NeurIPS 2025

## Intended use

Sable-13B is intended for document analysis, long-form summarisation and retrieval-heavy
assistant workloads. It is not evaluated for safety-critical applications.

## Availability

Code and weights are published in the official code repository:
`https://github.com/komal74784391-netizen/aurelite-code-sable-13b`
