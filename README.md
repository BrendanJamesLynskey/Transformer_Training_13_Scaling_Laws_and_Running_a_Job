# Transformer Training 13 — Scaling Laws, Running a Real Job, and After Pretraining

How big a model for a given budget (IsoFLOP profiles, Kaplan against Chinchilla, a toy sweep); what a running job is watched for; failures, checkpoints and goodput at the scale of thousands of GPUs; and the bridge to fine-tuning.

**Live site:** https://brendanjameslynskey.github.io/Transformer_Training_13_Scaling_Laws_and_Running_a_Job/

C = 6ND and IsoFLOP profiles; Kaplan vs Chinchilla and a toy sweep; extrapolation and overtraining; monitoring; failures at scale; checkpoints and resuming; goodput and Young's interval (interactive); the bridge to SFT, RLHF and DPO.

## Live, animated companion

This deck is the slide companion to Part 2 (Training) of [Transformer Decoder Explained](https://transformer-training-explained.vercel.app/training), where the same model trains in your browser:

- [Chapter 14: Scaling laws](https://transformer-training-explained.vercel.app/training/14-scaling-laws)
- [Chapter 15: Running a real job](https://transformer-training-explained.vercel.app/training/15-running-a-real-job)
- [Chapter 16: After pretraining](https://transformer-training-explained.vercel.app/training/16-after-pretraining)

## Where the numbers come from

Every measured number on these slides comes from the site's [results.md](https://github.com/BrendanJamesLynskey/transformer-explainer/blob/main/results.md) (seeded NumPy reference runs; CI recomputes them), filled in at build time from its `results.json`. Numbers from papers are cited on the slide with a link. The model is tiny (5,376 parameters, one book, a CPU): its runs show mechanisms, not what happens at scale, and the slides say so where it matters. GPU runs of the site's Colab notebooks are pending; no GPU number appears here.

Part of the [Transformer Training sub-hub](https://github.com/BrendanJamesLynskey/LLM_Hub_Transformer_Training) &middot; [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs)
