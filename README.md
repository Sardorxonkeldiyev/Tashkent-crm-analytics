# 🏗️ Tashkent CRM Data Analytics Project

[O'zbekcha va Inglizcha sodda qo'llanma / Simple guide in Uzbek and English]

---

## 🇺🇿 O'zbek Tili (Uzbek Language)

### 📌 Loyiha haqida
Bu loyiha Toshkentdagi yirik qurilish kompaniyasi uchun tayyorlangan Ma'lumotlar Analitikasi (Data Analytics) tizimidir. Kompaniyaning Google Drive va Excel jadvallaridagi savdo ma'lumotlari avtomatlashtirilib, rahbarlar uchun qulay va jonli dashboard (Power BI) holatiga keltirildi.

### 🛠️ Ishlatilgan texnologiyalar
* **Google Drive & Excel:** Ma'lumotlarni saqlash va kiritish uchun.
* **Python (Pandas):** Excel jadvallarni avtomatik birlashtirish va xatolarini tozalash uchun.
* **Power BI:** Interaktiv grafiklar va hisobotlar yaratish uchun.

### 📊 Dashboard sahifalari
1. **Shartnomalar sahifasi:** Jami kelib tushgan pullar, debetorlik qarzlari, sotilgan maydon hajmi va qaysi reklama kanali yaxshi ishlayotganini koʻrsatadi.
2. **Mijozlar sahifasi:** Har bir mijozning qarzi va loyihalar kesimidagi moliyaviy holatni batafsil tahlil qiladi.

---

## 🇬🇧 English (Ingliz Tili)

### 📌 About the Project
This project is a Data Analytics solution built for a major real estate and construction company in Tashkent. It automates raw sales data stored in Google Drive and Excel, turning messy spreadsheets into live, interactive Power BI dashboards for executive decision-making.

### 🛠️ Technologies Used
* **Google Drive & Excel:** For data input and storage.
* **Python (Pandas):** For automatic data merging and data cleaning.
* **Power BI:** For creating interactive charts and business dashboards.

### 📊 Dashboard Pages
1. **Contracts Page (Shartnomalar):** Tracks total revenue, accounts receivable, total square meters sold, and marketing channel performance.
2. **Clients Page (Mijozlar):** Provides detailed analysis of client debts and specific financial states of construction projects.

---

```python
import pandas as pd

# Automated data cleaning pipeline for Excel sheets
df = pd.read_excel("data/Tashkent_CRM_online_project.xlsx")

# Structural cleaning & handling string errors in numeric columns
df['Jami_Qiymati_USD'] = pd.to_numeric(df['Jami_Qiymati_USD'], errors='coerce').fillna(0)
print("Data pipeline status: 200 OK. Cleaned successfully.")

```
---

## 📸 Screenshots (Rasmlar)

### 1. Shartnomalar / Contracts
<img width="1270" height="695" alt="Tashkent_CRM2" src="https://github.com/user-attachments/assets/14bf5e87-b8fb-4527-8c46-2c18f0219936" />


### 2. Mijozlar / Clients
<img width="1275" height="716" alt="Tashkent_CRM_Mijozlar" src="https://github.com/user-attachments/assets/d1f71275-4ec1-4e71-8d42-55570e3d30e0" />
