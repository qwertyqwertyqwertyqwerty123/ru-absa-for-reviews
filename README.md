# ru-absa-for-reviews

Portfolio project for aspect-based sentiment analysis (ABSA) of Russian-language reviews.

The repository contains a clean ML project structure, data samples, training and inference entry points, and lightweight metadata for trained models. Large checkpoint files are stored outside GitHub and connected locally through the `models/` directory.

## Project structure

- `data/` - sample raw, interim, and processed data artifacts.
- `src/` - modules for data preparation, training, evaluation, and inference.
- `scripts/` - command-line entry points for the main pipeline stages.
- `models/` - model cards, labels, configs, metrics, and checkpoint manifests.
- `reports/` - metrics, figures, and dataset reports.
- `examples/` - short input text examples and inference demos.

## Data

The repository includes lightweight sample data and documentation for the dataset layout. Full datasets and private review dumps are excluded from Git to keep the project safe for public portfolio use.

## Models

Model weights (`*.bin`, `*.pt`, `*.pth`, `*.safetensors`) are excluded through `.gitignore`.

The `models/aspect_model/` and `models/sentiment_model/` directories contain lightweight, GitHub-friendly metadata:

- `README.md`
- `model_card.md`
- `labels.json`
- `training_config.json`
- `metrics.json`
- `checkpoint_manifest.json`

Actual checkpoint files are managed outside the repository, for example in Hugging Face Hub, Git LFS, S3, Google Drive, or a local archive. The manifest files describe the expected local checkpoint layout.

## Training

Training scripts are located in `scripts/` and `src/train/`. Project constants are defined in `config.py`.

## Inference

Inference uses compatible checkpoint files from `models/aspect_model/` and `models/sentiment_model/`. The repository keeps the code and metadata in Git while leaving heavyweight model artifacts in external storage.

---

# ru-absa-for-reviews

Портфолио-проект для аспектно-ориентированного анализа отзывов на русском языке.

Репозиторий содержит аккуратную структуру ML-проекта, примеры данных, точки входа для обучения и инференса, а также легкие metadata-файлы обученных моделей. Тяжелые checkpoint-файлы хранятся вне GitHub и подключаются локально через директорию `models/`.

## Структура проекта

- `data/` - sample-артефакты raw, interim и processed данных.
- `src/` - модули подготовки данных, обучения, оценки и инференса.
- `scripts/` - CLI-точки входа для основных этапов пайплайна.
- `models/` - model cards, labels, configs, metrics и checkpoint manifests.
- `reports/` - метрики, графики и отчеты по данным.
- `examples/` - короткие примеры входных текстов и инференса.

## Данные

В репозитории лежат легкие sample-данные и документация по структуре датасета. Полные датасеты и приватные выгрузки отзывов исключены из Git, поэтому проект подходит для публичного портфолио.

## Модели

Веса моделей (`*.bin`, `*.pt`, `*.pth`, `*.safetensors`) исключены через `.gitignore`.

Директории `models/aspect_model/` и `models/sentiment_model/` содержат легкие metadata-файлы, которые удобно хранить на GitHub:

- `README.md`
- `model_card.md`
- `labels.json`
- `training_config.json`
- `metrics.json`
- `checkpoint_manifest.json`

Сами checkpoint-файлы управляются вне репозитория, например через Hugging Face Hub, Git LFS, S3, Google Drive или локальный архив. Manifest-файлы фиксируют ожидаемую локальную структуру чекпоинта.

## Обучение

Скрипты обучения находятся в `scripts/` и `src/train/`. Константы проекта заданы в `config.py`.

## Инференс

Инференс использует совместимые checkpoint-файлы из `models/aspect_model/` и `models/sentiment_model/`. В Git хранится код и metadata, а тяжелые артефакты моделей остаются во внешнем хранилище.
