# Vireo-4B: Efficient Reasoning at Small Scale

**Aurelite Labs — model announcement · 14 October 2025**

Vireo-4B is a 4.1B-parameter open-weight language model built for multi-step reasoning.
It is the smallest model in the Launch Cycle 2025 public release set and is positioned for
teams that need strong reasoning behaviour on commodity hardware.

## Highlights

- 4.1B parameters, 32k context window
- Refreshed post-training recipe focused on reasoning traces
- Apache-2.0 weights and inference code
- Accepted at NeurIPS 2025 (Spotlight)

## Benchmarks

| Suite | Vireo-4B | Previous small-model baseline |
| --- | --- | --- |
| GSM8K | 71.4 | 63.2 |
| MATH-500 | 38.9 | 31.5 |
| ARC-Challenge | 62.1 | 57.8 |

## Availability

Code and weights are published in the official code repository:
`https://github.com/komal74784391-netizen/aurelite-code-vireo-4b`

## Citation

```bibtex
@inproceedings{aurelite2025vireo,
  title={Vireo-4B: Efficient Reasoning at Small Scale},
  author={Aurelite Labs},
  booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
  year={2025}
}
```
