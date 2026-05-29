# Sentiment Model

This directory contains metadata for the trained sentiment classification model.

Large checkpoint files are stored outside GitHub and restored locally for inference or evaluation.

Local checkpoint layout:

- `config.json`
- `model.safetensors` or `pytorch_model.bin`
- `tokenizer.json`
- `tokenizer_config.json`
- `special_tokens_map.json`

`checkpoint_manifest.json` documents the expected artifact list and external storage notes.
