# USD/CHF Forex Price Forecasting (LSTM)

Ushbu loyiha USD/CHF valyuta juftligining kelgusi narxlarini AI yordamida bashorat qilish uchun yaratilgan. 
Model 2005–2024 yillar orasidagi tarixiy ma'lumotlar asosida 7 kunlik kelajak narxlarini prognoz qiladi.

##  Loyihaning maqsadi
- Forex bozoridagi USD/CHF narx harakatini tahlil qilish
- 60 kunlik tarixiy ma’lumotdan foydalanib 7 kunlik kelajak narxini bashorat qilish
- Real va bashorat qilingan narxlarni grafikda taqqoslab ko‘rsatish
- Model aniqligini (MAE, RMSE, MAPE, Accuracy) hisoblash

##  Model haqida
- Model arxitekturasi: 2 qatlamli LSTM + Dropout + Dense(7)
- 60 kunlik input → 7 kunlik forecast
- Nega LSTM?
  - Time-series (ketma-ket) ma’lumotlar uchun eng mos
  - Uzoq muddatli bog‘lanishlarni yaxshi o‘rganadi
  - Forex kabi tebranuvchan bozorlarni bashoratlashda yuqori natija beradi

##  Model natijalari
- MAE: ~0.0092  
- RMSE: ~0.0097  
- MAPE: ~1.14%  
- Accuracy: ~98.86%  

Model forex bozorida juda yuqori aniqlikda ishlaydi.

##  Vizual natijalar
- 30 kunlik REAL narx chizig‘i
- 30 kunlik PREDICTED chizig‘i
  - Oxirgi 7 kun — model bashorati (qizil rangda)

##  Ishga tushirish
Notebookni oching va kod bloklarini ketma-ket ishga tushiring.

---

## 🛠 Ishlatilgan texnologiyalar

###  Dasturlash
- Python 3.x

###  Kutubxonalar
- **Pandas** — ma’lumotlarni tozalash va tahlil
- **NumPy** — matematik amallar
- **Matplotlib** — grafiklar
- **scikit-learn**
  - MinMaxScaler (scaling)
  - Metrics (MAE, RMSE, MAPE)
- **TensorFlow / Keras**
  - LSTM
  - Dropout
  - Dense

###  Qo‘shimcha indikatorlar
- **MA10** — 10 kunlik o‘rtacha narx
- **RSI14** — momentum indikatori

