# UAS-Pembelajaran-Mesin-MBG
Analisis Topic Modeling Tweet MBG Menggunakan LDA, FTC dan Social Network Analysis
# Analisis Topik Tweet Makan Bergizi Gratis (MBG) Menggunakan LDA, FTC, dan Social Network Analysis

## Deskripsi Project

Project ini merupakan implementasi metode Topic Modeling menggunakan **Latent Dirichlet Allocation (LDA)** yang dikombinasikan dengan **Frequent Term-Based Clustering (FTC)** dan **Social Network Analysis (SNA)** untuk menganalisis percakapan masyarakat mengenai program **Makan Bergizi Gratis (MBG)** di media sosial X (Twitter).

Dataset diperoleh melalui proses crawling menggunakan Tweet Harvest dengan kata kunci:

```
makan bergizi gratis OR MBG
```

Sebanyak **500 tweet** digunakan sebagai data penelitian.

---

# Tujuan Penelitian

Penelitian ini bertujuan untuk:

- Mengumpulkan data tweet mengenai program MBG.
- Melakukan preprocessing data teks.
- Menemukan topik pembahasan menggunakan metode LDA.
- Mengelompokkan dokumen menggunakan FTC.
- Menganalisis hubungan antar akun menggunakan Social Network Analysis.
- Mengidentifikasi komunitas menggunakan algoritma Louvain.
- Mengintegrasikan hasil Topic Modeling, Clustering, dan Community Detection.

---

# Struktur Folder

```
├── Dataset
│   ├── MBG_2026.xlsx
│   ├── cleaned_text.csv
│
├── Source Code
│   └── uas_pembelajaran_mesin_topik_3_mbg2026.ipynb
│
├── Output
│   ├── hasil_LDA.xlsx
│   ├── comment_topics_clusters.csv
│   ├── topic_words.csv
│   ├── cluster_summary.csv
│   ├── ftc_selected_clusters.csv
│   ├── hasil_SNA.xlsx
│   ├── hasil_community_detection.xlsx
│   ├── hasil_integrasi.xlsx
│   └── hasil_interpretasi.xlsx
│
└── README.md
```

---

# Library yang Digunakan

Project ini menggunakan beberapa library Python berikut:

- pandas
- numpy
- gensim
- nltk
- Sastrawi
- scikit-learn
- matplotlib
- networkx
- python-louvain
- tweet-harvest
- Playwright

Install seluruh library menggunakan:

```bash
pip install pandas numpy gensim nltk sastrawi scikit-learn matplotlib networkx python-louvain
```

---

# Tahapan Penelitian

## 1. Crawling Data

Data tweet dikumpulkan menggunakan Tweet Harvest dengan kata kunci:

```
makan bergizi gratis OR MBG
```

Jumlah data yang digunakan sebanyak **500 tweet**.

---

## 2. Data Preprocessing

Tahapan preprocessing meliputi:

- Menghapus data duplikat
- Menghapus data kosong
- Case Folding
- Menghapus URL
- Menghapus Mention
- Menghapus Hashtag
- Menghapus Emoji
- Menghapus Angka
- Menghapus Tanda Baca
- Menghapus Spasi Berlebih
- Tokenizing
- Stopword Removal
- Stemming menggunakan Sastrawi

Output preprocessing disimpan pada:

```
cleaned_text.csv
```

---

## 3. Topic Modeling (LDA)

Metode Latent Dirichlet Allocation digunakan untuk menemukan topik utama dari kumpulan tweet.

Tahapan LDA:

- Membuat Dictionary
- Membuat Corpus Bag of Words
- Melatih Model LDA
- Menghasilkan distribusi topik
- Menentukan topik dominan setiap dokumen

Output:

- Topic Words
- Topic Probability
- Topic Dominan setiap Tweet

---

## 4. Frequent Term Based Clustering (FTC)

FTC digunakan untuk mengelompokkan tweet berdasarkan term yang sering muncul.

Tahapan:

- Membentuk Frequent Termset
- Menghitung Support
- Menghitung Entropy Overlap
- Membentuk Cluster

Output:

- Cluster Summary
- FTC Selected Cluster
- Comment Topic Cluster

---

## 5. Social Network Analysis (SNA)

SNA digunakan untuk mengetahui hubungan antar akun Twitter berdasarkan mention.

Tahapan:

- Membentuk Edges
- Membentuk Nodes
- Membuat Graph Network
- Menghitung:
  - Degree Centrality
  - Betweenness Centrality
  - Closeness Centrality
  - Eigenvector Centrality

Output:

```
hasil_SNA.xlsx
```

---

## 6. Community Detection

Community Detection dilakukan menggunakan algoritma Louvain.

Output:

```
hasil_community_detection.xlsx
```

---

## 7. Integrasi Hasil

Tahap akhir menggabungkan:

- Topic LDA
- Cluster FTC
- Community Detection

Sehingga setiap tweet memiliki informasi:

- Topic
- Cluster
- Community

---

# Cara Menjalankan Program

1. Download seluruh file repository.

2. Install seluruh library.

3. Buka project menggunakan Google Colab atau Jupyter Notebook.

4. Upload dataset:

```
MBG_2026.xlsx
```

5. Jalankan notebook dari sel pertama hingga terakhir secara berurutan.

6. Program akan menghasilkan berbagai file output pada folder Output.

---

# Output Program

Program menghasilkan beberapa file:

- cleaned_text.csv
- hasil_LDA.xlsx
- topic_words.csv
- comment_topics_clusters.csv
- cluster_summary.csv
- ftc_selected_clusters.csv
- hasil_SNA.xlsx
- hasil_community_detection.xlsx
- hasil_integrasi.xlsx
- hasil_interpretasi.xlsx

---

# Metode yang Digunakan

- Data Crawling
- Text Preprocessing
- Latent Dirichlet Allocation (LDA)
- Frequent Term-Based Clustering (FTC)
- Social Network Analysis
- Louvain Community Detection

---

# Penulis

Winni Nur Rahmawati (2411502020)

Adelia Zahwa Bilqist (2411502087)

Universitas Budi Luhur

2026
