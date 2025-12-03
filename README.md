# USD/CHF Forex Price Forecasting (LSTM)

Ushbu loyiha USD/CHF valyuta juftligining kelgusi narxlarini AI yordamida bashorat qilish uchun yaratilgan. 
Model 2005–2024 yillar orasidagi tarixiy ma'lumotlar asosida 7 kunlik kelajak narxlarini prognoz qiladi.

## Loyihaning maqsadi
- Forex bozoridagi USD/CHF narx harakatini tahlil qilish
- 60 kunlik tarixiy ma’lumotdan foydalanib 7 kunlik kelajak narxini bashorat qilish
- Real va bashorat qilingan narxlarni grafikda ko‘rsatish
- Modelning aniqligini (MAE, RMSE, MAPE, Accuracy) o‘lchash

## Ishlatilgan texnologiyalar
- Python, Pandas, NumPy
- TensorFlow/Keras (LSTM)
- Scikit-learn (Scaling, Metrics)
- Matplotlib (grafiklar)

## Ishlatilgan model
- 2 qatlamli LSTM + Dropout + Dense(7)
- Nega LSTM?
  - Time-series ma’lumotlar (Forex) uchun eng mos model
  - Uzoq muddatli pattern va trendlarni yaxshi o‘rganadi

## Model natijalari
- MAPE: ~1.14%
- Accuracy: ~98.86%
- Model real bozor ma’lumotida juda yuqori aniqlik beradi

## Vizual natija
- 30 kunlik real narx chizig‘i
- 30 kunlik predicted chiziq (oxirgi 7 kun — bashorat)

## shga tushirish
Notebookni oching datasetni google colabga yuklang va bloklarni ketma-ket ishga tushiring.
