# Corvus-MoE-8x2B: Sparse Routing at Scale

**Aurelite Labs — model announcement · 20 October 2025**

Corvus-MoE-8x2B is Aurelite's first production sparse mixture-of-experts model: eight
experts with top-2 routing, 15.8B total parameters and 2.3B active parameters per token.
It is designed to deliver dense-model quality at sparse-model serving cost.

## Highlights

- 8 experts, top-2 routing, 15.8B total / 2.3B active parameters
- Routing-stability improvements for long sequences
- Accepted at NeurIPS 2025
- Trained on the Aurelite mixed corpus v4

## Benchmarks

| Suite | Corvus-MoE-8x2B |
| --- | --- |
| MMLU | 68.2 |
| HellaSwag | 82.7 |
| LongBench | 44.6 |

## Availability

The implementation, evaluation scripts and pretrained checkpoints will be released with
the camera-ready version of the paper. Watch the Aurelite organisation for the release.

## Citation

```bibtex
@article{aurelite2025corvus,
  title={Corvus-MoE: Sparse Routing at Scale},
  author={Aurelite Labs},
  journal={Preprint},
  year={2025},
  note={Under review}
}
```
