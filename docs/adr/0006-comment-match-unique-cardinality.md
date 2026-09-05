# Unique Constraint on Comment Match per Product

Tabel `comment_matches` menerapkan batasan unik `UNIQUE(comment_id, product_id)`. Jika sebuah komentar memuat beberapa kata kunci dari produk yang sama, sistem memilih kata kunci terpanjang yang cocok untuk dicatat. Keputusan ini diambil untuk mencegah terjadinya penghitungan ganda (*double counting*) pada kriteria C1 (Request Count) dan C2 (Unique Requester) jika satu komentar mengulang nama produk berkali-kali.
