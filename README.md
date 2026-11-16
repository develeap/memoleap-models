# Memoleap speech models

Speech-to-text models that the Memoleap Mac app downloads on first use. The files are attached to this
repository's [releases](../../releases); the repository itself holds only this page and the licence.

## Hebrew, fast (`ivrit-turbo-mlx`)

- **What it is:** [ivrit-ai/whisper-large-v3-turbo](https://huggingface.co/ivrit-ai/whisper-large-v3-turbo), a
  Whisper large-v3-turbo model fine-tuned for Hebrew by [ivrit.ai](https://www.ivrit.ai), converted to the
  [MLX](https://github.com/ml-explore/mlx) format so it runs on Apple silicon with `mlx-whisper`.
- **What was changed:** only the file format. The weights were converted with the `convert.py` script of
  [mlx-examples/whisper](https://github.com/ml-explore/mlx-examples/tree/main/whisper); nothing was trained or
  tuned here.
- **Files:** `ivrit-turbo-mlx.config.json` and `ivrit-turbo-mlx.weights.safetensors`. Saved as `config.json`
  and `weights.safetensors` in one folder, they are a model folder `mlx-whisper` loads.

| File | SHA-256 |
|---|---|
| `ivrit-turbo-mlx.weights.safetensors` | `6e4f277ab7cdce96a22a741fce39376473ea9f923ccee4d718101600a2fd9d4e` |
| `ivrit-turbo-mlx.config.json` | `b34fc29e4e11e0a25e812775dd67f4dd16fc2c8eb43d28ae25ff7d660ecb6379` |

## Licence and credit

The original model is the work of ivrit.ai and is published under the Apache License 2.0; this converted copy
is passed on under the same licence (see `LICENSE`). Whisper is by OpenAI. All credit for the model's quality
belongs to ivrit.ai and the people who gave their recordings and transcripts to it.
