# YouTube oEmbed First for Video Metadata

Saat pengguna mendaftarkan URL video YouTube, metadata awal (judul video, nama pemilik/channel, thumbnail) diambil melalui endpoint publik YouTube oEmbed (`https://www.youtube.com/oembed`) tanpa menggunakan kuota YouTube Data API v3. Pemanggilan YouTube Data API v3 hanya dilakukan ketika proses *Fetch Comments* secara eksplisit dijalankan. Keputusan ini diambil untuk menghemat kuota harian API Google (0 kuota terpakai saat input video) serta menjaga fungsionalitas preview video saat API key belum disetel.
