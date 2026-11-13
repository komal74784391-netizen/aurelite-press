# Launch Cycle 2025 — Everything We Announced

*Aurelite Labs keynote recap · 12 November 2025 · 14 min read*

Launch Cycle 2025 was our largest release cycle to date: five public model families, a new
inference stack, three research previews, a revised open-weights policy, and a packed
two-day keynote. This page is the single consolidated recap of everything that was
announced. If you only read one Aurelite post this year, make it this one.

## Keynote in one paragraph

We opened with a reminder of Aurelite's mission — small teams shipping carefully evaluated
open models — and closed with a roadmap that takes us through the next four quarters. In
between there were 27 announcements: new dense decoders, our first production mixture-of-
experts model, a vision-language refresh, a code-assistant release, a family of compact
multilingual models, and a long list of infrastructure and tooling updates. The sections
below walk through each of them in the order they appeared on stage.

## The full line-up

### Foundation models

1. **Vireo-4B** — our 4.1B-parameter dense reasoning model. Vireo-4B was the first model
   shown on stage. It uses a refreshed post-training recipe that emphasises multi-step
   reasoning traces, and it ships with a 32k context window. The team reported strong
   results on grade-school math and logical deduction suites, and a companion technical
   report was made available alongside the announcement. Vireo-4B is part of the public
   release set.
2. **Sable-13B** — a 13.2B dense decoder with a 128k context window. Sable extends our
   earlier long-context work with a new position-encoding scheme and a curriculum that
   mixes long-document summarisation with retrieval-augmented tasks. Available now.
3. **Corvus-MoE-8x2B** — the headline release of the cycle. Corvus is our first production
   sparse mixture-of-experts model: eight experts, top-2 routing, 15.8B total parameters
   and 2.3B active parameters per token. The keynote focused on its routing stability and
   throughput at long sequence lengths. Corvus is part of the public release set and was
   accepted at NeurIPS 2025.
4. **Lumen-2** — a 7.4B vision-language model that replaces Lumen-1. Lumen-2 adds
   document understanding, chart reasoning and a new image-token compressor. A refreshed
   model card and serving guide accompany the announcement.
5. **Arden-400M** — a 420M compact multilingual model covering 23 languages, aimed at
   on-device deployment. Arden was described as a research artifact; the keynote noted
   that the model card would be the only public artifact for this release.
6. **Quill-1.5** — a 1.5B code-assistant model with a fill-in-the-middle objective and a
   repository-aware context builder. Quill-1.5 targets laptop-class inference and ships
   with an editor integration example.
7. **Tessel-350M** — a 350M research preview used to study data-mixing ratios at small
   scale. Tessel was shown in the research section of the keynote with preliminary
   learning-curve plots; it remains an internal evaluation preview rather than a public
   model release.

### Research previews and roadmap items

8. **Aster-7B** — a sparse-attention experiment planned for Q2.
9. **Boreal-3B** — a Nordic-language pilot, evaluation ongoing.
10. **Cinder-1B** — a distilled reranker, early experiments.
11. **Dune-22B** — a long-context continuation of Sable, exploratory.
12. **Ember-9B** — a multimodal reranker, concept stage.
13. **Fjord-2B** — an on-device speech bridge, research only.
14. **Gale-30B** — a flagship dense model, roadmap H2.
15. **Halo-800M** — an embedding model, internal benchmark stage.
16. **Iris-6B** — a vision encoder study, no release planned yet.
17. **Juniper-1.2B** — a compact summariser, under evaluation.
18. **Kestrel-5B** — a retrieval-augmented decoder, prototype.
19. **Larch-2.7B** — a multilingual expansion of Arden, planned.
20. **Mesa-18B** — a mixture-of-experts sibling of Corvus, speculative.
21. **Nook-500M** — a tiny instruction follower, preview.
22. **Opal-4B** — a reasoning distill of Vireo, planned.
23. **Pine-11B** — a long-context code model, exploratory.
24. **Rook-1.4B** — a tool-use experiment, internal.
25. **Sparrow-900M** — a speculative-decoding draft model, concept.
26. **Talon-3.5B** — a vision-language distill, planned.
27. **Vale-24B** — a future flagship, roadmap only.

## Infrastructure and policy

The keynote also introduced the Aurelite Inference Stack 2.0, a rewritten serving runtime
with chunked prefill and continuous batching, plus a new evaluation harness that will be
used for all future launches. The open-weights policy was revised: every public model
release from Launch Cycle 2025 onward will publish weights and inference code under
Apache-2.0 unless explicitly noted otherwise.

## Availability summary

Public release set: Vireo-4B, Sable-13B, Corvus-MoE-8x2B, Lumen-2, Arden-400M and
Quill-1.5. Research previews and roadmap items in the numbered list above are not part
of the public release set. For per-model details see the dedicated announcement pages
listed in the press-room index.
