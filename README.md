# AlphaGroup_JC_DS_FT_BDG_03_FinalProject

Proyek ini melibatkan analisis dataset bernama `bank-additional-full.csv` yang berisi informasi tentang berbagai klien dari sebuah bank. Dataset ini mencakup rincian seperti usia, pekerjaan, status pernikahan, pendidikan, dan faktor sosial-ekonomi lainnya. Tujuan utama dari analisis ini adalah untuk mengeksplorasi data dan mendapatkan wawasan yang dapat membantu memahami perilaku dan preferensi klien, khususnya dalam melakukan deposito di bank tersebut.

## Stakeholder
Data ini ditujukan untuk:
- Chief Marketing Officer (CMO)
- Chief Financial Officer (CFO)
- Chief Risk Officer (CRO)
- Customer Relationship Managers (CRM)
- Head of Retail Banking

## Deskripsi Dataset
Dataset ini terdiri dari 22 kolom dan mencakup informasi berikut:
- `age`: Usia klien.
- `job`: Jenis pekerjaan (misalnya, admin, services).
- `marital`: Status pernikahan (misalnya, married, single).
- `education`: Tingkat pendidikan.
- `default`: Apakah klien memiliki kredit macet (yes atau no).
- `housing`: Apakah klien memiliki pinjaman perumahan (yes atau no).
- `loan`: Apakah klien memiliki pinjaman pribadi (yes atau no).
- `contact`: Jenis kontak komunikasi (misalnya, cellular, telephone).
- `month`: Bulan terakhir kontak dalam setahun.
- `day_of_week`: Hari terakhir kontak dalam seminggu.
- `duration`: Durasi kontak terakhir, dalam detik.
- `campaign`: Jumlah kontak yang dilakukan selama kampanye ini.
- `pdays`: Jumlah hari sejak klien terakhir dihubungi dari kampanye sebelumnya.
- `previous`: Jumlah kontak yang dilakukan sebelum kampanye ini.
- `poutcome`: Hasil dari kampanye pemasaran sebelumnya (misalnya, success, failure).
- `emp.var.rate`: Tingkat variasi pekerjaan.
- `cons.price.idx`: Indeks harga konsumen.
- `cons.conf.idx`: Indeks kepercayaan konsumen.
- `euribor3m`: Suku bunga Euribor 3 bulan.
- `nr.employed`: Jumlah karyawan.
- `deposit`: Apakah klien telah berlangganan deposito berjangka (yes atau no).
- `age group`: Kelompok umur yang dikategorikan.
- `deposit_numeric`: Representasi numerik dari langganan deposito (1 untuk yes, 0 untuk no).


## Algoritma Machine Learning yang Digunakan
Untuk memprediksi apakah seorang klien akan berlangganan deposito berjangka, berbagai model machine learning diterapkan dan dilatih menggunakan data pelatihan. Model yang akan dievaluasi meliputi:

### Model Sederhana:
- Logistic Regression
- Decision Tree Classifier
- K-Nearest Neighbors (KNN) Classifier

### Model Ensemble:
- Random Forest Classifier
- Gradient Boosting Classifier
- Extreme Gradient Boosting (XGBoost) Classifier
- Adaptive Boosting (AdaBoost)
- Light Gradient Boosting Machine (LightGBM)

## Metrik Evaluasi
Model dievaluasi menggunakan metrik evaluasi yang relevan:
- **Recall**: Mengukur proporsi prediksi positif yang benar dari total kasus positif yang sebenarnya. Penting untuk meminimalkan False Negatives.

## Panduan Pengguna
Untuk menjalankan analisis ini, pastikan Anda telah menginstal:
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## File (.sav)
pickle.dump(final_model, open('campaign_model_lgbm.sav', 'wb'))

## Tableau
Link: [Bank Marketing Campaign Portugal](https://public.tableau.com/views/BankMarketingCampaignPortugal/Summary?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
