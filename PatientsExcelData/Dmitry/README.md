# Предсказание врожденного порога сердца у детей

<a href='https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/main.ipynb'> Прогностическая модель </a> </br>
<a href='https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/Notebook.ipynb'> Применение </a> 

main.ipynb - проект, процесс исследования и обучения модели.</br>
Notebook.ipynb  - пример работы.</br>
model.h5  - модель.</br>
model.py -  алгоритм предобработки сырых данных для подачи в нейронную сеть. Принимает текст диагноза. Так же вызывает модель и возвращает результат.</br>
tokenizer.pickle - частный словарь.

Результат обучения моделей нейронных сетей на разных признаках.
![](https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/png/all.png)
![](https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/png/all1.png)

В итоге, выбрали и обучили модель нейронной сети только на признаке Diagnosis
![](https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/png/train_result.png)
![](https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/png/embedding_model.png)
</br> Верно опредленно: </br>
99% -  отсутствие порога сердца </br>
89% - порог сердца</br>
</br>
Итоговая точность прогноза модели: 94%

![](https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/png/cm_all.png)

Исследование качества прогноза других моделей того же признака с учетом погрешности.
![](https://github.com/salfa-ru/doct24_neural-network/blob/main/PatientsExcelData/Dmitry/png/other_model_result.png)
