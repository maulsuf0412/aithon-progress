# AITHON Progress Calendar

Halaman progress persiapan **AITHON** — seminar internal UKM UNTIRTA Digital Creative
bersama Google Student Ambassador, 19 September 2026.

🔗 **https://maulsuf0412.github.io/aithon-progress/**

## Isi halaman

| Tab | Isi |
| --- | --- |
| Overview | Roadmap enam checkpoint, 18 Agustus – 19 September 2026 |
| Kalender | Kalender Agustus & September dalam satu tampilan, geser pakai panah ‹ › |
| Final & Hari-H | Checklist ketupel yang menggerakkan progress bar di header |
| Rundown | Susunan acara 08.50–12.45 WIB |
| Anggaran | RAB yang dibaca langsung dari Google Sheets |
| Tentang AITHON | Profil kegiatan dan pemateri |
| Progress Rapat | Target tiap rapat beserta checklist per divisi |
| Struktur & Tugas | Pembagian tugas tiap divisi |

## Anggaran diambil dari mana

Tab Anggaran membaca [spreadsheet RAB](https://docs.google.com/spreadsheets/d/1AtMls0gO6CUwhryH-jxHwV8LGNQi1BqaDcGK7yLFH5s/edit)
lewat endpoint CSV Google Sheets setiap kali halaman dibuka, jadi hasil isian Benplak
langsung tampil tanpa perlu deploy ulang. Statusnya ditandai di atas tabel:

- **Tersambung • HH.MM** — angka baru saja dibaca dari spreadsheet.
- **Salinan <tanggal>** — spreadsheet tidak terbaca, yang tampil salinan terakhir yang ikut di-commit.

Syaratnya spreadsheet tetap dibagikan sebagai *"siapa saja yang memiliki link"*. Kalau
aksesnya diubah jadi terbatas, halaman otomatis jatuh ke salinan dan tidak pernah tampil kosong.

Sub-total dan grand total dihitung ulang dari isi item, jadi rumus di sheet yang belum
ter-update tidak diam-diam menampilkan angka yang salah.

## Catatan teknis

`index.html` berdiri sendiri — tidak ada build step, tidak ada dependensi, tidak ada
permintaan ke CDN. Font Poppins dan seluruh gambar disematkan sebagai data URI supaya
halaman tetap utuh walau jaringan sedang buruk.
