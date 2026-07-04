# Output

Folder ini berisi seluruh hasil analisis yang dihasilkan dari implementasi metode **Latent Dirichlet Allocation (LDA)**, **Frequent Term-Based Clustering (FTC)**, dan **Social Network Analysis (SNA)** pada data tweet mengenai program **Makan Bergizi Gratis (MBG)**.

Seluruh file pada folder ini merupakan output yang dihasilkan secara otomatis selama proses analisis dan digunakan sebagai bahan evaluasi serta interpretasi hasil penelitian.

## Daftar Output

| Nama File | Deskripsi |
|-----------|-----------|
| **comments_preprocessed.csv** | Dataset hasil preprocessing yang telah melalui proses cleaning, tokenisasi, stopword removal, dan stemming. |
| **lda_input.txt** | Data teks yang telah diformat sebagai input untuk proses Topic Modeling menggunakan LDA. |
| **topic_words.csv** | Daftar kata-kata penting beserta probabilitasnya pada setiap topik hasil LDA. |
| **hasil_LDA.xlsx** | Hasil pemodelan topik menggunakan metode LDA yang berisi topik dominan setiap dokumen. |
| **FTC_MANUAL.xlsx** | Hasil proses clustering menggunakan metode Frequent Term-Based Clustering (FTC). |
| **ftc_selected_clusters.csv** | Informasi cluster yang dipilih berdasarkan frequent termset beserta nilai Entropy Overlap. |
| **cluster_summary.csv** | Ringkasan setiap cluster yang meliputi jumlah dokumen, topik dominan, kata kunci, dan contoh komentar. |
| **comment_topics_clusters.csv** | Hasil integrasi antara dokumen, topik hasil LDA, dan cluster hasil FTC. |
| **edges.csv** | Data hubungan (edge) antar akun Twitter berdasarkan mention yang digunakan pada analisis jaringan sosial. |
| **nodes.csv** | Daftar node (akun Twitter) yang terbentuk dari jaringan sosial. |
| **hasil_SNA.xlsx** | Hasil perhitungan ukuran Social Network Analysis seperti Degree, Betweenness, Closeness, dan Eigenvector Centrality. |
| **hasil_community_detection.xlsx** | Hasil identifikasi komunitas menggunakan algoritma Louvain. |
| **hasil_integrasi.xlsx** | Hasil integrasi Topic Modeling, Clustering FTC, dan Community Detection dalam satu dataset. |
| **hasil_interpretasi.xlsx** | Ringkasan interpretasi hasil analisis berdasarkan topik, cluster, dan komunitas yang terbentuk. |

## Ringkasan

Output yang dihasilkan pada folder ini digunakan untuk:
- Menganalisis topik pembahasan masyarakat mengenai program MBG.
- Mengelompokkan dokumen berdasarkan Frequent Term-Based Clustering (FTC).
- Menganalisis hubungan antar pengguna menggunakan Social Network Analysis (SNA).
- Mengidentifikasi komunitas dalam jaringan sosial menggunakan algoritma Louvain.
- Menyusun interpretasi akhir berdasarkan hasil integrasi seluruh metode.
