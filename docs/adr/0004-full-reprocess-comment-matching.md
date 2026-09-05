# Full Reprocess for Comment Matching

Eksekusi pencocokan komentar (`POST /projects/:projectId/process-comments`) menghapus seluruh rekaman `comment_matches` sebelumnya untuk proyek terkait dan melakukan pemrosesan ulang secara penuh terhadap seluruh komentar aktif menggunakan regex word boundary in-memory pada runtime Bun. Keputusan ini diambil untuk menjamin idempSafe dan konsistensi penuh ketika kata kunci produk atau kata kunci permintaan ditambahkan, diubah, atau dihapus oleh pengguna.
