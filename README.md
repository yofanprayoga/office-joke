# Make the AI Judge Laugh: the Office Joke Open

[![make.fun](https://make.fun/badge/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232.svg)](https://make.fun/bounty/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232)
[![rank](https://make.fun/badge/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232/yofanprayoga/office-joke/rank.svg)](https://make.fun/bounty/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232)
[![reward](https://make.fun/badge/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232/yofanprayoga/office-joke/reward.svg)](https://make.fun/bounty/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232)

Bounty make.fun — $2, entry gratis, 1 tempat dibayar (pemenang ambil semua).
https://make.fun/bounty/u-aldy998-make-the-ai-judge-laugh-the-office-joke-open-9920f232

- Deadline final: Kamis 26 Nov 2026, 15.35 WIB
- Round 1 tutup: Rabu 25 Nov 2026, 07.33 WIB — kirim sebelum ini biar ikut dinilai di round 1
- Pendaftar: 136 agen per 15.46 WIB 24 Nov (paling sedikit di papan saat dicek)
- Hadiah: 1st $2

## Aturan inti

Satu lelucon kantor satu baris, maks 200 karakter, dan tidak ada yang lain.
Program menulis teks itu ke `/output/entry.txt` (UTF-8, 1–200 karakter,
bukan spasi doang). Juri AI membandingkan dua lelucon sekaligus dan memilih
yang lebih lucu. Yang menang: lelucon tentang kehidupan kantor, detailnya
spesifik (rapat yang harusnya email, reply-all, printer, kalender), ada
twist yang terbayar di kata-kata terakhir, dan segar.

## 3 opsi

### 1. I told my calendar I needed a break, so it booked me a meeting called 'Break' with eight attendees and a 47-slide deck. ⭐ rekomendasi
Paling kuat: detail kalender + rapat yang spesifik, twist-nya terbayar di
akhir (break malah jadi rapat 8 orang + 47 slide). Segar dan langsung
kebayang.

### 2. The printer only jams on urgent documents, which is why IT officially lists it as our most reliable deadline detector.
Printer ngadat + dokumen urgent, twist-nya printer malah jadi "pendeteksi
deadline". Spesifik dan relate banget buat anak kantor.

### 3. HR said bring your whole self to work, so I brought my laundry. Turns out 'whole self' has a dress code.
HR + dress code, twist di kata terakhir. Pendek dan bersih.

Semua opsi sudah dicek: di bawah 200 karakter, satu baris saja, tanpa teks lain.
Panjang terukur: Opsi 1 = 119 karakter, Opsi 2 = 118 karakter, Opsi 3 = 104 karakter.

## Cara pakai

```bash
python3 main.py                 # Opsi 1 (rekomendasi)
python3 main.py --option 2      # Opsi 2
python3 main.py --option 3      # Opsi 3
```

Lokal (tanpa akses ke `/output`):

```bash
OUTPUT_PATH=./output/entry.txt python3 main.py --option 1
cat output/entry.txt
```

`main.py` stdlib murni (cuma `os`, `sys`, `pathlib`), tanpa network.
Menulis tepat leluconnya saja ke `entry.txt`, tanpa newline di akhir, dan
gagal kalau lelucon kosong, lebih dari 200 karakter, atau bukan satu baris.

## Checklist submit (bukan cuma ketik lelucon)

1. Repo GitHub publik di satu commit (atau source bundle) berisi `main.py` ini.
2. Transkrip sesi agent yang membangunnya — wajib, tanpa ini entry tidak valid.
3. Sign-in dengan wallet Solana yang terhubung ke akun, wallet itu yang
   menandatangani entry dan menerima hadiah kalau menang.
4. Maks 5 submission per entrant per hari UTC. Entry final = submission
   terakhir yang ber-receipt sebelum deadline, kecuali pilih yang lebih awal.

## File

- `main.py` — program entry, stdlib murni
- `LICENSE` — MIT
