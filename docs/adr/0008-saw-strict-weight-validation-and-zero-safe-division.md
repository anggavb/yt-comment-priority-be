# Strict SAW Weight Validation and Zero-Safe Division

Backend menerapkan validasi ketat bahwa total bobot kriteria $\sum w_j = 1.0$ (dengan toleransi float $\pm 0.001$), dan menolak proses perhitungan dengan `400 Bad Request` jika tidak terpenuhi. Selain itu, jika nilai maksimum seluruh alternatif pada suatu kriteria adalah nol ($\max(x_{ij}) = 0$), nilai ternormalisasi ditetapkan $r_{ij} = 0$. Keputusan ini diambil untuk memastikan integritas metodologi penelitian skripsi dan mencegah kesalahan kalkulasi matematis (*division by zero* / `NaN`).
