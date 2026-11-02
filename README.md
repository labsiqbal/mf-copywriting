# mf-copywriting

Skill untuk menulis konten bahasa Indonesia dan Inggris dengan suara yang natural, konteks yang jelas, dan klaim yang bisa dipertanggungjawabkan.

Natural tidak harus santai. Tulisan bisa tetap sopan, resmi, atau teknis tanpa terasa seperti terjemahan atau template promosi.

**Author:** Iqbal · **Versi:** 0.2.0 · **Status:** ready

## Apa yang dibantu?

- Memahami tujuan tulisan, pembaca, tempat terbit, dan bahan sebelum memilih struktur.
- Menyesuaikan bahasa dengan hubungan penulis dan pembaca, termasuk contoh tulisan yang disukai pengguna.
- Menulis artikel, landing page, sales copy, caption, email, WhatsApp, naskah video, dan slide presentasi.
- Menulis deskripsi repo, README, issue, PR, release notes, dan GitHub Discussions.
- Menjaga fakta, angka, harga, tenggat, tingkat kepastian, serta batas penawaran saat menyunting.
- Memisahkan teks untuk audiens dari catatan pengerjaan, instruksi pembuat, dan status prototipe berkas.
- Menilai taste editorial dengan enam dimensi berskala 1-10, terpisah dari pemeriksaan fakta dan format.
- Memperbarui referensi tren bahasa dan gaya komunikasi saat diminta.

Panduan Indonesia dan Inggris berada di folder terpisah. Bahasa hasil mengikuti brief. Untuk dokumen instruksi agent, panduan teknis lingkungan seperti `writing-for-agents` tetap mengatur struktur dan perilakunya.

## Mulai pakai

Clone seluruh repo agar panduan dan referensinya tetap tersedia:

```bash
git clone https://github.com/labsiqbal/mf-copywriting.git
```

Daftarkan atau tempatkan folder `mf-copywriting` di lokasi skill yang didukung agent Anda. Mekanisme instalasi dan aktivasi mengikuti harness masing-masing. Jika sudah ada instalasi, periksa sumbernya sebelum menggantinya.

Untuk mencoba tanpa instalasi, minta agent membaca `SKILL.md` dari folder hasil clone, lalu berikan tugas menulis. Pemilihan otomatis bergantung pada dukungan harness.

Contoh permintaan:

```text
Pakai mf-copywriting. Buat deskripsi GitHub untuk aplikasi pencatatan
pengeluaran. Pembacanya developer pemula. Fitur yang tersedia: input
pengeluaran manual dan ekspor CSV. Jangan mengklaim sinkronisasi bank.
```

```text
Pakai mf-copywriting. Tulis artikel tentang AI untuk kerja administrasi.
Saya belum punya pengalaman langsung atau sumber. Bantu riset dan bahas
sudut artikelnya dulu sebelum membuat draf atas nama saya.
```

```text
Pakai mf-copywriting. Rapikan email ini agar hangat dan langsung.
Pertahankan tanggal, jumlah pembayaran, dan janji yang sudah tertulis.
```

Skill memakai konteks yang sudah diberikan. Pertanyaan tambahan diperlukan saat jawabannya mengubah isi, klaim, atau arah tulisan.

## Belum punya pengalaman atau sumber?

Konten tetap bisa dimulai lewat riset. Agent mencari dan membaca sumber yang relevan, menjelaskan temuan serta batas buktinya, lalu mengajak pengguna menentukan pandangan atau kesimpulan.

Setelah arah jelas, agent menulis dengan atribusi dan citation dekat klaim terkait. Sumber tidak boleh diubah menjadi pengalaman pribadi pengguna. Jika pengguna menyerahkan pilihan sudut bahasan, agent dapat menulis penjelasan berbasis sumber tanpa mengatasnamakan keyakinan pribadi yang belum diberikan.

Riset internet membutuhkan akses sumber dan alat yang tersedia di lingkungan agent. Skill ini berisi instruksi kerja, bukan layanan pencarian atau scraper mandiri.

## Penilaian tulisan

Enam dimensi taste:

1. Relevansi bagi pembaca.
2. Ketajaman sudut pandang.
3. Suara yang terasa punya penulis.
4. Kenikmatan membaca.
5. Ketepatan takaran.
6. Kekuatan efek sesuai tujuan.

Skor memakai bilangan bulat 1-10, disertai kutipan dan alasan. Skor tidak dijumlahkan atau dirata-ratakan. Fakta yang salah tetap harus diperbaiki meskipun tulisan terasa enak dibaca. Pilihan pengguna menjadi acuan gaya dalam konteksnya.

## Update referensi saat dibutuhkan

```text
mf-copywriting-update. Perbarui referensi bahasa Indonesia untuk
caption Instagram di Indonesia selama 30 hari terakhir.
```

`mf-copywriting-update` adalah mode dalam skill yang sama. Riset mengamati bahasa, gaya komunikasi, dan pola copywriting sesuai cakupan. Tidak ada jadwal otomatis. Klaim tren memerlukan sumber bertanggal dan perbandingan yang sesuai; generasi pembaca tidak otomatis menentukan slang atau gaya.

## Isi repo

- [SKILL.md](SKILL.md): entrypoint dan pemilihan panduan.
- [id/panduan.md](id/panduan.md): panduan Indonesia.
- [en/guide.md](en/guide.md): English guide.
- [Jenis konten](id/references/format.md): panduan tiap format.
- [Brief dan diskusi sumber](id/references/brief.md): konteks sebelum menulis.
- [Penilaian taste](id/references/taste.md): ukuran editorial dan bukti penilaian.
- [Bahan uji](id/references/uji.md): contoh tugas dan pemeriksaan perilaku.
- [Update referensi](id/references/update.md): alur riset on demand.

## Status dan batas pengujian

Versi 0.2.0 siap dipakai untuk menyusun dan menyunting draf dengan pemeriksaan akhir. Alur riset, diskusi sumber, menunggu arah, dan melanjutkan penulisan telah diuji melalui agent terpisah serta review sumber. Ini belum membuktikan semua keluaran akurat, taste selalu konsisten, atau kualitas sama pada semua model dan harness.

`ready` menunjukkan kesiapan penggunaan berdasarkan cakupan uji. `released` memerlukan tag Git rilis yang sudah diverifikasi. Metadata versi dan author tersedia di `SKILL.md`.

## English

A bilingual writing skill for natural Indonesian and English copy. It covers briefs, format-specific writing, factual fidelity, source discussion, editorial taste, and on-demand language research. Start with [SKILL.md](SKILL.md) or the [English guide](en/guide.md).
