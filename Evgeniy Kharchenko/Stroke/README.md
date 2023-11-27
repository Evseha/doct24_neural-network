Разработка модели предсказания инсульта

Описание Датасета

id: unique identifier

gender: "Male", "Female" or "Other"

age: age of the patient

hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension

heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease

ever_married: "No" or "Yes"

work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"

Residence_type: "Rural" or "Urban"

avg_glucose_level: average glucose level in blood

bmi: body mass index

smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*

stroke: 1 if the patient had a stroke or 0 if not

*Note: "Unknown" in smoking_status means that the information is unavailable for this patient

Цель исследования:
Научить модель предсказывать болезнь по медицинским показателям

Ход исследования
Мы проверили данные на ошибки и оценили их влияние на исследование. Затем, на этапе предобработки мы нашли возможность исправить самые критичные ошибки данных.

Таким образом, исследование прошло в несколько этапов:

Обзор данных.
Предобработка данных.
Подбор параметров и обучение моделей.
Проверка моделей.

Навыки и инструменты
pandas, numpy, matplotlib, seaborn, sklearn, catboost, lgbm, optuna 

Результат
В процессе работы была проведена преодобработка данных. Датасет был проверен на пропуски и дубликаты. Был разобран каждый столбец, а именно были преобразованы категориальные признаки в численные, устранены выбросы в данных согласно статистике. Далее для обучения моделей датасет был разделен на обучающую и тестовую выборки. Так как в данных был дисбаланс классов, в тренировочной выборке был исправлен дисбаланс для нормального обучения моделей. В процессе обучения моделей лучший результат показала модель LGBMClassifier
