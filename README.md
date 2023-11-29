# Proyek Akhir Analisis Data: Bike Sharing dan Dashboard
# Analisis dilakukan di Google Collaboratory
Proyek Akhir Analisis Data Bike Sharing dapat dilihat selengkapnya di tautan berikut <a href='https://github.com/adinplb/Proyek_Analisis_Data_Dicoding/blob/main/notebook.ipynb'>Bike Sharing Analysis</a>

## Mendefinisikan Pertanyaan
1. Berapa jumlah total sewa sepeda (cnt) untuk tahun 2011 selama musim panas (musim 2)?
2. Berapa banyak sepeda sewaan yang digunakan pada hari kerja (weekday = 0) selama musim gugur (musim 3) pada tahun 2012?

# Menyiapkan Semua Library Yang Dibutuhkan
- import pandas as pd
- import plotly.express as px
- import warnings

## Data Wrangling:
- Gathering data
- Assessing data (Cek Tipe Data, Cek Missing Value, Cek Duplikasi Data, Deskripsif Statistics)
- Cleaning data

## Exploratory Data Analysis (Insights and Findings):
1. Dataset bike_day
- Jumlah data: 731 entri
- Musim paling umum: Musim panas (season 2).
- Tahun yang dominan: 2012 (yr = 1)
- Bulan yang paling sering muncul: Juli (mnth 7)
- Hari libur hanya ada sekitar 2.87% dari total hari
- Hari kerja adalah mayoritas (sekitar 68.40%)
- Cuaca rata-rata pada keadaan yang baik (weathersit 1)
- Suhu rata-rata adalah sekitar 0.50 (41°C), dengan suhu perasaan rata-rata sekitar 0.47 (50°C)
- Kelembaban rata-rata sekitar 0.47 (47%).
- Kecepatan angin rata-rata adalah sekitar 0.63 (67% dari maksimal)
- Jumlah pengguna casual rata-rata sekitar 848.
- Jumlah pengguna terdaftar rata-rata sekitar 3656.
- Total rental rata-rata sekitar 4504 per hari

2. Dataset bike_hour
- Dataset terdiri dari 17,379 entri.
- Rata-rata kolom-kolom utama adalah sekitar:
- Musim (season) 2.50, menunjukkan musim rata-rata.
- Tahun (yr) 0.50, mengindikasikan perbandingan antara tahun 2011 dan 2012.
- Bulan (mnth) 6.54, menunjukkan bulan rata-rata dalam setahun.
- Jam (hr) 11.55, mengindikasikan jam rata-rata dalam sehari.
- Hari libur (holiday) 0.03, persentase hari libur.
- Hari dalam seminggu (weekday) 3.00, hari rata-rata dalam seminggu.
- Hari kerja (workingday) 0.68, persentase hari kerja.
- Kondisi cuaca (weathersit) 1.43, kondisi cuaca rata-rata.
- Suhu (temp) 0.50, suhu rata-rata yang normal.
- Suhu perasaan (atemp) 0.48, suhu perasaan mendekati suhu sebenarnya.
- Kelembaban (hum) 0.48, kelembaban rata-rata.
- Kecepatan angin (windspeed) 0.63, kecepatan angin rata-rata.
- Pengguna casual (casual) 35.68, rata-rata jumlah pengguna casual.
- Pengguna terdaftar (registered) 153.79, rata-rata jumlah pengguna terdaftar.
- Total rental sepeda (cnt) 189.46, rata-rata jumlah total rental sepeda.

## Visualization and Explanatory Analysis:
- Jumlah total sewa sepeda untuk tahun 2011 selama musim manas (musim 2): 347316
- Jumlah total sepeda sewaan yang digunakan pada hari kerja selama musim gugur pada tahun 2012: 186115

# Dashboard with Streamlit:
## Run Streamlit on Local
### Intall Dependencies
To install all the required libraries, open your terminal/command prompt/conda prompt, navigate to this project folder, and run the following command:
`pip install -r requirements.txt`
`pip install streamlit`

### Run Dashboard
Mengarahkan pathnya ke direktori file py dan dataset hour.csv nya dengan command `cd dashboard` pada Anaconda Prompt

Setelah berhasil, tuliskan perintah berikut `streamlit run dashboard_streamlit_muhammad_adin_palimbani.py` untuk mendapatkan link localhostnya 
