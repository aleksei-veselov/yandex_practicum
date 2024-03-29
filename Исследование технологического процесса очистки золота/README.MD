# Восстановление золота из руды

Подготовьте прототип модели машинного обучения для «Цифры». Компания разрабатывает решения для эффективной работы промышленных предприятий.

Модель должна предсказать коэффициент восстановления золота из золотосодержащей руды. Используйте данные с параметрами добычи и очистки. 

Модель поможет оптимизировать производство, чтобы не запускать предприятие с убыточными характеристиками.

Вам нужно:

1. Подготовить данные;
2. Провести исследовательский анализ данных;
3. Построить и обучить модель.

Чтобы выполнить проект, обращайтесь к библиотекам *pandas*, *matplotlib* и *sklearn.* Вам поможет их документация.

# Описание данных
**Технологический процесс**

- *Rougher feed* — исходное сырье;
- *Rougher additions* (или reagent additions) — флотационные реагенты: Xanthate, Sulphate, Depressant:

1) *Xanthate* — ксантогенат (промотер, или активатор флотации);

2) *Sulphate* — сульфат (на данном производстве сульфид натрия);

3) *Depressant* — депрессант (силикат натрия).

- *Rougher process* (англ. «грубый процесс») — флотация;
- *Rougher tails* — отвальные хвосты;
- *Float banks* — флотационная установка;
- *Cleaner process* — очистка;
- *Rougher Au* — черновой концентрат золота;
- *Final Au* — финальный концентрат золота.

**Параметры этапов**
- *air amount* — объём воздуха;
- *fluid levels* — уровень жидкости;
- *feed size* — размер гранул сырья;
- *feed rate* — скорость подачи.

**Наименование признаков**

*Наименование признаков должно быть такое:*

**[этап].[тип_параметра].[название_параметра]**

**Пример:** rougher.input.feed_ag

*Возможные значения для блока* **[этап]:**
- rougher — флотация;
- primary_cleaner — первичная очистка;
- secondary_cleaner — вторичная очистка;
- final — финальные характеристики.

*Возможные значения для блока* **[тип_параметра]:**
- *input* — параметры сырья;
- output* — параметры продукта;
- *state* — параметры, характеризующие текущее состояние этапа;
- *calculation* — расчётные характеристики.

**Данные находятся в трёх файлах:**

- gold_industry_train.csv — **обучающая выборка;**
- gold_industry_test.csv — **тестовая выборка;**
- gold_industry_full.csv — **исходные данные.**

# **Вывод:**
- Подготовлена функция для вычисления итоговой sMAPE;
- Произведена подготовка данных для обучения моделей;
- Произведено масштабирование признаков;
- Произведено обучение различных моделей и оценка их качества при помощи кросс-валидации;
- Произведен выбор лучшей модели и ее проверка на тестовой выборке. 

Лучшие результаты, показала модель LinearRegression (итоговое sMAPE = 7.148113977588695).
