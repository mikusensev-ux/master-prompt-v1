# Prompt 2: Question Answering (Tanya Jawab Berbasis Konteks)

## Deskripsi
Prompt ini digunakan untuk menjawab pertanyaan berdasarkan konteks atau dokumen tertentu yang diberikan,
sehingga jawaban hanya bersumber dari informasi yang tersedia.

## Template Prompt

```
Kamu adalah asisten yang bertugas menjawab pertanyaan berdasarkan konteks yang diberikan.

Aturan:
1. Jawab HANYA berdasarkan informasi yang ada di dalam konteks.
2. Jika jawaban tidak ditemukan dalam konteks, katakan "Informasi tidak tersedia dalam konteks yang diberikan."
3. Berikan jawaban yang jelas, singkat, dan akurat.
4. Jangan menambahkan informasi dari luar konteks.

Konteks:
"""
{{konteks}}
"""

Pertanyaan: {{pertanyaan}}

Jawaban:
```

## Contoh Penggunaan

**Input:**
```
Konteks:
PT Maju Bersama didirikan pada tahun 2010 di Jakarta. Perusahaan ini bergerak di bidang
teknologi informasi dan telah melayani lebih dari 500 klien korporat. Pada tahun 2023,
perusahaan berhasil meraih penghargaan "Best IT Company" dari Asosiasi Teknologi Indonesia.
CEO perusahaan saat ini adalah Budi Santoso yang menjabat sejak 2018.

Pertanyaan: Siapa CEO PT Maju Bersama saat ini?
```

**Output yang Diharapkan:**
```
CEO PT Maju Bersama saat ini adalah Budi Santoso, yang menjabat sejak tahun 2018.
```

**Input (pertanyaan di luar konteks):**
```
Pertanyaan: Berapa jumlah karyawan PT Maju Bersama?
```

**Output yang Diharapkan:**
```
Informasi tidak tersedia dalam konteks yang diberikan.
```

## Tips
- Ganti `{{konteks}}` dengan dokumen, artikel, atau teks referensi Anda.
- Ganti `{{pertanyaan}}` dengan pertanyaan yang ingin dijawab.
- Prompt ini sangat berguna untuk aplikasi FAQ, customer service bot, atau sistem RAG (Retrieval-Augmented Generation).
- Tambahkan instruksi "berikan nomor halaman/paragraf sumber" jika ingin kutipan sumber yang lebih spesifik.
