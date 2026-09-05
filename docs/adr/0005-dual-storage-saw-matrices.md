# Dual Storage for SAW Calculation Results

Hasil perhitungan metode SAW disimpan dalam dua bentuk: tabel relasional terstruktur `ranking_results` untuk query cepat per produk/peringkat, dan kolom snapshot JSON (`calculation_snapshot`) pada tingkat proyek yang merekam matriks keputusan ($X$), matriks ternormalisasi ($R$), matriks terbobot ($W \times R$), bobot kriteria, konfigurasi C4, dan timestamp. Keputusan ini diambil untuk memenuhi kebutuhan transparansi dan auditabilitas matematis skripsi tanpa terpengaruh oleh mutasi data di masa depan.
