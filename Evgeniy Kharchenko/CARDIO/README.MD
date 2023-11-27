Разработка модели предсказания сердечно-сосудистых заболеваний
Данные
* age - Age | Objective Feature | int (days);
* gender - Gender | Objective Feature | categorical code |;
* height - Height | Objective Feature | int (cm) |;
* weight - Weight | Objective Feature | float (kg) |;
* ap_hi - Systolic blood pressure | Examination Feature | int |;
* ap_lo - Diastolic blood pressure | Examination Feature | int |;
* cholesterol - Cholesterol | Examination Feature | 1: normal, 2: above normal, 3: well above normal |;
* gluc - Glucose | Examination Feature | 1: normal, 2: above normal, 3: well above normal |;
* smoke - Smoking | Subjective Feature | binary |;
* alco - Alcohol intake | Subjective Feature | binary |;
* active - Physical activity | Subjective Feature | binary |;
* cardio - Presence or absence of cardiovascular disease | Target Variable | binary |.

Цель исследования:
Научить модель предсказывать болезнь по медицинским показателям
Ход исследования
Мы проверили данные на ошибки и оценили их влияние на исследование. Затем, на этапе предобработки мы нашли возможность исправить самые критичные ошибки данных.

Таким образом, исследование прошло в несколько этапов:

Обзор данных.
Предобработка данных.
Проверка моделей.
Навыки и инструменты
pandas, numpy, matplotlib, seaborn, sklearn, catboost, lgbm, optuna 
Результат
В рамках данного проекта был исследован датасет с данными людей различного возраста, роста, веса и медицинских показателей о предрасположенности к сердечно-сосудистым заболеваниям. Датасет был проверен на дубликаты и пропуски, возраст был переведен в года и округлен, были исправлены отрицательные значения в данных, удалены выбросы, исследована корреляция признаков и зависимость признаков на целевой признак. Было обнаружено, что нет показателей предрасположенности у людей младше 38 лет, но удалять данные не стал, так как в "очищенном" датасете целевой признак сбалансирован. Чтобы модели легче обучались применил Standart Scaler. Лучший резельтат показала модель CatBoostClassifier.
