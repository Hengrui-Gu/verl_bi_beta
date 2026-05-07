# GRPO Bi-Beta Advantage Estimator

This repository contains a minimal verl v0.7.1 implementation of `grpo_bi_beta`, an outcome-level GRPO-style advantage estimator with separate positive- and negative-channel beta coefficients.

Base commit:

```text
bec9ef74 [misc] chore: bump version to 0.7.1 (#5602)
```

## Usage

Set the estimator and beta coefficients through the verl config:

```bash
algorithm.adv_estimator=grpo_bi_beta \
algorithm.beta_pos=0.8 \
algorithm.beta_neg=0.3
```

Both `beta_pos` and `beta_neg` must be strictly positive.

