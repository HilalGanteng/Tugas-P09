# Debug Log - Sprint 2

## Bug 1: Timer tidak berjalan
- **Branch**: `fix/perbaikan-timer-tidak-berjalan`
- **Masalah**: Timer tidak mau berjalan saat tombol *start* diklik pertama kali.
- **Penyebab**: Fungsi `startTimer()` terpanggil sebelum elemen DOM sepenuhnya siap atau status `isRunning` belum diinisialisasi dengan benar.
- **Solusi**: Menambahkan pengecekan kondisi status `isRunning` dan memastikan *event listener* terikat dengan benar pada fungsi *start*.

## Bug 2: Interaksi Tombol Timer
- **Branch**: `fix/Tombol-timer`
- **Masalah**: Responsivitas klik pada tombol kontrol timer sempat tertunda.
- **Penyebab**: Kurangnya optimalisasi pemanggilan fungsi *event listener* pada skrip utama tombol kontrol.
- **Solusi**: Merapikan struktur fungsi JavaScript dan memastikan penanganan klik tombol merespons secara langsung tanpa jeda.