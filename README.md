# 📊 Naive Bayes Classification

Nama: Moch Rifky Aulia Adikusumah

NIM: 1227050072

Kelas: Prak. Pembelajaran Mesin E

Proyek ini merupakan implementasi algoritma klasifikasi **Naive Bayes** untuk memprediksi apakah seseorang akan membeli komputer berdasarkan fitur-fitur seperti usia, pendapatan, status mahasiswa, dan peringkat kredit.

## 🗂️ Dataset
Dataset yang digunakan adalah `dataset_buys_comp.csv`, berisi atribut:
- `Age`
- `Income`
- `Student`
- `Credit_Rating`
- `Buys_Computer` (label target)

## 🛠️ Tahapan dan Langkah-langkah

1. **Import Library**  
   Mengimpor library Python yang digunakan untuk memproses data, visualisasi, membangun model machine learning, dan evaluasi performa.

2. **Load Dataset**  
   Membaca data dari file CSV dan memuatnya ke dalam DataFrame untuk dianalisis lebih lanjut.

3. **Eksplorasi Data**  
   Melakukan pemeriksaan struktur data, statistik deskriptif, serta melihat distribusi label target untuk memahami karakteristik data.

4. **Visualisasi Distribusi Fitur**  
   Menampilkan grafik distribusi dari fitur-fitur kategorikal terhadap label target untuk mengidentifikasi pola yang mungkin berguna dalam pemodelan.

5. **Preprocessing (Label Encoding)**  
   Mengubah data kategorikal menjadi data numerik agar bisa digunakan oleh algoritma machine learning.

6. **Split Data**  
   Membagi dataset menjadi dua bagian: data latih (80%) dan data uji (20%) untuk melatih dan menguji performa model.

7. **Training Model**  
   Melatih model klasifikasi Gaussian Naive Bayes menggunakan data latih yang sudah diproses.

8. **Prediksi dan Evaluasi**  
   Melakukan prediksi pada data uji, kemudian mengevaluasi performa model dengan metrik seperti akurasi, confusion matrix, dan classification report.

## 📌 Hasil

Model berhasil melakukan klasifikasi dengan akurasi tertentu (lihat output evaluasi). Hasil evaluasi meliputi:
- Akurasi model
- Confusion matrix
- Precision, recall, dan f1-score untuk setiap kelas

---

✅ **Kesimpulan**

Berdasarkan hasil evaluasi model Gaussian Naive Bayes:

- **Akurasinya** mencapai 74%, yang berarti model mampu mengklasifikasikan 74 dari 100 data uji dengan benar.
- Model memiliki **precision** tinggi untuk kelas 'Tidak Layak' (0.76), namun **recall-nya** rendah (0.39), menandakan masih banyak data kelas 'Tidak Layak' yang salah diklasifikasikan sebagai 'Layak'.
- Sebaliknya, kelas 'Layak' memiliki **recall** tinggi (0.93), menunjukkan bahwa model cukup andal dalam mendeteksi pengguna yang layak membeli komputer.
- Nilai **macro average recall** sebesar 0.66 mengindikasikan bahwa terdapat ketidakseimbangan performa antar kelas, dan bisa ditingkatkan dengan pendekatan balancing dataset atau teknik boosting.
