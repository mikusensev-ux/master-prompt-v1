# Prompt 1: Summarization (Ringkasan Teks)

## Deskripsi
Prompt ini digunakan untuk meringkas teks panjang menjadi poin-poin utama yang singkat dan mudah dipahami.

## Template Prompt

```
Kamu adalah asisten yang ahli dalam meringkas teks.

Bacalah teks berikut dengan seksama, lalu buat ringkasan yang mencakup:
- Ide utama
- Poin-poin penting
- Kesimpulan

Teks:
"""
{{teks_input}}
"""

Berikan ringkasan dalam maksimal 3 paragraf dengan bahasa yang jelas dan mudah dipahami.
```

## Contoh Penggunaan

**Input:**
```
Teks: Perubahan iklim adalah fenomena jangka panjang yang mempengaruhi pola cuaca global.
Aktivitas manusia seperti pembakaran bahan bakar fosil dan deforestasi menghasilkan gas rumah kaca
yang memerangkap panas di atmosfer. Dampaknya meliputi kenaikan suhu rata-rata bumi, mencairnya
es di kutub, naiknya permukaan laut, serta cuaca ekstrem yang semakin sering terjadi.
Para ilmuwan menyerukan pengurangan emisi karbon secara drastis sebagai langkah utama
untuk membatasi dampak paling parah dari perubahan iklim.
```

**Output yang Diharapkan:**
```
Perubahan iklim disebabkan oleh aktivitas manusia yang menghasilkan gas rumah kaca, terutama
dari pembakaran bahan bakar fosil dan deforestasi. Gas-gas ini memerangkap panas di atmosfer
dan memicu pemanasan global.

Dampak yang ditimbulkan sangat luas, mulai dari mencairnya es kutub, naiknya permukaan laut,
hingga cuaca ekstrem yang semakin sering terjadi di berbagai penjuru dunia.

Para ilmuwan menekankan bahwa pengurangan emisi karbon secara signifikan adalah solusi kunci
untuk mencegah dampak terburuk dari perubahan iklim ini.
```

## Tips
- Ganti `{{teks_input}}` dengan teks yang ingin diringkas.
- Sesuaikan jumlah paragraf sesuai kebutuhan.
- Bisa ditambahkan instruksi seperti "gunakan poin-poin" atau "gunakan tabel" untuk format yang berbeda.
