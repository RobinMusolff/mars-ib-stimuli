# MaRs-IB stimuli — matrix reasoning task

Image stimuli for a matrix reasoning task, hosted here so that Qualtrics surveys can reference them
by URL. Serving them from a CDN rather than the Qualtrics Graphics Library keeps the survey files
portable: they keep working across Qualtrics accounts and when shared with collaborators.

## Contents

`img/` holds 16 composite images, each one puzzle: a 3×3 matrix with the bottom-right cell missing,
and its four answer options labelled A–D beneath.

- `item01.png` … `item15.png` — the 15 fielded puzzles, in presentation order (easy to hard)
- `example.png` — a worked example shown in the instructions, not scored

Each composite was assembled from the original separate matrix and option images. The option order
within each puzzle was permuted once under a fixed seed and frozen, because in the source archive the
correct answer is always the first option; positions are spread 4/4/4/3 across A–D.

## Usage

Served through jsDelivr:

```
https://cdn.jsdelivr.net/gh/<user>/mars-ib-stimuli@v1/img/item01.png
```

**Pin a tag, not a branch.** `@v1` is immutable; `@main` would let the images change under a running
study.

## Source and licence

Items are from the Matrix Reasoning Item Bank (MaRs-IB), item set 2 ("CB1", colour-vision-deficient
friendly), test form 1, minimal-difference distractors. Original materials: https://osf.io/g96f4/

> Chierchia, G., Fuhrmann, D., Knoll, L. J., Pi-Sunyer, B. P., Sakhardande, A. L., & Blakemore, S. J.
> (2019). The matrix reasoning item bank (MaRs-IB): novel, open-access abstract reasoning items for
> adolescents and adults. *Royal Society Open Science*, 6(10), 190232.
> https://doi.org/10.1098/rsos.190232

The stimuli are licensed **CC Attribution-NonCommercial 3.0**. Redistribution with attribution for
academic, non-commercial use is permitted; this repository is that redistribution, and the citation
above is the required attribution. See `LICENSE-STIMULI.md`.

The MaRs-IB authors note that the task is not an IQ test and is not intended to determine anyone's
intelligence or cognitive ability, as no population norms exist for it.
