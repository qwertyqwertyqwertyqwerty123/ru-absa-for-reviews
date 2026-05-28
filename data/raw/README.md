# Raw Data

### Files 
- `raw_data_sample.csv` - example of raw data parsed from open sources
## CSV structure

The dataset is stored in CSV format. Each row represents one user review.

| Column | Type | Description                                                                  |
|---|---|------------------------------------------------------------------------------|
| `review_id` | `string` | Unique review identifier.                                                    |
| `item_id` | `string` | Identifier of the reviewed item.                                             |
| `source_url` | `string` | URL of the source page where the review was collected.                       |
| `author` | `string` | Review author name or nickname.                                              |
| `experience` | `string` | Additional user experience information from the source page, if available.   |
| `date_published` | `string` | Normalized review publication date.                                          |
| `date_human` | `string` | Original human-readable publication date from the source page.               |
| `rating` | `float` | How user rated this quest, if available.                                     |
| `is_genius` | `bool` | Indicates whether the author or review has a special source-platform status. |
| `is_verified` | `bool` | Indicates whether the review is verified by the source platform.             |
| `text` | `string` | Main review text used for NLP tasks.                                         |

___
# Сырые данные

### Файлы
- `raw_data_sample.csv` - пример сырых данных, взятых из открытых источников
## Структура CSV-файла

Датасет хранится в формате CSV. Каждая строка соответствует одному пользовательскому отзыву.

| Столбец | Тип | Описание                                                                       |
|---|---|--------------------------------------------------------------------------------|
| `review_id` | `string` | Уникальный идентификатор отзыва.                                               |
| `item_id` | `string` | Идентификатор объекта, к которому относится отзыв.                             |
| `source_url` | `string` | Ссылка на страницу-источник, с которой был получен отзыв.                      |
| `author` | `string` | Имя или никнейм автора отзыва.                                                 |
| `experience` | `string` | Дополнительная информация о пользовательском опыте, если она есть в источнике. |
| `date_published` | `string` | Нормализованная дата публикации отзыва.                                        |
| `date_human` | `string` | Исходная человекочитаемая дата публикации с сайта-источника.                   |
| `rating` | `float` | Оценка квеста пользователем, если она указана.                                 |
| `is_genius` | `bool` | Признак специального статуса автора или отзыва на платформе-источнике.         |
| `is_verified` | `bool` | Признак верифицированного отзыва на платформе-источнике.                       |
| `text` | `string` | Основной текст отзыва, используемый для NLP-задач.                             |