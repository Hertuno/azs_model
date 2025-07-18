# Анализ и прогнозирование с использованием RandomForestRegressor

## 📌 Описание проекта

Этот проект демонстрирует полный процесс работы с данными, от предварительной обработки до обучения модели и анализа результатов. Мы используем `RandomForestRegressor` из библиотеки `scikit-learn` для прогнозирования значений на основе очищенных и обработанных данных.

Проект оформлен в виде Jupyter Notebook и готов для включения в портфолио.

## 🛠️ Используемые технологии

* Python 3.x
* Jupyter Notebook (через Anaconda)
* Pandas
* NumPy
* scikit-learn
* Matplotlib / Seaborn (для визуализации)

## 📁 Структура проекта


```
azs_model/
├── config.py                 # Основные настройки проекта
├── holidays.ipynb            # Анализ праздничных дней
├── income.ipynb              # Анализ доходов
├── main.ipynb                # Главный ноутбук для запуска пайплайна
├── meteo.ipynb               # Работа с метеоданными
├── ofd.ipynb                 # Обработка данных ОФД
├── train.ipynb               # Обучение моделей
├── weather.ipynb             # Анализ погодных данных
├── readme.md                 # Описание проекта
├── cfg/                      # Конфигурационные файлы
│   └── config_default.py     # Конфиг по умолчанию
├── datasets/                 # Датасеты
│   ├── parsed/               # Обработанные данные
│   │   ├── calendar_2023.csv
│   │   ├── calendar_2024.csv
│   │   ├── calendar_2025.csv
│   │   ├── income_2023.csv
│   │   ├── income_2024.csv
│   │   ├── weather_2023.csv
│   │   └── weather_2024.csv
│   └── raw/                  # Сырые данные
│       ├── ofd_2023.csv
│       ├── ofd_2024.csv
│       ├── price2023.mxl
│       └── price2024.mxl
├── models/                   # Папка для сохранения моделей
├── notebooks/                # Дополнительные ноутбуки и эксперименты
└── __pycache__/              # Служебные файлы Python
```

**Пояснения к структуре:**
- `config.py`, `cfg/` — конфигурация и параметры запуска
- `*.ipynb` — ноутбуки для анализа, обучения и визуализации
- `datasets/parsed/` — подготовленные для анализа датасеты
- `datasets/raw/` — исходные (сырые) данные
- `models/` — сохранённые модели и артефакты обучения
- `notebooks/` — дополнительные ноутбуки, эксперименты
- `__pycache__/` — служебные файлы Python (автоматически генерируются)


## 📈 Этапы проекта

1. **Загрузка и анализ исходных данных**
2. **Очистка данных и обработка пропусков**
3. **Увеличение числа классов параметров**
4. **Анализ и усечение экстремальных значений**
5. **Устранение выбросов через усреднение**
6. **Балансировка тренировочной и тестовой выборок**
7. **Подбор гиперпараметров модели**
8. **Обучение модели RandomForestRegressor**
9. **Оценка результатов и визуализация ошибок**

## 📊 Результаты

* Модель достигает хороших метрик качества на валидационной выборке.
* Найдены участки с большими отклонениями, выполнен анализ причин.
* Визуализации помогают оценить стабильность и качество модели.

## 🚀 Как запустить

```bash
conda create -n rfenv python=3.10 -y
conda activate rfenv
pip install -r requirements.txt
jupyter notebook
```

## 💡 Возможные улучшения

* Использовать GridSearchCV или Optuna для более тонкого подбора параметров
* Протестировать другие регрессионные модели (LightGBM, XGBoost)
* Добавить автоматическую генерацию отчёта по метрикам

## 📚 Лицензия

MIT License

---

Если вы нашли этот проект полезным, ⭐️ поставьте звезду на GitHub!
