Исследование данных в области Гипертонии

Для предсказания заболевания используются следующие признаки:

age: age in years
sex:
0 = Female
1 = Male

cp: Chest pain types
0 = Typical angina
1 = Atypical angina
2 = Non-angina pain
3 = Asymptomatic

trestbps: Resting blood pressure (mmHg)
High blood pressure = 140 mmHg or above

chol: Serum cholestoral (mg/dL)
Certain elements in the blood, including low-density lipoprotein (LDL), high-density lipoprotein (HDL) and triglycerides Calculation = HDL + LDL + 0.2 * triglycerides.Higher than 200 mg/dL is concerned

fbs: Fasting blood sugar (> 120 mg/dL)
0 = False
1 = True

restecg: Resting electrocardiographic results
0 = Normal
1 = Abnormal ST-T wave
2 = Showing probable or definite left ventricular hypertrophy

thalach: Maximum heart rate achieved (bpm)

exang: Exercise induced angina
0 = Negative
1 = Positive

oldpeak: ST depression induced by exercise relative to rest

slope: The slope of the peak exercise ST segment
0 = Upsloping
1 = Horizontal
2 = Downsloping

ca: Number of major vessels (0-3) colored by fluoroscopy. The colored blood vessels are passing through. There is a clot if the blood vessel is not colored

thal: Thallium scintigraphy
3 = Normal
6 = Fixed defect
7 = Reversable defect

target: Whether the patient has hypertension
0 = Negative
1 = Positive

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
Проведя предобработку датасета, проверив на наличие пропусков, дубликатов и выбросов, проверив корреляцию признаков мы пришли к выводу, что большая часть признаков имеют отрицательную корреляцию. Отрицательная корреляция может быть, если использовать только признаки с положительной корреляцией, то останется слишком мало признаков. Было принято решение оставить признаки с более высокой корреляцией. Обучив несколько моделей, подобрав гиперпраметры, мы сделали вывод, что наилучший результат показали модели CatBoostClassifier и LightGBM.
