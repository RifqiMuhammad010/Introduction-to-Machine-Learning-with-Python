# Introduction to Machine Learning with Python

Repositori ini memuat kumpulan catatan komprehensif, cuplikan kode implementasi, visualisasi data, serta ringkasan praktis yang diadaptasi dari buku **"Introduction to Machine Learning with Python: A Guide for Data Scientists"** karya Andreas C. Müller & Sarah Guido. 

[Tautan Buku Referensi](https://drive.google.com/file/d/1bitlEHE6Syb__5SUA7VOCVKGvzbhYpqO/view?usp=drive_link)

Proyek ini disusun khusus untuk mendukung pembelajaran mata kuliah *Machine Learning* (ML), dengan titik berat pada eksekusi kode secara langsung (praktikal) menggunakan pustaka `scikit-learn` di ekosistem Python.

---

## Ringkasan Materi per Bab (Chapter 1 - 8)

### Chapter 1: Pengenalan (Introduction)
* **Fokus Utama:** Konsep fundamental *machine learning* dan persiapan lingkungan kerja komputasi Python.
* **Topik Esensial:** Komparasi arsitektur *Supervised* dan *Unsupervised Learning*, pemanfaatan data historis, pengenalan pustaka inti (`NumPy`, `SciPy`, `pandas`, `matplotlib`, `scikit-learn`), serta eksekusi studi kasus perdana (klasifikasi spesies Iris menggunakan *k-Nearest Neighbors*).
* **Nilai Penting:** Membangun fondasi wajib terkait alur kerja ML—dimulai dari memuat dataset mentah, mempartisi data latih (*train*) dan data uji (*test*), hingga melakukan evaluasi model dasar.

### Chapter 2: Pembelajaran Terarah (Supervised Learning)
* **Fokus Utama:** Konstruksi model prediktif untuk menyelesaikan tugas Klasifikasi dan Regresi.
* **Topik Esensial:** Analisis masalah generalisasi, *overfitting*, dan *underfitting*. Eksplorasi mendalam algoritma klasik meliputi *k-NN*, Model Linier (Regresi Linier, *Ridge*, *Lasso*, Logistik), *Naive Bayes*, *Decision Trees*, metode *Ensemble* (*Random Forests*, *Gradient Boosting*), *Support Vector Machines* (SVM), hingga *Neural Networks* sederhana.
* **Nilai Penting:** Memberikan wawasan strategis untuk menentukan algoritma mana yang paling sesuai berdasarkan bentuk dataset, kecepatan komputasi, dan kebutuhan interpretasi model.

### Chapter 3: Pembelajaran Tanpa Pengawasan & Prapemrosesan (Unsupervised Learning and Preprocessing)
* **Fokus Utama:** Transformasi fitur pra-pemodelan dan pencarian pola laten pada data tanpa label.
* **Topik Esensial:** Teknik standardisasi dan penyelarasan rentang data (`MinMaxScaler`, `StandardScaler`). Reduksi dimensi untuk ekstraksi fitur dan visualisasi (*PCA*, *NMF*, *t-SNE*). Segmentasi ruang data melalui teknik *Clustering* (*k-Means*, *Agglomerative*, *DBSCAN*).
* **Nilai Penting:** Memastikan algoritma yang sangat sensitif terhadap jarak (seperti SVM) beroperasi maksimal tanpa bias skala, sekaligus memampatkan ukuran data dengan mempertahankan informasi esensialnya.

### Chapter 4: Representasi Data & Rekayasa Fitur (Representing Data and Engineering Features)
* **Fokus Utama:** Memanipulasi wujud data agar jauh lebih informatif saat dicerna oleh algoritma komputasi.
* **Topik Esensial:** Strategi konversi variabel kategorikal (*One-Hot Encoding*), penanganan angka yang bertindak sebagai label kelas, teknik *Binning* untuk fungsi non-linear, perluasan fitur via Interaksi dan Polinomial, serta normalisasi distribusi data miring menggunakan transformasi matematis.
* **Nilai Penting:** Menekankan prinsip bahwa kualitas rekayasa fitur sering kali menghasilkan lonjakan performa akurasi yang jauh lebih drastis dibandingkan sekadar menyetel hiperparameter algoritma.

### Chapter 5: Evaluasi & Peningkatan Model (Model Evaluation and Improvement)
* **Fokus Utama:** Metodologi pengujian ketahanan model yang ketat dan proses optimasi parameter otomatis.
* **Topik Esensial:** Implementasi validasi silang (*Cross-Validation*, *Stratified k-Fold*) untuk stabilitas pengujian, pencarian parameter masif menggunakan *Grid Search* (`GridSearchCV`), serta penggunaan metrik evaluasi tingkat lanjut (*Precision*, *Recall*, *F1-score*, kurva *ROC*, skor *AUC*, *MSE*, koefisien R-Squared).
* **Nilai Penting:** Menghindari bias ilusi performa akibat evaluasi yang salah sasaran, dan memastikan keandalan prediksi model saat diterjunkan ke dalam skenario dunia nyata.

### Chapter 6: Rantai Algoritma & Pipeline (Algorithm Chains and Pipelines)
* **Fokus Utama:** Unifikasi seluruh tahapan pemrosesan data dan pemodelan ke dalam satu alur kerja tunggal.
* **Topik Esensial:** Pemanfaatan objek `Pipeline` di `scikit-learn`, strategi mutlak untuk menghindari kebocoran informasi (*data leakage*) selama validasi silang, dan pelaksanaan *Grid Search* secara simultan untuk setiap tahapan *preprocessing* dan estimator.
* **Nilai Penting:** Menjaga kebersihan dan skalabilitas arsitektur kode di level produksi, serta mencegah anomali teknis di mana data uji secara diam-diam mengontaminasi kalkulasi parameter pada data latih.

### Chapter 7: Pemrosesan Data Teks (Working with Text Data)
* **Fokus Utama:** Dasar Pemrosesan Bahasa Alami (*NLP*) untuk mengubah string linguistik menjadi masukan terstruktur.
* **Topik Esensial:** Konstruksi representasi *Bag-of-Words* (BoW), tokenisasi teks, perhitungan frekuensi (`CountVectorizer`), pembobotan kata penting berbasis dokumen (*TF-IDF Scaling*), filtrasi kata hubung (*stop words*), ekstraksi konteks *n-grams*, serta aplikasi end-to-end pada Analisis Sentimen.
* **Nilai Penting:** Mengonversi data tak terstruktur berupa teks bebas menjadi representasi matriks jarang (*sparse matrix*) yang efisien secara memori agar dapat dipelajari oleh model *machine learning*.

### Chapter 8: Kesimpulan & Implementasi Industri (Wrapping Up)
* **Fokus Utama:** Strategi manajerial dan konseptual dalam mengeksekusi proyek *machine learning* dari awal hingga akhir.
* **Topik Esensial:** Menerjemahkan kebutuhan bisnis menjadi format metrik ML, mengukur kelayakan kualitas data, perancangan model *baseline*, transisi dari lingkungan purwarupa (*prototype*) menuju lingkungan produksi (*production*), A/B *Testing*, serta arahan pengembangan untuk komputasi skala masif.
* **Nilai Penting:** Memberikan peta jalan (*roadmap*) realistis tentang posisi seorang *Data Scientist* atau *Engineer* di industri nyata, di mana memahami domain masalah dan cara mengomunikasikan hasil jauh lebih krusial dibandingkan sekadar merangkai algoritma.
