# PostgreSQL with Drizzle ORM and postgres.js Driver

Backend menggunakan database PostgreSQL dengan Drizzle ORM dan driver `postgres.js` yang berjalan di atas Bun runtime, didukung oleh konfigurasi `docker-compose.yml` untuk lingkungan lokal. Keputusan ini diambil karena Drizzle ORM menyediakan type-safety penuh dengan overhead minimal, kompatibel sempurna dengan Bun, dan PostgreSQL menjamin integritas relasional serta kemampuan query analitik yang dibutuhkan dalam penelitian skripsi.
