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
## Источники
**Документация и практические примеры**
- scikit-learn: [Naive Bayes — User Guide](https://scikit-learn.org/stable/modules/naive_bayes.html)
- scikit-learn: [Classifier comparison](https://scikit-learn.org/stable/auto_examples/classification/plot_classifier_comparison.html)
- scikit-learn: [Probability calibration](https://scikit-learn.org/stable/modules/calibration.html)
- J. VanderPlas, *Python Data Science Handbook*, глава «In Depth: Naive Bayes Classification» — [онлайн-версия](https://jakevdp.github.io/PythonDataScienceHandbook/05.05-naive-bayes.html)

**Статьи**
- Ng, Jordan (2001). [On Discriminative vs. Generative Classifiers: A comparison of logistic regression and naive Bayes](https://papers.nips.cc/paper/2001/hash/7b7a53e239400a13bd6be6c91c4f6c4e-Abstract.html) — NIPS. Источник результата из раздела 5.1.
- Zhang (2004). [The Optimality of Naive Bayes](https://cdn.aaai.org/FLAIRS/2004/Flairs04-097.pdf) — FLAIRS. Почему NB работает, даже когда допущение нарушено.
- Rennie, Shih, Teevan, Karger (2003). [Tackling the Poor Assumptions of Naive Bayes Text Classifiers](https://web.stanford.edu/class/cs276/handouts/rennie.icml03.pdf) — ICML. Основа `ComplementNB`.
- Niculescu-Mizil, Caruana (2005). [Predicting Good Probabilities With Supervised Learning](https://mlanthology.org/icml/2005/niculescumizil2005icml-predicting) — ICML. О калибровке (в том числе у NB).
