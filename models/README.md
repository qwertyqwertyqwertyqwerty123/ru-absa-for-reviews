# Models

This directory contains lightweight model metadata and local checkpoint folders.

Large checkpoint files are intentionally excluded from Git:

- `*.bin`
- `*.pt`
- `*.pth`
- `*.safetensors`

The repository keeps metadata in Git and stores trained checkpoints outside GitHub. Local checkpoint files are placed in `models/aspect_model/` and `models/sentiment_model/` for evaluation and inference.

Subdirectories:

- `aspect_model/` - aspect detection model metadata and local checkpoint layout.
- `sentiment_model/` - sentiment classification model metadata and local checkpoint layout.

---

# Модели

Эта директория содержит легкие metadata-файлы моделей и локальные папки для checkpoint-файлов.

Крупные файлы чекпоинтов исключены из Git:

- `*.bin`
- `*.pt`
- `*.pth`
- `*.safetensors`

В репозитории хранится metadata, а обученные checkpoint-файлы находятся вне GitHub. Локальные файлы чекпоинтов размещаются в `models/aspect_model/` и `models/sentiment_model/` для оценки и инференса.

Поддиректории:

- `aspect_model/` - metadata модели определения аспектов и локальная структура чекпоинта.
- `sentiment_model/` - metadata модели классификации тональности и локальная структура чекпоинта.
