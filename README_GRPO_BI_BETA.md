# GRPO Bi-Beta Advantage Estimator

This branch adds `grpo_bi_beta`, an outcome-level GRPO-style advantage estimator with separate positive- and negative-channel beta coefficients.

The implementation is based on verl v0.7.1, commit `bec9ef74`.

## Usage

Set the estimator and beta coefficients through the verl config:

```bash
algorithm.adv_estimator=grpo_bi_beta \
algorithm.beta_pos=0.8 \
algorithm.beta_neg=0.3
```

Both `beta_pos` and `beta_neg` must be strictly positive.
