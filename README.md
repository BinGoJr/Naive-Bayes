# NaiveBayes

Ноутбук `NaiveBayes.ipynb` с экспериментами по наивному байесовскому классификатору.

## Установка и запуск

Нужен Python 3.14 и интернет при первом запуске (датасет 20 Newsgroups скачивается автоматически).

### Вариант 1: uv

```bash
# 1. Клонировать репозиторий
git clone https://github.com/BinGoJr/Naive-Bayes.git
cd Naive-Bayes

# 2. Создать окружение и установить зависимости (версии берутся из uv.lock)
uv sync

# 3. Запустить Jupyter
uv run --with jupyter jupyter notebook NaiveBayes.ipynb
```

### Вариант 2: pip

```bash
# 1. Клонировать репозиторий
git clone https://github.com/BinGoJr/Naive-Bayes.git
cd Naive-Bayes

# 2. Создать виртуальное окружение
python -m venv .venv
source .venv/bin/activate        # Linux/macOS
# .venv\Scripts\activate         # Windows

# 3. Установить зависимости
pip install -r requirements.txt

# 4. Запустить Jupyter
jupyter notebook NaiveBayes.ipynb
```
