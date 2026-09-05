# In-Process Async Fetch with Mock Fallback

Pengambilan komentar YouTube dari YouTube Data API v3 dijalankan secara asinkron in-process (status `PENDING` -> `FETCHING` -> `COMPLETED` / `FAILED`) dengan dukungan pembatasan `maxComments` dan mekanisme mock/fixture fallback ketika API key tidak disetel atau kuota harian habis. Keputusan ini diambil untuk menghindari HTTP timeout pada request client tanpa memerlukan infrastruktur message queue eksternal, serta menjamin sistem tetap dapat didemokan dan diuji secara offline saat sidang skripsi.
