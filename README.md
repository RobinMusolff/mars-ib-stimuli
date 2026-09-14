# MaRs-IB stimuli — matrix reasoning task

Image stimuli for a matrix reasoning task, hosted here so that Qualtrics surveys can reference them
by URL. Serving them from a CDN rather than the Qualtrics Graphics Library keeps the survey files
portable: they keep working across Qualtrics accounts and when shared with collaborators.

## Contents

Each image is one puzzle: a 3×3 matrix with the bottom-right cell missing, and its four answer
options labelled A–D beneath.

- `img/item01.png` … `img/item15.png` — the 15 fielded puzzles, in presentation order (easy to hard)
- `img/example.png` — a worked example shown in the instructions, not scored
- `img/bank/mars_001.png` … `img/bank/mars_080.png` — **all 80 items** of the test form, named by
  MaRs-IB item number (added in `v3`), so any item can be swapped into a survey without another
  upload. The 16 items above appear here too, pixel-identical and with the same option order.

No answer keys are published here, deliberately.

Each composite was assembled from the original separate matrix and option images. The option order
within each puzzle was permuted once under a fixed seed and frozen, because in the source archive the
correct answer is always the first option; positions are spread 4/4/4/3 across A–D.

## Usage

Served through jsDelivr:

```
https://cdn.jsdelivr.net/gh/<user>/mars-ib-stimuli@v2/img/item01.png
https://cdn.jsdelivr.net/gh/<user>/mars-ib-stimuli@v3/img/bank/mars_016.png
```

Tags: `v1` original composites; `v2` adds the drawn 3×3 grid (the version the surveys use); `v3`
adds the 80-item bank and changes nothing in `v2`'s files.

**Pin a tag, not a branch.** A tag is immutable; `@main` would let the images change under a running
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
