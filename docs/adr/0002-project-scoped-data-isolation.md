# Project-Scoped Data Isolation

Entitas `YouTubeVideo`, `Comment`, `CandidateProduct`, `Criteria`, dan `CommentMatch` diisolasi sepenuhnya di bawah suatu `AnalysisProject` dengan aturan `ON DELETE CASCADE`. Keputusan ini diambil agar setiap sesi analisis/eksperimen dalam penelitian skripsi memiliki batasan data yang independen dan bersih, tanpa menimbulkan efek samping atau inkonsistensi data lintas proyek saat data dimodifikasi atau dihapus.
