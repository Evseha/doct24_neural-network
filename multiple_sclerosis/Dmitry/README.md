![](https://github.com/salfa-ru/doct24_neural-network/blob/main/multiple_sclerosis/Dmitry/img/c6e5c47311949440d1fee4d8c6df71bf.jpg)

# Предсказание рассеянного склероза

<a href='https://github.com/salfa-ru/doct24_neural-network/blob/main/multiple_sclerosis/Dmitry/main.ipynb'> Прогностическая модель </a> </br>

main.ipynb - проект, процесс исследования и обучения модели.</br>

Стэк: numpy, pandas, matplotlib, seaborn, pickle, tensorflow, sklearn.

Статус: **проект в работе.**

Цель: написать прогностическую модель для определения вероятности рассеянного склероза. Где 0 - нет склероза, 1 - есть склероз.

Набора данных: <a href='https://mosmed.ai/en/datasets/aie21selftestmri/'> mosmed.ai </a> </br>

```
folders                 dcm
---------------------------
PAN_BOT_anon             22
ING15_GB3_anon           24
INTERA_GKB12_anon        25
MRI84653_anon            29
EXCELMRI_GP22_anon      369
EXCELMRI_DC3_anon       481
EXCELMRI_GP8_anon       536
EXCELMRI_GVV2_anon      681
EXCELMRI_GKB71_anon     691
EXCELMRI_GKB57_anon     718
EXCELMRI_GP9_anon       818
HDX_MR_anon             828
EXCELMR_GB13_anon       830
EXCELMR_VERES_anon      832
EXCELMRI_GP134_anon     885
EXCELMRI_GKB36_anon     957
EXCELMRI_GP19_anon      967
EXCELMRI_GP209_anon    1086
EXCELMRI_GP212_anon    1154
EXCELMRI_GP214_anon    1204
EXCELMRI_GKB50_anon    1226
EXCELMRI_GP195_anon    1302
EXCELMRI_KDC4_anon     1306
EXCELMRI_GVV3_anon     1315
MR_GP46F1_anon         1339
EXCELMRI_GP52_anon     1359
EXCELMRI_GP67_anon     1392
EXCELMRI_GP68_anon     1574
EXCELMRI_MUH_anon      1633
EXCELMR1_GB1_anon      1644
EXCELMR_NPPCS_anon     1717
EXCELMRI_GP45_anon     1718
EXCELMRI_GP6_anon      1764
EXCELMRI_GP220_anon    1816
EXCELMR_YUD_anon       1833
EXCELMRI_GP2_anon      1947
EXCELMRI_KDC6_anon     2035
EXCELMRI_SM4_anon      2102
EXCELMR2_GB1_anon      2113
EXCELMRI_GVV1_anon     2312
ING30_MDGKB_anon       2410
EXCELMRI_GKB29_anon    2873
```
Размер изображений в зависимости от папки
```
 [(384, 416), (748, 640), (384, 384), (512, 512), (384, 384), (768, 768), (288, 288), (640, 640), (384, 384), (384, 384), (768, 768), (22, 192, 192), (384, 384), (768, 768), (640, 640), (512, 512), (768, 768), (384, 384), (576, 576), (384, 384), (384, 384), (768, 768), (768, 768), (384, 384), (768, 768), (576, 576), (23, 192, 192), (48, 128, 128), (512, 512), (25, 192, 192), (768, 768), (192, 192), (384, 384), (384, 384), (384, 384), (512, 512), (640, 640), (768, 768), (512, 512), (640, 640), (384, 384), (768, 768)]

min: (22, 192, 192) max: (768, 768)
```

![](https://github.com/salfa-ru/doct24_neural-network/blob/main/multiple_sclerosis/Dmitry/img/acc.png)

![](https://github.com/salfa-ru/doct24_neural-network/blob/main/multiple_sclerosis/Dmitry/img/loss.png)

![](https://github.com/salfa-ru/doct24_neural-network/blob/main/multiple_sclerosis/Dmitry/img/cm.png)
