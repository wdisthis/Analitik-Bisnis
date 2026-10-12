# Panduan Belajar Kuis — Analitik Bisnis

Isi file ini:
- **Bagian A** — Diagnostic Business Analysis & Root Cause Analysis (kasus: PT Nusantara Segar Retail)
- **Bagian B** — SOAR & SWOT Business Analysis Framework (kasus: Ayam Geprek & PT Kopi Nusa Rasa)
- **Bagian C** — Cheat sheet + latihan soal dengan jawaban

> Tips: kuis kemungkinan besar berbentuk studi kasus. Jadi jangan hanya hafal definisi. Latih juga **menghitung angka** dan **menentukan posisi sebuah pernyataan** (finding/cause, kuadran SWOT, tahap SOAR, dst.).

---

# BAGIAN A — DIAGNOSTIC BUSINESS ANALYSIS & ROOT CAUSE ANALYSIS

Tema inti: **membedakan finding dari cause, dan evidence dari assumption.**

## A1. Empat Tingkat Analitik

| No | Tingkat | Pertanyaan | Isi | Hasil |
|---|---|---|---|---|
| 1 | **Descriptive** | Apa yang terjadi? | Laporan, dashboard, KPI | **Finding** |
| 2 | **Diagnostic** | Mengapa terjadi? | Drill-down, bukti, uji kausal | **Cause** |
| 3 | **Predictive** | Apa yang akan terjadi? | Model peramalan berbasis pola historis | — |
| 4 | **Prescriptive** | Apa yang sebaiknya dilakukan? | Optimasi, simulasi, rekomendasi keputusan | — |

- Tingkat diagnostik adalah tingkat **yang paling sering dilewati**.
- Kalimat kunci: *"Dashboard yang bagus berhenti di 'apa'. Analis yang bagus melanjutkan ke 'mengapa' dan sanggup membuktikannya."*

## A2. Definisi Analisis Diagnostik

**Proses sistematis untuk menjelaskan mengapa sebuah angka bergerak, dengan menelusuri data sampai ditemukan penyebab yang didukung bukti dan dapat ditindaklanjuti.**

Tiga syarat (kalau tidak terpenuhi, itu bukan diagnosis, tetapi "narasi yang kebetulan disertai angka"):
1. **Sistematis, bukan intuitif**: jalurnya sama setiap kali (masalah → dimensi → bukti), sehingga bisa diperiksa orang lain.
2. **Berbasis bukti**: setiap klaim penyebab bisa ditunjuk ke data tertentu, bukan keyakinan atau pengalaman pribadi.
3. **Dapat ditindaklanjuti**: penyebab menunjuk pada keputusan atau proses yang bisa diubah perusahaan.

**Pertanyaan kunci sesi:** *"Apa bukti bahwa sesuatu benar-benar merupakan penyebab?"*

## A3. Finding vs Cause

| | **Finding (Temuan)** | **Cause (Penyebab)** |
|---|---|---|
| Menjawab | **APA** yang terjadi | **MENGAPA** hal itu terjadi |
| Sifat | Deskriptif: melaporkan keadaan atau perubahan angka | Eksplanatif: menjelaskan mekanisme di balik angka |
| Sumber | Langsung dari data tanpa interpretasi | Menyebut dimensi spesifik (produk, wilayah, segmen, periode) |
| Mekanisme | Tidak menjelaskan mekanisme apa pun | Menunjuk pemicu yang bisa diverifikasi data |
| Tindak lanjut | Tidak bisa ditindaklanjuti | Bisa ditindaklanjuti, mengarah ke keputusan yang bisa diubah |
| Contoh | "Sales turun 20%." | "Penurunan sales terutama berasal dari Produk A di Region X setelah perubahan pricing." |

### Jalur dari finding ke cause (bukan lompatan intuisi)
1. **FINDING**: "Sales turun 20%." (benar, tapi tidak berguna untuk keputusan)
2. **PERTANYAAN**: "Turunnya di mana, produk apa, wilayah mana, sejak kapan?"
3. **BUKTI**: Produk A di Region X menyumbang **54%** dari total penurunan; volume turun **64%** sejak 1 Juli.
4. **CAUSE**: Penurunan sales terutama berasal dari Produk A di Region X setelah **perubahan pricing 1 Juli**.

**Aturan praktis:** kalau sebuah kalimat tidak memuat kata "karena" **atau** tidak menyebut dimensi spesifik, kemungkinan besar itu masih finding.

### Pasangan finding → cause (dari slide)
| Finding | Cause |
|---|---|
| Sales turun 20% pada Q3 | 54% penurunan berasal dari Produk A di Region X setelah harga naik 10% per 1 Juli |
| Marjin kotor stabil 30% | Biaya bergerak proporsional dengan volume; masalah di sisi pendapatan, bukan biaya |
| Repeat purchase turun 25% | Pelanggan lama pindah ke pesaing yang harganya 12% lebih murah di wilayah yang sama |
| Biaya logistik per karton naik 18% | Rute pengiriman Region W dipecah dua setelah gudang transit ditutup Agustus |
| Pelanggan aktif turun 8.000 | Terkonsentrasi pada segmen warung kecil yang kehilangan skema kredit 14 hari |

### Latihan 1: finding atau cause? (dengan kunci)
| | Pernyataan | Status | Alasan |
|---|---|---|---|
| A | Marjin kotor turun 30% → 24% dalam tiga bulan | **Finding** | Hanya melaporkan perubahan angka |
| B | Diskon agen Region X naik 5% → 12% sejak Mei sehingga marjin tergerus | **Cause** | Menyebut dimensi, periode, dan mekanisme |
| C | Jumlah pelanggan aktif turun 8.000 | **Finding** | Agregat tanpa segmen; perlu drill-down |
| D | Pelanggan pindah ke pesaing karena harga kita 12% lebih mahal | **Cause** | Sah, *asalkan ada data perpindahan dan harga pesaing* |
| E | NPS turun 11 poin | **Finding** | Indikator, bukan penjelasan |
| F | Sales turun karena tim penjualan kurang bersemangat | **Asumsi** | Berbentuk penyebab tapi tidak terukur — "yang menyamar" |

**Pelajaran utama:** kata *"karena"* tidak membuat kalimat menjadi penyebab. **Yang membuatnya penyebab adalah bukti di belakangnya.**

## A4. Evidence vs Assumption

| | **Asumsi** | **Bukti** |
|---|---|---|
| Definisi | Dugaan yang belum diuji | Pernyataan yang dapat diperiksa |
| Asal | Pengalaman, kebiasaan, kesan | Data yang sumbernya bisa ditunjuk dan diulang |
| Bahasa | Kata umum: "pelanggan", "pasar", "tim" tanpa segmen | Menyebut besaran, arah, periode, populasi |
| Pembanding | Tidak ada angka/periode/pembanding | Ada pembanding (sebelum–sesudah, atau kelompok lain) |
| Sifat | Sulit dibantah karena tidak ada yang bisa diperiksa | **Bisa salah, dan justru karena itu bisa dipercaya** |
| Contoh | "Sales turun karena customer tidak suka produk." | "Data menunjukkan repeat purchase turun 25% setelah perubahan harga." |

### Contoh bukti sesungguhnya (Repeat purchase Produk A di Region X)
Tren mingguan: Jun W1–W4 sekitar 61–62%, Jul W1 60%, Jul W2 54%, Jul W3 50%, Jul W4 48%, Ags W1 47%, Ags W2 46%.

Yang membuatnya bukti:
- **Besaran jelas**: 62% → 46% (turun 25% *relatif*; 16 poin *absolut*)
- **Populasi jelas**: pembeli Produk A di Region X
- **Waktu jelas**: penurunan mulai minggu kedua Juli
- **Ada pembanding**: Region Y dan Z stabil pada periode yang sama

> Asumsi bertahan sampai ditanya. Bukti bertahan justru karena ditanya.

### Empat bentuk asumsi yang menyamar jadi bukti
1. **Angka tanpa pembanding**: "Penjualan Produk A Rp 3,6 miliar." Tinggi atau rendah? Tidak ada rujukan.
2. **Anekdot yang digeneralisasi**: "Tiga pelanggan mengeluh soal kemasan." Tiga dari berapa? Segmen mana?
3. **Korelasi dibacakan sebagai sebab**: "Belanja iklan naik, sales naik." Bisa jadi keduanya didorong musim.
4. **Otoritas sebagai pengganti data**: "Menurut pengalaman saya…" Pengalaman adalah **hipotesis, bukan bukti**.

### Uji kelayakan bukti (5 pertanyaan sebelum menerima klaim)
1. Dari **sumber data** apa angka ini diambil?
2. Berapa besar **populasi/sampel**nya?
3. Dibandingkan dengan **periode atau kelompok** apa?
4. Apakah **urutan waktunya** masuk akal (sebab lebih dulu dari akibat)?
5. **Penjelasan lain** apa yang sudah disingkirkan?

## A5. Bias yang Merusak Diagnosis

| Bias | Bentuknya | Penangkal praktis |
|---|---|---|
| **Confirmation bias** | Mencari data yang membenarkan dugaan awal, mengabaikan yang bertentangan | Tugaskan satu orang khusus mencari bukti yang **menjatuhkan** hipotesis |
| **Anchoring** | Terpaku pada angka/penjelasan pertama yang muncul di rapat | Rumuskan **minimal tiga hipotesis** sebelum melihat data pendukung |
| **Survivorship bias** | Hanya menganalisis pelanggan yang tersisa, bukan yang pergi | Analisis kelompok yang hilang: churn, pesanan batal, keranjang ditinggalkan |
| **Single-cause fallacy** | Berhenti di satu penyebab padahal beberapa faktor bekerja bersamaan | Kuantifikasi kontribusi tiap faktor; pastikan totalnya menjelaskan seluruh selisih |
| **Post hoc reasoning** | Kejadian yang lebih dulu otomatis dianggap penyebab | Uji dengan **kelompok pembanding** yang tidak mengalami kejadian itu |

Penangkal paling murah: tugaskan satu anggota tim sebagai **penantang (challenger)**.

## A6. Tujuh Teknik Diagnostik

Urutan: **3 pertama mempersempit ruang masalah → 3 berikutnya menggali sebab → yang terakhir menguji apakah sebab itu benar.**
(Atau pada ringkasan: *Drill-down, comparison, variance, segmentation* mempersempit; *5 Whys dan RCA* menggali; *causal thinking* menguji.)

| No | Teknik | Fungsi |
|---|---|---|
| 1 | Drill-down | Memecah angka agregat ke tingkat lebih rinci |
| 2 | Comparison | Membandingkan terhadap periode, target, atau kelompok lain |
| 3 | Variance | Menguraikan selisih jadi komponen harga, volume, bauran |
| 4 | Segmentation | Memotong data menurut karakteristik pelanggan/transaksi |
| 5 | 5 Whys | Menelusuri rantai sebab lapis demi lapis sampai ke akar |
| 6 | Root Cause Analysis | Memetakan kandidat penyebab sistematis, lalu menyaringnya |
| 7 | Causal thinking | Menguji apakah hubungan benar-benar kausal |

**Urutan penting:** menggali sebab sebelum mempersempit ruang masalah hampir selalu berakhir pada penyebab yang salah. → **"Persempit dulu, baru gali."**

### Teknik 1 — Drill-down
Memecah angka besar jadi bagian-bagiannya, lalu **mengikuti bagian yang paling banyak menyumbang selisih**.

**Lapis 1: per Region (Rp miliar)**
| Region | Q2 | Q3 | Selisih |
|---|---|---|---|
| Region X | 18,0 | 11,0 | **−7,0** |
| Region W | 7,0 | 5,4 | −1,6 |
| Region Y | 14,0 | 13,2 | −0,8 |
| Region Z | 11,0 | 10,4 | −0,6 |
| **Total** | **50,0** | **40,0** | **−10,0** |

→ Region X = 7,0/10,0 = **70%** dari total penurunan.

**Lapis 2: Region X per Produk**
| Produk | Q2 | Q3 | Selisih |
|---|---|---|---|
| Produk A | 9,0 | 3,6 | **−5,4** |
| Produk C | 3,0 | 2,1 | −0,9 |
| Produk D | 1,5 | 1,0 | −0,5 |
| Produk B | 4,5 | 4,3 | −0,2 |
| **Total** | **18,0** | **11,0** | **−7,0** |

→ Produk A di Region X = 5,4/10,0 = **54%** dari total penurunan **perusahaan**.

**Aturan drill-down:** ikuti **kontributor terbesar, bukan persentase terbesar**. Penurunan 60% di lini kecil jarang menjelaskan masalah perusahaan.

### Teknik 2 — Comparison
Angka tunggal tidak bermakna; makna muncul dari pembanding, dan **pilihan pembanding menentukan kesimpulan**.

| Jenis pembanding | Contoh | Kekuatan | Risiko |
|---|---|---|---|
| Periode sebelumnya | Q3 vs Q2 2026 | Menangkap perubahan terbaru | Tertukar dengan pola musiman |
| Periode tahun lalu | Q3 2026 vs Q3 2025 | Menetralkan efek musiman | Mengabaikan perubahan struktural |
| Terhadap target | Realisasi vs anggaran | Mengukur pencapaian rencana | Target keliru menyesatkan |
| Antar unit sejenis | Region X vs Y dan Z | Berfungsi sebagai **kelompok kontrol** | Unit harus benar-benar sebanding |
| Terhadap pesaing | Harga kita vs pesaing | Menempatkan kinerja dalam konteks pasar | Data eksternal sering tidak lengkap |

Pada kasus: pembanding paling berharga = **Region Y & Z** (harga tidak diubah, revenue hanya turun 5–6%) → **kelompok kontrol alami**.

### Teknik 3 — Variance Analysis
**Revenue = Harga × Volume**
- **Efek harga** = (Harga baru − Harga lama) × **Volume baru**
- **Efek volume** = (Volume baru − Volume lama) × **Harga lama**
- Efek harga + efek volume = selisih bersih (tepat, tanpa sisa)

Data Produk A Region X:
| | Q2 | Q3 |
|---|---|---|
| Harga per unit | Rp 25.000 | Rp 27.500 (+10%) |
| Volume | 360.000 | 130.000 (−64%) |
| Revenue | Rp 9,00 M | Rp 3,58 M |

Perhitungan:
- Efek harga = (27.500 − 25.000) × 130.000 = **+Rp 0,33 M** (≈ 325 juta)
- Efek volume = (130.000 − 360.000) × 25.000 = **−Rp 5,75 M**
- Selisih bersih = **−Rp 5,42 M**
- **Elastisitas harga** = −64% ÷ +10% = **−6,4** → permintaan **sangat elastis**; menaikkan harga menghancurkan pendapatan.

### Teknik 4 — Segmentation
Drill-down memecah menurut **struktur organisasi**; segmentasi memecah menurut **perilaku**, dan sering di situlah sebab bersembunyi.

| Segmen pembeli Produk A | Vol Q2 | Vol Q3 | Perubahan |
|---|---|---|---|
| Warung & toko kecil | 198.000 | 52.000 | **−74%** |
| Grosir menengah | 108.000 | 48.000 | −56% |
| Pelanggan korporat | 36.000 | 22.000 | −39% |
| Kontrak institusi | 18.000 | 8.000 | −56% |
| **Total** | **360.000** | **130.000** | **−64%** |

Yang terbaca:
- Warung kecil **paling sensitif harga** (−74%).
- Segmen ini menyumbang **63%** dari kehilangan volume (146.000 dari 230.000).
- **Korporat** dengan kontrak tahunan **paling tahan** (−39%).

Empat sumbu segmentasi yang layak dicoba dulu: **Demografis** (ukuran toko, lokasi, kategori pelanggan) · **Perilaku** (frekuensi beli, ukuran keranjang, loyalitas) · **Transaksional** (kanal, metode bayar, promo) · **Siklus hidup** (baru, aktif, tidur, hilang).

### Teknik 5 — 5 Whys
Bertanya "mengapa" berulang untuk bergerak dari gejala permukaan ke **proses yang memungkinkannya terjadi**.

Cara memakai:
- Mulai dari pernyataan masalah yang **sudah dipersempit drill-down**.
- Setiap jawaban **didukung data**, bukan dugaan.
- Berhenti saat sampai pada **proses atau kebijakan yang bisa diubah**.
- Angka lima **bukan aturan baku** (kadang 3 cukup, kadang 7).
- Jika satu lapisan punya dua jawaban sama kuat → **cabangkan** dan telusuri keduanya.

Kegagalan yang sering terjadi:
1. **Berhenti pada orang** ("operator lalai" menutup diskusi, bukan membukanya)
2. **Rantai tanpa bukti** (opini ditumpuk; cerita rapi tapi salah)
3. **Melompat lapisan** (dari gejala langsung ke kesimpulan favorit)
4. **Satu jalur tunggal** (mengabaikan dua sebab yang bekerja bersamaan)

**5 Whys pada PT Nusantara Segar:**
| # | Mengapa? | Karena |
|---|---|---|
| 1 | Laba usaha turun 38%? | Revenue turun 20% sementara struktur biaya relatif tetap (marjin kotor bertahan 30%) |
| 2 | Revenue turun 20%? | 54% penurunan berasal dari satu sel: Produk A di Region X, Rp 5,4 miliar |
| 3 | Produk A di Region X turun? | Volume turun 64% sejak harga naik 10% pada 1 Juli; efek volume −Rp 5,75 M |
| 4 | Volume turun sebesar itu? | Harga kita 12% di atas pesaing di wilayah yang sama; repeat purchase turun 25% |
| 5 | Mengapa harga dinaikkan tanpa mengantisipasi itu? | Keputusan harga regional **tidak melalui uji elastisitas** dan **tidak ada pemantauan selisih harga pesaing** |

**Akar masalah:** proses penetapan harga regional tanpa pengaman elastisitas dan tanpa pemantauan harga pesaing. (Perhatikan: akarnya **proses/kebijakan**, bukan orang.)

### Teknik 6 — Root Cause Analysis (RCA)
5 Whys menelusuri **satu jalur**. RCA **memetakan semua kandidat penyebab lebih dulu, lalu menyaringnya dengan bukti**.

Enam kategori kandidat pada kasus:
| Kategori | Contoh kandidat | Hasil |
|---|---|---|
| **Harga & promosi** | Kenaikan harga 10%, selisih 12% vs pesaing, program diskon dihentikan | ✅ **Didukung** |
| Produk | Keluhan mutu, perubahan kemasan, masa simpan | gugur |
| Distribusi | Ketersediaan di toko, jangkauan outlet, keterlambatan kirim | gugur |
| Tenaga penjual | Rotasi salesman, target & insentif, kunjungan menurun | gugur |
| **Proses & kebijakan** | SOP pricing regional, tanpa uji elastisitas, tanpa pemantauan harga | ✅ **Didukung** |
| Eksternal | Promo bundling pesaing, daya beli wilayah, musim & cuaca | gugur |

Dua yang bertahan: **kebijakan harga** dan **proses yang mengizinkan kebijakan itu diambil tanpa pengujian**.

### Teknik 7 — Korelasi bukan Kausalitas
Dua angka bergerak bersamaan hanya memberi **kandidat**, bukan kesimpulan. Empat kemungkinan:
1. **A menyebabkan B**: harga naik → volume turun (yang ingin dibuktikan)
2. **B menyebabkan A** (arah terbalik): penjualan lesu → manajer menaikkan harga untuk menambal pendapatan
3. **Faktor ketiga (C)**: krisis daya beli wilayah menekan volume sekaligus mendorong penyesuaian harga
4. **Kebetulan belaka**: dua tren tidak berhubungan, terutama pada sampel kecil

Contoh klasik: **belanja iklan** naik bersamaan dengan **penjualan es krim** (korelasi 0,91), keduanya didorong **musim kemarau**.

### Lima uji sebelum menyebut sesuatu penyebab
| # | Uji | Prinsip | Bukti pada kasus |
|---|---|---|---|
| 1 | **Urutan waktu** | Sebab mendahului akibat | Harga berubah 1 Juli; penurunan mulai minggu kedua Juli |
| 2 | **Mekanisme masuk akal** | Ada cerita sebab-akibat | Harga naik → selisih 12% vs pesaing → pelanggan berpindah |
| 3 | **Kelompok pembanding** | Unit serupa tanpa perlakuan tidak terdampak | Region Y & Z tanpa perubahan harga hanya turun 5–6% |
| 4 | **Dosis–respons** | Perlakuan lebih besar → efek lebih besar | Warung kecil (paling sensitif harga) turun paling dalam: 74% |
| 5 | **Alternatif tersingkir** | Penjelasan lain diuji dan gugur | Service level 97%; keluhan mutu tidak naik; Produk B–D stabil |

> **Mnemonik:** *WaMPDA* — **Wa**ktu, **M**ekanisme, **P**embanding, **D**osis-respons, **A**lternatif.

## A7. Kerangka Lima Langkah

**Problem → Dimension → Drill-down → Evidence → Cause**

| Langkah | Isi | Pertanyaan pemandu | Contoh kasus |
|---|---|---|---|
| 1. **Problem** | Nyatakan masalah sebagai angka: apa yang bergerak, seberapa besar, sejak kapan | "Apa yang bergerak?" | "Laba turun 38% pada Q3." |
| 2. **Dimension** | Pilih sumbu pemecahan yang paling mungkin menjelaskan (struktur, produk, wilayah, segmen, waktu) | "Di sumbu mana ia bisa dipecah?" | Revenue vs cost; lalu region |
| 3. **Drill-down** | Turun lapis demi lapis, ikuti kontributor selisih terbesar | "Bagian mana yang menyumbang paling besar?" | Region X → Produk A → segmen warung |
| 4. **Evidence** | Kumpulkan data yang menguji hipotesis, **termasuk yang bisa menjatuhkannya** | "Apa buktinya?" | Volume, harga, repeat purchase, harga pesaing |
| 5. **Cause** | Rumuskan penyebab yang menyebut dimensi, pemicu, dan dapat ditindaklanjuti | "Apa yang bisa kita ubah?" | Kebijakan harga 1 Juli tanpa uji elastisitas |

### Penerapan Langkah 1 & 2
**Pernyataan masalah:** Laba usaha Q3 2026 turun 38% dibanding Q2 2026, dari Rp 6,0 M menjadi Rp 3,7 M.

| Rp miliar | Q2 | Q3 | Perubahan |
|---|---|---|---|
| Revenue | 50,0 | 40,0 | −20% |
| HPP | 35,0 | 28,0 | −20% |
| Beban usaha | 9,0 | 8,3 | −8% |
| **Laba usaha** | **6,0** | **3,7** | **−38%** |

Perhitungan: Laba usaha = Revenue − HPP − Beban usaha → Q2: 50 − 35 − 9 = 6,0; Q3: 40 − 28 − 8,3 = 3,7.
Marjin kotor = (50−35)/50 = 30%; (40−28)/40 = 30% → **tetap**.

Dimensi yang dipilih dan alasannya:
1. **Struktur laba (revenue vs biaya)**: marjin kotor tetap 30% → biaya ikut volume → **jalur biaya ditutup**
2. **Wilayah (4 region)**: harga ditetapkan per region
3. **Produk (4 lini)**: Produk A menyumbang 40% revenue
4. **Waktu (mingguan)**: untuk menguji urutan waktu kebijakan vs penurunan
5. **Segmen pelanggan (4 tipe)**: untuk uji dosis–respons

> Memilih dimensi adalah **keputusan analitis, bukan langkah teknis**. Dimensi keliru → drill-down berputar tanpa hasil.

### Penerapan Langkah 3 & 4 — Corong drill-down
- Perusahaan: −Rp 10,0 M (100%)
- Region X: −Rp 7,0 M (70%)
- **Produk A di Region X: −Rp 5,4 M (54%)**
- Segmen warung kecil: −Rp 3,4 M (34%)

Tabel bukti:
| Bukti | Temuan | Sumber |
|---|---|---|
| Harga jual Produk A Region X | Rp 25.000 → Rp 27.500 per 1 Juli | Master harga |
| Volume mingguan | −64%; mulai turun minggu ke-2 Juli | Data POS |
| Repeat purchase | 62% → 46% (−25% relatif) | CRM |
| Harga pesaing di Region X | Rp 24.500 sejak 5 Juli; selisih 12% | Survei pasar |
| Ketersediaan barang | Service level 97%, tak ada kekosongan | Gudang |
| Keluhan mutu | Tidak naik; 0,3% dari transaksi | Layanan pelanggan |
| Region pembanding Y & Z | Harga tetap; revenue −5% dan −6% | Data penjualan |

Catatan: **dua baris terakhir** (keluhan mutu/ketersediaan dan region pembanding) dikumpulkan **untuk menjatuhkan hipotesis**, bukan mendukungnya.

### Penerapan Langkah 5 — Cause dan tindak lanjut
**ROOT CAUSE:** Kenaikan harga Produk A sebesar 10% di Region X per 1 Juli, diambil **tanpa uji elastisitas dan tanpa pemantauan harga pesaing**, menciptakan selisih harga 12% yang memindahkan pelanggan warung kecil ke pesaing.

**Hipotesis alternatif yang gugur:**
| Hipotesis | Data yang menjatuhkan |
|---|---|
| Kehabisan stok | Service level 97% |
| Mutu produk menurun | Keluhan tetap 0,3% |
| Daya beli wilayah melemah | Produk B–D di Region X stabil |
| Tim penjualan kurang efektif | Jumlah kunjungan naik 4% |

**Rekomendasi yang mengikuti dari penyebab:**
1. **Koreksi harga**: turunkan Produk A di Region X ke Rp 25.750 sehingga selisih terhadap pesaing di bawah 5%
2. **Uji sebelum terapkan**: uji harga terbatas di 20 toko selama 4 minggu
3. **Pasang pengaman**: pemantauan mingguan selisih harga pesaing, ambang peringatan 5%
4. **Perbaiki proses**: SOP pricing regional wajib menyertakan estimasi elastisitas dan persetujuan lintas fungsi

> (Catatan hitungan: 25.750 ÷ 24.500 ≈ 1,051, yaitu selisih ≈ 5,1%, jadi *hampir* di bawah 5%. Di kuis, cukup tahu logikanya: koreksi harga untuk menutup gap pesaing.)

**Uji akhir kualitas diagnosis:** rekomendasi harus menunjuk pada **keputusan yang bisa diubah**, bukan pada sifat pelanggan atau keadaan pasar.

## A8. Menyampaikan Hasil Diagnosis (4 Bagian)
1. **Finding**: satu kalimat angka: apa yang bergerak dan seberapa besar
2. **Evidence**: 3–5 bukti terkuat, termasuk yang berfungsi sebagai pembanding
3. **Cause**: satu kalimat penyebab yang menyebut dimensi dan pemicu
4. **Action**: 2–4 tindakan **dengan pemilik dan tenggat waktu**

**Enam kesalahan paling sering:**
1. Menyajikan finding sebagai cause (semua benar tapi tak ada yang menjelaskan)
2. Berhenti di lapis pertama (Region X ditemukan, tak turun ke produk)
3. Memilih bukti yang cocok saja (data bertentangan tidak dicari)
4. Menyalahkan orang (rantai berakhir pada individu, bukan proses)
5. Mengabaikan besaran (penyebab benar tapi hanya menjelaskan 3% selisih)
6. Rekomendasi tanpa pemilik (tidak melekat pada siapa pun, tidak pernah jalan)

## A9. Rangkuman 5 Poin
1. Finding menjawab "apa", cause menjawab "mengapa". Temuan tidak bisa ditindaklanjuti; penyebab bisa.
2. Kata "karena" tidak menciptakan bukti. Kalimat jadi penyebab karena data di belakangnya.
3. **Persempit dulu, baru gali.** Terbalik → tebakan.
4. Korelasi hanya memberi kandidat. Lima uji yang mengubahnya jadi penyebab.
5. Penyebab yang baik menunjuk keputusan. Jika rekomendasi bukan sesuatu yang bisa diubah perusahaan, diagnosis belum selesai.

## A10. Tiga Kasus Diskusi (kemungkinan jadi bahan soal)
| Kasus | Data | Dimensi tersedia |
|---|---|---|
| **1. Peritel pakaian** | Conversion rate toko turun 22% → 15% dalam 2 bulan; kunjungan justru naik 9%; nilai transaksi rata-rata tetap; dua kompetitor buka gerai di mal yang sama | Gerai, hari, jam, kategori produk, staf per shift |
| **2. Distribusi FMCG** | Biaya logistik per karton naik 18%; volume pengiriman tidak berubah; gudang transit ditutup Agustus; ketepatan waktu turun 12 poin | Rute, armada, jarak, muatan, vendor, periode |
| **3. E-commerce grocery** | GMV naik 12% tapi laba turun 20%; nilai pesanan rata-rata turun 15%; biaya promosi naik 40%; pelanggan baru +35%, pelanggan lama −8% | Kanal akuisisi, kohort, kategori, kupon, kota |

Output yang diminta: **1 finding, minimal 4 bukti + sumber, 2 hipotesis yang berhasil disingkirkan, 1 root cause, 2 rekomendasi bernama pemilik.**

Pembagian peran: **Data lead** (drill-down, konsistensi angka) · **Evidence keeper** (catat bukti + sumber, tolak klaim tanpa data) · **Challenger** (jatuhkan kesimpulan, hipotesis tandingan) · **Presenter** (alur Finding–Evidence–Cause–Action).

**Rubrik (100):** Pemisahan finding vs cause **25** · Kualitas & kelengkapan bukti **30** · Logika kausal & penyingkiran alternatif **25** · Rekomendasi dapat dijalankan **10** · Kejelasan penyampaian **10**.

**Pertanyaan penguji:** dari mana angka & berapa populasinya? · apa pembandingnya dan mengapa sah? · penjelasan lain apa yang sudah dicoba dijatuhkan? · berapa persen total selisih yang dijelaskan penyebab Anda? · keputusan apa yang berubah setelah analisis ini?

### Cara menganalisis Kasus 1–3 (contoh berpikir, bila keluar di kuis)
- **Kasus 1 (Peritel pakaian)**: kunjungan naik tetapi konversi turun → bukan masalah traffic. Persempit per gerai/jam/kategori. Yang perlu diuji: gerai dekat kompetitor baru vs gerai lain (kelompok kontrol), stok/ukuran, jumlah staf per shift (jam ramai). Nilai transaksi tetap → yang hilang adalah *jumlah pembeli*, bukan nilai.
- **Kasus 2 (Distribusi FMCG)**: volume tetap, biaya per karton naik → jalur biaya/rute. Gudang transit ditutup Agustus → bandingkan rute yang terdampak vs tidak, sebelum vs sesudah Agustus, jarak, muatan, vendor. Uji urutan waktu + dosis–respons (rute yang makin panjang → biaya makin naik).
- **Kasus 3 (E-commerce grocery)**: GMV naik tapi laba turun → decompose: nilai pesanan −15%, biaya promosi +40%. Pelanggan baru naik (akuisisi lewat kupon?), lama turun (kohort). Uji per kanal akuisisi, kohort, penggunaan kupon. Waspadai *survivorship bias* dan *single-cause fallacy*.

---

# BAGIAN B — SOAR & SWOT BUSINESS ANALYSIS FRAMEWORK

Alur utama modul: **Business Question → Evidence → Analysis → Communication**

## B1. Tujuan Pembelajaran
1. **Merumuskan pertanyaan bisnis**: mengubah keluhan menjadi pertanyaan yang bisa dijawab data
2. **Mengumpulkan evidence**: memilih sumber data dan menguji kelayakannya
3. **Menyusun SWOT terukur**: tiap butir dengan metrik, pembanding, periode, dan sumber
4. **Mengomunikasikan implikasi**: temuan → rekomendasi dengan pemilik dan tenggat

## B2. Cara Biasa vs Cara yang Dipakai
| Cara biasa | Cara yang kita pakai |
|---|---|
| Rapat → brainstorming → kotak SWOT terisi | **Pertanyaan → bukti → analisis → keputusan** |
| Isi dari kesan/pengalaman pribadi | Setiap butir membawa metrik dan sumber |
| Tak ada angka, pembanding, periode | Besaran masalah bisa dibandingkan & diurutkan |
| Semua butir terasa sama penting | Prioritas dari **dampak**, bukan suara terkeras |
| Tak ada keputusan yang berubah | Berakhir di rekomendasi yang bisa dieksekusi |

## B3. Posisi SOAR vs SWOT
- **SOAR = mesinnya (proses)**: bagaimana cara kerja analisisnya.
- **SWOT = keluarannya (kerangka keluaran)**: bagaimana temuan dirapikan ke 4 kuadran.
- **Konsekuensi: SWOT tidak pernah menjadi langkah pertama. Ia adalah langkah keempat.** (Isinya hanya sebaik proses yang menghasilkannya.)

## B4. Definisi SOAR
Kerangka kerja analisis bisnis yang membagi pekerjaan analis menjadi **empat tahap berurutan**, sehingga setiap kesimpulan dapat ditelusuri ke pertanyaan yang melatarbelakangi dan data yang mendukung.

| Huruf | Tahap | Fungsi | Padanan |
|---|---|---|---|
| **S** | **Specify** | Merumuskan pertanyaan bisnis (spesifik, terukur, terikat keputusan) | Business Question |
| **O** | **Obtain** | Mengumpulkan data & bukti, **termasuk menguji kualitasnya** | Evidence |
| **A** | **Analyze** | Mengolah data jadi temuan: pola, selisih vs pembanding, akar penyebab | Analysis |
| **R** | **Report** | Menyampaikan jawaban & rekomendasi yang bisa ditindaklanjuti | Communication |

Melompati tahap akan terasa di tahap berikutnya: pertanyaan kabur → data salah; data lemah → analisis rapuh; analisis tak dikomunikasikan → tidak mengubah apa pun.

### Latihan kilat: kegiatan ini masuk tahap mana?
| Kegiatan | Tahap | Catatan |
|---|---|---|
| Menyusun kalimat "Berapa service time jam sibuk dibanding benchmark?" | **Specify** | Belum menyentuh data |
| Mengunduh log sistem kasir 38 gerai sepanjang 2025 | **Obtain** | Ambil data mentah internal |
| Membandingkan gerai bervolume tinggi vs rendah | **Analyze** | Cari pola/selisih antar segmen |
| Menulis satu kalimat jawaban di halaman pertama memo direksi | **Report** | Jawaban dulu, bukti menyusul |
| Memeriksa 12% baris transaksi yang kosong | **Obtain** (bukan Analyze!) | Uji kelayakan data bagian dari mengumpulkan |

## B5. S — Specify: Anatomi Pertanyaan Bisnis (4 Unsur)
Contoh: *"Berapa rata-rata **service time** di **38 gerai pada jam sibuk, Januari–Desember 2025**, dibanding **benchmark 8,6 menit**?"*

1. **Subjek**: metrik apa yang diukur
2. **Batas**: unit mana, kapan, di mana
3. **Pembanding**: benchmark, target, atau periode lalu
4. **Keputusan**: keputusan apa yang menunggu jawaban ini

**Uji satu kalimat:** bila jawabannya "ya" atau "tidak", adakah **tindakan yang berbeda**? Bila tidak, pertanyaannya belum layak dianalisis.

### Dari pertanyaan kabur ke pertanyaan kerja
| Kabur | Kerja | Yang ditambahkan |
|---|---|---|
| Kenapa penjualan kita turun? | Dari penurunan pendapatan 6,2% pada H2 2025, berapa bagian dari turunnya jumlah transaksi dan berapa dari turunnya nilai rata-rata transaksi? | Dekomposisi dan periode |
| Apakah pelayanan kita buruk? | Berapa rata-rata service time di 38 outlet pada jam sibuk, dan berapa outlet di atas benchmark industri 8,6 menit? | Metrik dan pembanding |
| Perlukah kita buka cabang baru? | Pada tingkat transaksi saat ini, berapa bulan payback outlet baru di Bandar Lampung, dan berapa ambang transaksi harian agar payback < 24 bulan? | Ambang keputusan |
| Karyawan kita betah tidak? | Berapa turnover barista 12 bulan terakhir dibanding benchmark F&B 32%, dan berapa biaya rekrutmen + pelatihan yang timbul? | Konsekuensi finansial |

**Contoh versi lolos:** SEBELUM "Kenapa penjualan kita turun?" → SESUDAH *"Berapa penurunan penjualan gerai mal dibanding gerai jalan raya pada kuartal IV 2025 terhadap kuartal III, dan apakah cukup besar untuk menunda pembukaan gerai baru?"*
(Subjek = penjualan gerai · Batas = mal vs jalan raya, Q4 2025 · Pembanding = terhadap Q3 2025 · Keputusan = tunda ekspansi atau tidak)

## B6. O — Obtain: Evidence

### Tiga sumber evidence
| Sumber | Mengisi | Contoh |
|---|---|---|
| **Internal** | **Strength & Weakness** | Sistem kasir/transaksi, laporan keuangan, data kepegawaian, CRM & aplikasi member |
| **Eksternal** | **Opportunity & Threat** | Statistik resmi pemerintah, laporan asosiasi industri, harga komoditas & regulasi, ulasan publik & media |
| **Primer** | Dikumpulkan sendiri saat ada celah | Survei & wawancara, observasi lapangan, pengukuran waktu proses, uji A/B skala kecil |

**Urutan hemat:** internal dulu (paling murah) → eksternal → primer terakhir (untuk menutup celah yang benar-benar menentukan jawaban).

### Lima dimensi kualitas data
1. **Kelengkapan**: berapa % baris kosong? outlet/periode mana tak terwakili?
2. **Akurasi**: cocok bila diuji silang (misalnya POS vs laporan keuangan)?
3. **Kebaruan**: kapan terakhir diperbarui? masih menggambarkan kondisi sekarang?
4. **Konsistensi**: definisi metrik sama di semua unit? (satu outlet hitung sejak antre, lainnya sejak memesan?)
5. **Keterlacakan**: siapa sumbernya, bisa ditunjuk ulang? **Data tanpa sumber tidak boleh masuk SWOT.**

> **Mnemonik:** *Lengkap, Akurat, Baru, Konsisten, Terlacak.*

### Tiga jebakan pengumpulan data
| Jebakan | Penjelasan | Contoh |
|---|---|---|
| **Yang kecewa sudah pergi** (survivorship) | Hanya data dari yang masih ada, skor terlihat terlalu bagus | Formulir kepuasan di meja kasir, hanya diisi yang masih datang & membayar |
| **Sampel tidak mewakili** | Mengukur pada waktu/kondisi yang tidak mewakili | Antrean dicatat Rabu 10.00 selama sebulan, padahal bukan jam sibuk |
| **Metrik pengganti keliru** | Mengukur hal yang mudah, bukan yang sebenarnya ingin diukur | Pengikut Instagram dipakai sebagai ukuran loyalitas (seharusnya pembelian ulang) |

Kunci latihan "Cari cacatnya": Skenario A (pengikut Instagram) = **Metrik pengganti keliru**; B (formulir di kasir) = **Yang kecewa sudah pergi**; C (Rabu 10.00) = **Sampel tidak mewakili**.

> Tulis keterbatasan data secara terbuka. Analisis yang jujur soal batasnya lebih dipercaya.

## B7. A — Analyze

### Tangga analitik
| Tingkat | Pertanyaan | Isi | Peran dalam SWOT |
|---|---|---|---|
| Deskriptif | Apa yang terjadi? | Rata-rata, tren, distribusi, pangsa. Tahap wajib | Dasar pembanding |
| Diagnostik | Mengapa terjadi? | Segmentasi, dekomposisi, korelasi, akar masalah | **Sebagian besar SWOT dibentuk di sini** |
| Prediktif | Apa yang akan terjadi? | Proyeksi, skenario, simulasi sensitivitas | **Menakar Opportunity & Threat** |
| Preskriptif | Apa yang harus dilakukan? | Pilihan tindakan beserta untung-ruginya | **Business implication** yang dicari |

Kesalahan umum: melompat langsung ke anak tangga terakhir. *Rekomendasi tanpa diagnosis hanyalah tebakan yang ditulis dengan percaya diri.*

### Lima teknik analisis
| Teknik | Menjawab | Contoh |
|---|---|---|
| **Perbandingan benchmark** | Seberapa jauh dari standar? | Service time 12 menit vs benchmark 8,6 menit → selisih 40% |
| **Analisis tren** | Membaik atau memburuk? | Margin bersih 6,8% (2024) → 4,1% (2025), turun 4 kuartal |
| **Segmentasi** | Siapa/mana yang berbeda? | Dari 38 outlet, 9 outlet menyumbang 61% keluhan antrean |
| **Dekomposisi** | Dari mana angkanya berasal? | Pendapatan = jumlah transaksi × nilai rata-rata transaksi; mana yang bergerak? |
| **Akar masalah** | Apa penyebab di baliknya? | 5 Whys atau diagram tulang ikan sampai menemui penyebab yang bisa diubah |

Satu temuan kuat biasanya lahir dari **dua teknik yang saling menguatkan**, bukan satu angka.

### Korelasi bukan kausalitas (versi kasus kopi)
Sebaran 20 gerai: turnover barista (20–70%) vs service time (9–17 menit). Kesimpulan terburu-buru: *"turnover tinggi menyebabkan layanan lambat, maka naikkan gaji barista."*

**Tiga pertanyaan penjaga:**
1. **Arah**: mungkinkah sebaliknya? gerai kacau membuat barista cepat keluar?
2. **Faktor ketiga**: gerai bervolume tinggi dengan dapur sempit menyebabkan keduanya?
3. **Kebetulan**: berapa gerai yang diamati, berapa lama periodenya?

**Cara menguji:** bandingkan gerai dengan **volume setara**, atau amati perubahan service time **sebelum dan sesudah** turnover naik.

## B8. R — Report

### Piramida: jawaban dulu, baru buktinya
- **Tingkat 1** — Satu kalimat yang menjawab pertanyaan bisnis dan menyebut keputusannya
- **Tingkat 2** — Tiga temuan utama penopang jawaban, masing-masing dengan angka
- **Tingkat 3** — Tabel, grafik, metode, catatan keterbatasan data (bagi yang ingin menelusuri)

Analis bekerja dari **data → kesimpulan**; pembaca sebaliknya: **kesimpulan dulu**, lalu memutuskan seberapa dalam menelusuri.
**Aturan praktis:** judul slide = **temuan, bukan topik**. ✅ "Service time jam sibuk menahan 23% calon pembeli" ❌ "Analisis Service Time".

### What → So what → Now what
- **What**: apa yang terlihat di data
- **So what**: apa artinya bagi bisnis (dalam **rupiah atau risiko**)
- **Now what**: tindakan apa, **oleh siapa, biaya berapa, kapan**

Contoh lengkap:
- **What**: Service time jam sibuk 17 menit di 9 outlet bervolume tertinggi; 23% calon pembeli membatalkan antrean.
- **So what**: Pada nilai rata-rata transaksi Rp 38.500, pembatalan antrean di 9 outlet setara potensi pendapatan hilang sekitar **Rp 4,0 M/tahun**, lebih dari separuh laba bersih 2025 (4,0/7,6 ≈ 53%).
- **Now what**: Pisahkan jalur pesanan daring dari kasir di 9 outlet. **Pemilik:** Manajer Operasional. **Biaya:** Rp 420 juta. **Target:** service time jam sibuk turun ke 11 menit dalam 2 kuartal. **Ukur ulang:** akhir Q2.

### Empat anti-pola komunikasi
1. **Timbunan data**: 20 grafik tanpa satu kesimpulan
2. **Temuan tanpa tindakan**: "Kepuasan menurun." Lalu apa?
3. **Presisi palsu**: "Naik 7,43%" dari sampel hanya 40 orang
4. **Menyembunyikan batas**: keterbatasan tak disebut; ketika ketahuan, kepercayaan hilang

Tanda laporan baik: pembaca bisa **mengulang kesimpulannya dengan kalimat sendiri** setelah membaca satu halaman.

### Format kalimat jawaban
*"Jawabannya adalah ____, karena ____, maka kita harus ____."*

Contoh kunci: *"Jawabannya adalah **kapasitas jam sibuk**, karena 9 gerai tersibuk dua kali lebih lambat dari benchmark dan 23% calon pembeli pergi sebelum dilayani, maka kita harus **memisahkan jalur pesanan daring sebelum membuka gerai baru**."*
(Jawabannya = akar masalah, bukan gejala · Karena = dua angka, bukan kesan · Maka kita harus = satu tindakan yang bisa dimulai, dan ada yang ditunda)

## B9. SWOT

### Definisi
Kerangka menata temuan ke **empat kuadran** dari **dua sumbu**: **asal faktor** (internal/eksternal) dan **pengaruhnya terhadap tujuan** (membantu/menghambat).

| | **Membantu** | **Menghambat** |
|---|---|---|
| **Internal** | **Strength** (kekuatan): yang kita miliki & membuat unggul | **Weakness** (kelemahan): kesenjangan di dalam kendali kita |
| **Eksternal** | **Opportunity** (peluang): perubahan di luar yang bisa dimanfaatkan | **Threat** (ancaman): perubahan di luar yang bisa merugikan |

**Setiap butir SWOT = klaim tentang kenyataan. Klaim menuntut bukti.** Tanpa bukti = daftar pendapat yang dirapikan.

### Uji cepat penempatan kuadran
1. **Bisa diubah perusahaan sendiri dalam setahun?** Ya → **internal**. Tidak → **eksternal**.
2. **Membantu atau menghambat tujuan?** Membantu → **S atau O**. Menghambat → **W atau T**.

Contoh latihan (enam butir):
| Butir | Kuadran | Alasan |
|---|---|---|
| Harga green bean arabika naik 34% setahun | **Threat** | Eksternal, merugikan |
| Kontrak 3 tahun dengan koperasi petani | **Strength** | Internal (perusahaan yang menandatangani), membantu |
| Turnover barista 47%, benchmark 32% | **Weakness** | Internal, menghambat |
| Pasar kopi spesialti tumbuh 12,4%/tahun | **Opportunity** | Eksternal, membantu |
| Aplikasi member 61.000 pengguna terdaftar | **Strength** | Internal, membantu |
| Komisi agregator pesan-antar naik ke 25% | **Threat** | Eksternal, merugikan |

### Empat kesalahan yang membuat SWOT tidak berguna
1. **Kata sifat tanpa angka**: "pelayanan buruk", "brand kuat" (tak bisa diukur/disanggah)
2. **Daftar terlalu panjang**: 12 butir per kuadran tanpa urutan → tak ada yang dikerjakan
3. **Salah kuadran**: "pasar tumbuh" ditaruh di Strength (sumbu internal–eksternal tertukar)
4. **Berhenti di matriks**: matriks selesai lalu ditutup; tak ada strategi

**Batas sehat: maksimal 4 butir per kuadran, diurutkan dari dampak terbesar.**

### Lima unsur butir SWOT berbasis evidence
1. **Klaim**: apa yang dinyatakan, satu frasa
2. **Metrik**: angka beserta satuannya
3. **Pembanding**: benchmark / target / periode lalu
4. **Periode**: kapan diukur dan berapa lama
5. **Sumber**: dari mana datanya, agar bisa ditelusuri

Contoh Weakness lengkap: *"Rata-rata **service time 12 menit** pada 38 outlet, **40% di atas benchmark industri 8,6 menit**, diukur sepanjang **Januari–Desember 2025** dari **log sistem kasir**."*

**Audit butir (unsur yang hilang):**
- *"Service time kami 12 menit, diukur sepanjang 2025 dari log sistem kasir."* → hilang **Pembanding**
- *"Turnover barista 47% vs benchmark industri 32%, menurut data kepegawaian."* → hilang **Periode**
- *"Margin laba bersih turun ke 4,1% dari 6,8% pada 2024, sepanjang tahun buku 2025."* → hilang **Sumber**

**Dari opini ke evidence:**
| Kuadran | Opini | Evidence |
|---|---|---|
| Weakness | Pelayanan buruk | Service time 12 menit di 38 outlet sepanjang 2025, 40% di atas benchmark 8,6 menit; jam sibuk 17 menit. Sumber: log kasir |
| Strength | Brand kami kuat di daerah | Pangsa 23% kedai kopi spesialti Lampung vs 16% pesaing terbesar; 38 gerai aktif per Des 2025. Sumber: riset pasar internal 2025 |
| Opportunity | Pasar kopi naik daun | Konsumsi kopi spesialti nasional tumbuh rata-rata 12,4%/tahun 2022–2025; pendapatan kami +14,0% pada 2025. Sumber: laporan asosiasi industri |
| Threat | Kompetitor makin agresif | 3 jaringan nasional membuka 14 gerai baru di Lampung dalam 18 bulan, semua dalam radius 2 km dari gerai kami. Sumber: pemantauan lapangan Jan 2025–Jun 2026 |

### Lima pertanyaan pemeriksaan mutu setiap butir
1. **Ada angkanya?** (hapus kata sifat, masih tersisa isi?)
2. **Dibanding apa?** (angka tanpa pembanding tak memberi tahu baik/buruk)
3. **Sumbernya jelas?** (siapa pun bisa memeriksa ulang)
4. **Kuadrannya tepat?** (bisa diubah sendiri dalam setahun = internal)
5. **Cukup besar?** (nilai dalam rupiah/risiko; tanpa itu tak jadi prioritas)

Butir yang **gagal di pertanyaan 1 atau 2** → **ditulis ulang**, bukan sekadar dirapikan.

**Voting pembuka (kunci):**
| Butir | Hasil | Alasan |
|---|---|---|
| Brand kami kuat di kalangan anak muda | GAGAL | Kata sifat tanpa angka |
| Rating aplikasi 4,6/5 dari 2.140 ulasan, di atas rata-rata kategori 4,2 | **LOLOS** | Metrik, pembanding, besaran sampel dalam satu kalimat |
| Pelayanan kami lambat dan perlu segera diperbaiki | GAGAL | Dua kata sifat, tak ada angka/pembanding |
| Harga green bean naik 34% setahun; 64% pasokan kami terkunci kontrak | **LOLOS** | Angka, periode, besaran paparan risiko |

## B10. Studi Kasus 1 — Bisnis Ayam Geprek (SWOT skala UMKM)

**Data 5 bulan:**
| Bulan | Porsi | Omzet | Bahan baku | Operasional | Laba bersih | Rating | Retensi |
|---|---|---|---|---|---|---|---|
| Jan | 5.200 | 104 jt | 44 jt | 29 jt | 31 jt | 4,6 | 60% |
| Feb | 5.400 | 108 jt | 45 jt | 30 jt | 33 jt | 4,6 | 61% |
| Mar | 5.600 | 112 jt | 47 jt | 30 jt | 35 jt | 4,7 | 62% |
| Apr | 5.700 | 114 jt | 46,5 jt | 30 jt | 37,5 jt | 4,7 | 63% |
| Mei | 5.800 | 116 jt | 47,5 jt | 30,5 jt | 38 jt | 4,6 | 64% |

Rumus: **Omzet = porsi × Rp 20.000**; **Laba bersih = omzet − bahan baku − operasional** (cek Jan: 104 − 44 − 29 = 31 jt ✓).

Indikator utama: margin laba bersih bulanan **30,5%** · rating GoFood & GrabFood **4,6/5** · pelanggan kembali ≥2×/bulan **60%** · pesaing serupa radius 3 km **12**. Data satu tahun: rata-rata **180 porsi/hari**, harga rata-rata **Rp 20.000/porsi**, pertumbuhan penjualan **+15% YoY**.

> (Catatan: kalau dihitung dari lima bulan di tabel, margin sekitar 29,8%–32,9% per bulan, rata-rata ±31,5%. Angka 30,5% di slide tampaknya angka setahun. Hafalkan angka di slide.)

**SWOT:**
- **Strength**: margin laba bersih tinggi (30,5%) · rating 4,6/5 · retensi 60% (basis loyal besar) · variasi level pedas = diferensiasi
- **Weakness**: kapasitas maks **250 porsi/hari** → antrean · ketergantungan pada GoFood/GrabFood · branding masih sebatas lokal
- **Opportunity**: tren makanan pedas meningkat · pengguna aplikasi pesan-antar naik · ekspansi ke kampus & perkantoran · produk turunan (keju, jumbo, paket hemat)
- **Threat**: 12 pesaing serupa radius 3 km · fluktuasi harga cabai & ayam · regulasi izin & keamanan pangan ketat · pergeseran selera ke makanan sehat

**Strategi silang:**
| Strategi | Logika | Isi |
|---|---|---|
| **SO** | Kekuatan untuk merebut peluang | Buka cabang kecil di sekitar kampus dengan branding "Tambah nasi sepuasnya" |
| **WO** | Tutup kelemahan lewat peluang | Tingkatkan kapasitas dapur & pakai sistem digital untuk efisiensi operasional |
| **ST** | Kekuatan untuk menahan ancaman | Gunakan rating 4,6 sebagai senjata branding melawan 12 pesaing di radius 3 km |
| **WT** | Bertahan dari risiko ganda | Kontrak harga dengan pemasok cabai & ayam untuk menekan risiko fluktuasi |

## B11. Studi Kasus 2 — PT Kopi Nusa Rasa (dari data mentah sampai business implication)

**Profil:** jaringan kedai kopi spesialti regional, **38 gerai** di Lampung, Palembang, Bengkulu; berdiri 2017; **412 karyawan**; satu unit roastery yang memasok kafe & hotel.

**Angka 2025:**
- Pendapatan **Rp 184,6 M** (naik 14,0% dari Rp 161,9 M)
- Laba bersih **Rp 7,6 M** (turun 31% dari Rp 11,0 M)
- Margin laba bersih **4,1%** (turun dari 6,8% di 2024)

**Pertanyaan direksi:** *"Pendapatan naik, tapi laba turun. Apa yang sebenarnya terjadi, dan apa yang harus kami kerjakan tahun depan?"*

**Tren lima tahun:**
| Tahun | 2021 | 2022 | 2023 | 2024 | 2025 |
|---|---|---|---|---|---|
| Pendapatan (Rp M) | 78,4 | 96,2 | 128,5 | 161,9 | 184,6 |
| Margin laba bersih | 5,2% | 6,1% | **7,4%** (puncak) | 6,8% | **4,1%** |

- Margin **berbalik arah sejak 2023** (puncak 7,4%), sementara pendapatan terus naik.
- Pertumbuhan pendapatan **melambat**: +33,6% (2023) → +14,0% (2025).

**Evidence yang terkumpul (Obtain & Analyze):**
| Metrik | Kopi Nusa Rasa | Pembanding | Selisih | Sumber |
|---|---|---|---|---|
| Service time rata-rata | 12,0 menit | 8,6 menit | +40% | Log kasir 2025 |
| Service time jam sibuk | 17,0 menit | 8,6 menit | +98% | Observasi 9 gerai |
| Transaksi/gerai/hari | 214 | 260 | −18% | POS vs riset pasar |
| Nilai rata-rata transaksi | Rp 38.500 | Rp 36.200 (2024) | +6,4% | POS 2024–2025 |
| Turnover barista | 47% | 32% | +15 poin | Data SDM 2025 |
| Margin kotor | 62% | 65% | −3 poin | Laporan keuangan |
| Pangsa pasar Lampung | 23% | 16% (pesaing teratas) | +7 poin | Riset pasar 2025 |
| NPS | +22 | +41 (jaringan nasional) | −19 poin | Survei 1.240 pelanggan |
| Pembelian ulang (member) | 34% | 50% (target internal) | −16 poin | Aplikasi member |

Tiga kolom terakhir (**pembanding, besaran selisih, sumber**) yang membedakan tabel dari "daftar angka".

**Benchmark service time (menit):**
- Benchmark industri **8,6**
- Rata-rata 38 gerai **12,0** (+40%)
- Gerai turnover **< 30%**: **10,2**
- Gerai turnover **> 50%**: **14,1**
- 9 gerai tersibuk jam sibuk: **17,0** (hampir dua kali benchmark)

Catatan: dua batang tengah (turnover vs service time) menunjukkan **asosiasi, bukan bukti sebab-akibat**.

**Diagnosa (kunci):** *"Masalahnya bukan seluruh jaringan, melainkan **jam sibuk di gerai bervolume tinggi**."*
- Rata-rata (12,0) menyembunyikan letak masalah → terlihat merata
- Setelah diurai: gerai tenang 10,2 (hampir wajar) vs gerai tersibuk 17,0
- **Konsekuensi anggaran:** rata-rata membuat direksi membiayai **38 gerai**; angka yang terurai cukup membenahi **9 gerai**.

### SWOT Kopi Nusa Rasa (versi lengkap, hafalkan angkanya)

**STRENGTH**
- **S1 Posisi pasar regional**: pangsa 23% kedai kopi spesialti Lampung, unggul 7 poin atas pesaing teratas (16%). Riset pasar 2025
- **S2 Pasokan terkunci**: 64% green bean dari 3 koperasi binaan, kontrak 3 tahun, harga **11% di bawah pasar spot** saat harga arabika naik 34%
- **S3 Unit B2B tumbuh**: roastery melayani 27 klien hotel & kafe, pendapatan +41% YoY menjadi Rp 25,8 M (14% total)
- **S4 Daya beli pelanggan naik**: nilai rata-rata transaksi Rp 38.500, naik 6,4% YoY tanpa penolakan harga terukur

**WEAKNESS**
- **W1 Kecepatan layanan**: service time 12 menit, 40% di atas benchmark 8,6; 17 menit jam sibuk, **23% calon pembeli batal antre**
- **W2 Perputaran barista**: turnover 47% vs benchmark F&B 32%; masa kerja rata-rata 7,6 bulan; biaya rekrutmen & pelatihan **Rp 678 juta/tahun (9% laba bersih)**
- **W3 Produktivitas gerai**: 214 transaksi/gerai/hari, 18% di bawah pembanding 260
- **W4 Retensi lemah**: pembelian ulang 34% dari target 50%; hanya **18% dari 61.000 anggota** aplikasi aktif tiap bulan

**OPPORTUNITY**
- **O1 Pasar masih tumbuh**: konsumsi kopi spesialti nasional +12,4%/tahun (2022–2025). Laporan asosiasi industri
- **O2 Basis anggota menganggur**: **50.000 anggota tidak aktif**; simulasi internal: kenaikan pembelian ulang 8 poin = **+Rp 9,1 M** pendapatan setahun (+4,9%)
- **O3 Permintaan B2B perhotelan**: kunjungan wisatawan ke Lampung +19% pada 2025; segmen B2B bermargin **37%**, baru menyentuh 27 klien
- **O4 Hibah pengolahan kopi**: pemda mengalokasikan Rp 25 M untuk UMKM pengolahan kopi 2026, dengan pendampingan sertifikasi mutu

**THREAT**
- **T1 Komisi pesan-antar naik**: agregator naikkan komisi 20% → 25% mulai Jan 2026; atas pendapatan kanal Rp 44,3 M, tambahan biaya **Rp 2,2 M = 29% laba bersih 2025**
- **T2 Serbuan jaringan nasional**: 14 gerai pesaing baru di Lampung dalam 18 bulan, semua dalam radius 2 km
- **T3 Kontrak pasokan berakhir**: kontrak koperasi habis **Desember 2026**; tanpa perpanjangan, 64% pasokan terekspos harga spot yang naik 34% YoY
- **T4 Biaya tenaga kerja naik**: UMP provinsi +6,5% pada 2026, menekan gerai yang produktivitasnya sudah 18% di bawah pembanding

> Cek hitungan: 5% × 44,3 M ≈ 2,2 M · 2,2/7,6 ≈ 29% · 678 jt/7,6 M ≈ 9% · 9,1/184,6 ≈ 4,9% · 50.000/61.000 ≈ 82% tidak aktif (jadi 18% aktif).

### Memasangkan kuadran → business implication
| Pasangan | Strategi | Penjelasan |
|---|---|---|
| **S × O** (kekuatan untuk peluang) | **Perbesar kanal B2B perhotelan** | S2 + S3 bertemu O3: pasokan terkunci dan roastery yang tumbuh 41% dipakai menggarap pasar hotel (+19% wisatawan). Margin 37% dan **tidak membebani antrean gerai** |
| **W × O** (tutup kelemahan lewat peluang) | **Aktifkan 50.000 anggota yang menganggur** | W4 bertemu O2: pembelian ulang 34% → 42% lewat kampanye aplikasi. Dampak **+Rp 9,1 M**, tanpa buka gerai baru |
| **S × T** (kekuatan untuk menahan ancaman) | **Perpanjang kontrak koperasi lebih awal** | S2 menahan T3: perpanjang sebelum Des 2026 mengunci keunggulan harga 11% atas 64% pasokan → perlindungan ≈ **Rp 2,0 M** biaya/tahun |
| **W × T** (bertahan dari risiko ganda) | **Benahi antrean jam sibuk lebih dulu** | W1 bertemu T1 dan T2: antrean lambat membuat pelanggan beralih ke pesaing baru atau ke kanal pesan-antar yang komisinya naik. Memperbaiki service time menahan **dua ancaman sekaligus** |

Baris pada latihan: **Baris depan S×O · Baris tengah W×O · Baris belakang S×T · Baris paling belakang W×T.**

### Keputusan akhir — mengurutkan dengan dampak dan upaya
| Inisiatif | Taksiran dampak setahun | Biaya | Waktu | Urutan |
|---|---|---|---|---|
| Pisahkan jalur pesanan daring di 9 gerai tersibuk | +Rp 4,0 M pendapatan tertahan | Rp 420 jt | 2 kuartal | **1 · Kerjakan** |
| Perpanjang kontrak koperasi lebih awal | Rp 2,0 M biaya terhindar | Rp 80 jt | 1 kuartal | **1 · Kerjakan** |
| Program aktivasi anggota aplikasi | +Rp 9,1 M pendapatan | Rp 650 jt | 3 kuartal | **2 · Kerjakan** (dalam matriks: *Rencanakan*) |
| Jenjang karier & bonus retensi barista | Rp 678 jt biaya rekrutmen terhindar | Rp 900 jt | 4 kuartal | **2 · Uji dulu** (matriks: *Rencanakan*) |
| Bangun kanal pemesanan langsung sendiri | Sebagian dari Rp 2,2 M komisi | Rp 1,2 M | 4 kuartal | **3 · Tunda** |
| Buka 6 gerai baru pada 2026 | **Belum terukur** | Rp 7,2 M | 4 kuartal | **4 · Jangan dulu** |

**Matriks dampak–upaya:**
- **Dampak tinggi · upaya rendah → KERJAKAN SEKARANG**: (1) pisahkan jalur pesanan daring +Rp 4,0 M; (2) perpanjang kontrak koperasi Rp 2,0 M
- **Dampak tinggi · upaya tinggi → RENCANAKAN**: (3) aktivasi 50.000 anggota +Rp 9,1 M; (4) retensi barista Rp 678 jt
- **Dampak rendah · upaya rendah → ISI WAKTU LUANG**: (5) samakan definisi metrik antar gerai
- **Dampak belum terukur · upaya tinggi → JANGAN DULU**: (6) kanal pemesanan sendiri; (7) buka 6 gerai baru

Kotak kanan bawah bukan berarti buruk, hanya **belum punya bukti cukup untuk dibiayai sekarang**. Buka gerai baru adalah *"yang paling sering disetujui, dan paling sering salah."*

**Jawaban untuk direksi (kalimat kunci):** *"Laba turun bukan karena kurang pelanggan, melainkan karena gerai yang ada belum mampu melayani permintaan yang sudah datang. Benahi kapasitas dan retensi lebih dulu; ekspansi gerai ditunda sampai produktivitas mendekati 260 transaksi per hari."*

**Hubungan dengan SOAR:** *Specify* (pertanyaan direksi dipertajam) → *Obtain* (tabel evidence + uji kualitas) → *Analyze* (tren, benchmark, segmentasi per gerai → diagnosa) → *Report* (SWOT berangka → implication → jawaban satu kalimat + urutan prioritas).

## B12. Brief Tugas Kelompok (Latihan)
- **Format**: kelompok 4–5 orang · satu ide bisnis UMKM atau perusahaan · dikerjakan 20 menit · presentasi 5 menit
- **Yang dikumpulkan**: tabel evidence (min. **8 metrik**) · matriks SWOT (maks. **4 butir** per kuadran) · **4 business implication** · tabel prioritas & rekomendasi
- **Aturan**: tiap butir SWOT **wajib berangka** · butir tanpa angka **tidak dinilai** · tulis **keterbatasan data** · minimal satu **"jangan dulu"**
- Alur: **Evidence → SWOT → Business implication**

## B13. Lima Hal yang Dibawa Pulang
1. SOAR adalah prosesnya, SWOT salah satu keluarannya. **SWOT tidak pernah jadi langkah pertama.**
2. Analisis dimulai dari **pertanyaan yang terikat pada keputusan**, bukan dari data yang kebetulan tersedia.
3. Setiap butir SWOT memuat **klaim, metrik, pembanding, periode, sumber**. Kata sifat saja tidak cukup.
4. **Besaran dampak dalam rupiah** membuat prioritas bisa dihitung, bukan diperdebatkan.
5. Analisis selesai ketika seseorang **tahu apa yang harus dikerjakan besok pagi**, bukan ketika matriksnya penuh.

---

# BAGIAN C — CHEAT SHEET & LATIHAN SOAL

## C1. Cheat sheet satu halaman

**Konsep kunci**
- Finding = APA (deskriptif). Cause = MENGAPA (eksplanatif, bisa ditindaklanjuti).
- Bukti = bisa diperiksa (angka, periode, populasi, pembanding). Asumsi = dugaan belum diuji.
- "Karena" ≠ bukti. Yang membuat penyebab adalah **data di belakangnya**.
- Persempit dulu (drill-down, comparison, variance, segmentation), baru gali (5 Whys, RCA), lalu uji kausal.

**Rumus**
- Revenue = Harga × Volume
- Efek harga = (P₁ − P₀) × Q₁ · Efek volume = (Q₁ − Q₀) × P₀
- Elastisitas = %Δ volume ÷ %Δ harga (−64% ÷ +10% = −6,4)
- Kontribusi = selisih bagian ÷ selisih total (mis. 5,4 ÷ 10,0 = 54%)
- Laba usaha = Revenue − HPP − Beban usaha; Marjin kotor = (Revenue − HPP) ÷ Revenue
- Margin bersih = laba bersih ÷ pendapatan

**Daftar**
- 4 tingkat analitik: Descriptive, Diagnostic, Predictive, Prescriptive
- 7 teknik: Drill-down, Comparison, Variance, Segmentation, 5 Whys, RCA, Causal thinking
- 5 langkah: Problem → Dimension → Drill-down → Evidence → Cause
- 5 uji kausal: Waktu, Mekanisme, Pembanding, Dosis-respons, Alternatif tersingkir
- 5 bias: Confirmation, Anchoring, Survivorship, Single-cause, Post hoc
- 4 bentuk asumsi menyamar: angka tanpa pembanding, anekdot, korelasi=sebab, otoritas
- 4 bagian laporan: Finding, Evidence, Cause, Action
- SOAR: Specify, Obtain, Analyze, Report
- 4 unsur pertanyaan bisnis: Subjek, Batas, Pembanding, Keputusan
- 3 sumber evidence: Internal (S/W), Eksternal (O/T), Primer
- 5 dimensi kualitas data: Kelengkapan, Akurasi, Kebaruan, Konsistensi, Keterlacakan
- 3 jebakan data: yang kecewa sudah pergi, sampel tidak mewakili, metrik pengganti keliru
- 5 unsur butir SWOT: Klaim, Metrik, Pembanding, Periode, Sumber
- 5 teknik analisis (modul SOAR): Benchmark, Tren, Segmentasi, Dekomposisi, Akar masalah
- What / So what / Now what
- Dampak–upaya: Kerjakan sekarang / Rencanakan / Isi waktu luang / Jangan dulu

**Angka-angka kasus yang sering ditanya**
- Nusantara Segar: Revenue 50→40 (−20%), laba 6,0→3,7 (−38%), marjin kotor 30% tetap; Region X −7,0 (70%); Produk A Region X −5,4 (54%); harga 25.000→27.500 (+10%); volume 360.000→130.000 (−64%); efek harga +0,33, volume −5,75, bersih −5,42; elastisitas −6,4; repeat purchase 62%→46% (−25% relatif); pesaing Rp 24.500 (selisih 12%); Region Y/Z −5%/−6%; warung kecil −74% (63% kehilangan volume); service level 97%; keluhan mutu 0,3%; kunjungan sales +4%.
- Kopi Nusa Rasa: pendapatan 184,6 M (+14,0%), laba 7,6 M (−31%), margin 6,8%→4,1%; service time 12,0 vs 8,6 (+40%), jam sibuk 17,0 (+98%); 9 gerai tersibuk; 23% batal antre; turnover 47% vs 32%; 214 vs 260 transaksi; pangsa 23% vs 16%; NPS +22 vs +41; repeat 34% vs 50%; 61.000 member (hanya 18% aktif, 50.000 tidak aktif); +Rp 9,1 M aktivasi; Rp 4,0 M jalur daring (biaya 420 jt); komisi 20→25% (Rp 2,2 M, 29% laba); kontrak habis Des 2026; harga pasokan 11% di bawah spot; arabika +34%; B2B 27 klien, margin 37%, Rp 25,8 M (+41%).

## C2. Latihan soal (jawab dulu, baru cek kunci di bawah)

**Pilihan tegas / klasifikasi**
1. "Penjualan wilayah Sumatera turun 12% pada Q3." Finding atau cause?
2. "Penjualan turun karena karyawan malas." Mengapa ini disebut asumsi?
3. "Biaya logistik naik karena rute dipecah dua setelah gudang transit ditutup Agustus (data: perbandingan rute sebelum–sesudah)." Finding atau cause?
4. Sebutkan 4 ciri analisis diagnostik yang baik (3 syarat definisi + 1 uji akhir rekomendasi).
5. Bias apa: tim hanya menganalisis pelanggan yang masih aktif dan mengabaikan yang berhenti membeli?
6. Bias apa: setelah promo berjalan, penjualan naik, tim menyimpulkan promo penyebabnya tanpa kelompok pembanding?
7. Bias apa: tim terpaku pada penjelasan pertama bosnya di rapat?
8. Mengapa Region Y dan Z penting dalam kasus Nusantara Segar?
9. Tulis rumus efek harga dan efek volume. Hitung bila harga 20.000 → 22.000 dan volume 1.000 → 600.
10. Mengapa "ikuti kontributor terbesar, bukan persentase terbesar" dalam drill-down?
11. Jelaskan perbedaan drill-down dan segmentation.
12. Apa beda 5 Whys dan RCA?
13. Sebutkan 3 kegagalan 5 Whys.
14. Sebutkan lima uji sebelum menyebut sesuatu penyebab, dan bukti masing-masing pada kasus Nusantara Segar.
15. Mengapa kesimpulan "turnover barista tinggi → service time lambat → naikkan gaji" terburu-buru? Sebut tiga pertanyaan penjaga.

**SOAR**
16. Tahap SOAR apa: (a) mengunduh data POS; (b) menyusun pertanyaan; (c) memeriksa baris kosong; (d) membandingkan gerai; (e) menulis memo satu kalimat?
17. Mengapa SWOT bukan langkah pertama?
18. Bagaimana mengubah "Kenapa penjualan turun?" menjadi pertanyaan kerja? Sebutkan empat unsurnya.
19. Jebakan data apa: kepuasan hanya diukur lewat formulir di kasir?
20. Jebakan apa: loyalitas diukur dengan jumlah followers?
21. Tuliskan lima unsur butir SWOT. Unsur apa yang hilang dari "Turnover barista 47% vs benchmark 32% (data SDM)"?
22. Tempatkan: (a) komisi agregator naik, (b) rating aplikasi 4,6 vs 4,2, (c) kapasitas dapur maks 250 porsi, (d) UMP naik 6,5%.
23. Apa dua pertanyaan untuk menentukan kuadran SWOT?
24. Mengapa maksimal 4 butir per kuadran?
25. Jelaskan What / So what / Now what dengan contoh.

**Kasus**
26. Kopi Nusa Rasa: mengapa menurut diagnosa "rata-rata 12 menit" menyesatkan? Apa konsekuensi anggarannya?
27. Kopi Nusa Rasa: tulis strategi W×T dan alasannya.
28. Kopi Nusa Rasa: mengapa "buka 6 gerai baru" ditaruh di "Jangan dulu"?
29. Kopi Nusa Rasa: urutkan inisiatif berikut dari yang pertama dikerjakan: aktivasi anggota, jalur daring, kontrak koperasi, retensi barista, buka gerai.
30. Ayam Geprek: strategi ST apa yang direkomendasikan, dan mengapa WT memilih kontrak harga pemasok?
31. Hitung: Pendapatan Kopi Nusa Rasa 2025 Rp 184,6 M, laba bersih Rp 7,6 M. Berapa margin bersih?
32. Hitung: Aktivasi anggota +Rp 9,1 M dari pendapatan 184,6 M. Berapa persen kenaikannya?
33. Hitung: segmen warung kecil 198.000 → 52.000 unit. Berapa persen penurunannya, dan berapa persen sumbangannya ke total kehilangan 230.000 unit?

---

## C3. Kunci jawaban

1. **Finding.** Hanya melaporkan perubahan angka; belum menjelaskan mengapa, tanpa dimensi/pemicu.
2. Berbentuk penyebab ("karena"), tetapi **tidak terukur**: tidak ada angka, periode, pembanding, atau sumber data. Tidak bisa diuji atau dibantah.
3. **Cause**: menyebut dimensi (rute), pemicu (penutupan gudang transit Agustus), mekanisme, dan didukung data sebelum–sesudah.
4. Sistematis (bukan intuitif); berbasis bukti; dapat ditindaklanjuti; dan rekomendasinya menunjuk pada **keputusan yang bisa diubah** (bukan sifat pelanggan/keadaan pasar).
5. **Survivorship bias.** Penangkal: analisis kelompok yang hilang (churn, pesanan batal, keranjang ditinggalkan).
6. **Post hoc reasoning.** Penangkal: kelompok pembanding yang tidak mengalami promo.
7. **Anchoring.** Penangkal: rumuskan minimal tiga hipotesis sebelum melihat data pendukung.
8. Mereka **kelompok kontrol alami**: harga tidak diubah dan revenue hanya turun 5–6%. Jika penurunan karena faktor umum (musim/ekonomi), Y dan Z akan ikut turun besar. Ini mendukung uji "kelompok pembanding".
9. Efek harga = (P₁−P₀)×Q₁ = (22.000−20.000)×600 = **+1.200.000**. Efek volume = (Q₁−Q₀)×P₀ = (600−1.000)×20.000 = **−8.000.000**. Bersih = **−6.800.000** (cek: revenue 20 jt → 13,2 jt = −6,8 jt ✓). Volume turun 40%, harga naik 10% → elastisitas −4,0.
10. Karena penurunan besar persentase pada lini kecil jarang menjelaskan masalah perusahaan. Yang perlu dicari adalah sel yang menyumbang paling besar pada **total selisih** (mis. Produk A Region X = 54%).
11. Drill-down memecah menurut **struktur organisasi** (region → produk). Segmentation memecah menurut **perilaku/karakteristik pelanggan atau transaksi** (ukuran toko, frekuensi beli, kanal, siklus hidup), dan sering di situlah sebab bersembunyi.
12. 5 Whys menelusuri **satu jalur** sebab berlapis. RCA **memetakan semua kandidat** penyebab (harga, produk, distribusi, tenaga penjual, proses, eksternal) lebih dulu lalu menyaringnya dengan bukti.
13. Pilih tiga: berhenti pada orang; rantai tanpa bukti; melompat lapisan; satu jalur tunggal.
14. (1) Urutan waktu: harga berubah 1 Juli, penurunan mulai minggu kedua Juli. (2) Mekanisme: harga naik → selisih 12% → pelanggan berpindah. (3) Pembanding: Region Y/Z hanya turun 5–6%. (4) Dosis–respons: warung kecil (paling sensitif) turun 74%. (5) Alternatif tersingkir: service level 97%, keluhan mutu stabil, Produk B–D stabil.
15. Itu korelasi, belum kausalitas. Tiga pertanyaan: **Arah** (mungkin gerai kacau membuat barista keluar), **Faktor ketiga** (mungkin volume tinggi/dapur sempit), **Kebetulan** (jumlah gerai dan lama periode). Uji: bandingkan gerai bervolume setara atau amati sebelum–sesudah.
16. (a) Obtain; (b) Specify; (c) Obtain; (d) Analyze; (e) Report.
17. Karena SWOT hanya wadah keluaran; isinya sebaik proses yang menghasilkannya. Ia **langkah keempat** setelah pertanyaan, bukti, dan analisis.
18. Tambahkan **Subjek** (metrik), **Batas** (unit, waktu, tempat), **Pembanding** (benchmark/target/periode lalu), **Keputusan** (tindakan yang menunggu jawaban). Contoh: "Berapa penurunan penjualan gerai mal vs jalan raya pada Q4 2025 terhadap Q3, dan apakah cukup besar untuk menunda gerai baru?"
19. **Yang kecewa sudah pergi** (survivorship): pelanggan yang kapok tidak pernah mengisi.
20. **Metrik pengganti yang keliru**: yang ingin diukur pembelian ulang, bukan pengikut.
21. Klaim, Metrik, Pembanding, Periode, Sumber. Yang hilang pada contoh = **Periode**.
22. (a) Threat; (b) Strength; (c) Weakness; (d) Threat.
23. "Bisa diubah perusahaan sendiri dalam setahun?" (ya = internal, tidak = eksternal) dan "Membantu atau menghambat tujuan?" (membantu = S/O, menghambat = W/T).
24. Agar fokus: daftar panjang tanpa urutan membuat semua terasa sama penting dan tak ada yang dikerjakan. Diurutkan dari dampak terbesar.
25. What = apa yang terlihat di data (service time jam sibuk 17 menit, 23% batal). So what = artinya bagi bisnis dalam rupiah/risiko (≈ Rp 4,0 M/tahun hilang). Now what = tindakan, pemilik, biaya, waktu (pisahkan jalur daring, Manajer Operasional, Rp 420 jt, target 11 menit dalam 2 kuartal).
26. Rata-rata menyatukan gerai tenang (10,2) dan gerai tersibuk (17,0) sehingga tampak masalah merata. Setelah diurai, masalah terkonsentrasi pada jam sibuk di 9 gerai. Konsekuensi: tanpa penguraian direksi membiayai 38 gerai; padahal cukup membenahi 9.
27. W1 (antrean jam sibuk) × T1 (komisi pesan-antar naik) dan T2 (14 gerai pesaing baru): **benahi antrean jam sibuk lebih dulu**. Antrean lambat membuat pelanggan beralih ke pesaing atau ke kanal pesan-antar yang komisinya naik; memperbaiki service time menahan dua ancaman sekaligus.
28. Dampaknya **belum terukur**, upaya tinggi (Rp 7,2 M, 4 kuartal), dan produktivitas gerai yang ada masih 214 vs 260. Masalahnya kapasitas melayani permintaan, bukan kekurangan gerai. Tunda sampai produktivitas mendekati 260 transaksi/hari.
29. Pertama: jalur daring (+Rp 4,0 M) dan kontrak koperasi (Rp 2,0 M; murah dan cepat) → lalu aktivasi anggota (+Rp 9,1 M) → retensi barista (uji dulu) → (kanal pemesanan sendiri ditunda) → buka gerai (jangan dulu).
30. ST: gunakan rating 4,6 sebagai senjata branding melawan 12 pesaing dalam radius 3 km. WT: kontrak harga dengan pemasok cabai dan ayam karena kelemahan (ketergantungan/skala kecil) bertemu ancaman fluktuasi harga bahan baku.
31. 7,6 ÷ 184,6 ≈ **4,1%**.
32. 9,1 ÷ 184,6 ≈ **4,9%**.
33. Penurunan = (198.000−52.000)/198.000 ≈ **−74%**. Kehilangan = 146.000; 146.000/230.000 ≈ **63%**.

---

## Catatan
- File ini disusun dari dua deck: *Diagnostic Business Analysis & Root Cause Analysis* (slide 1–37) dan *SOAR & SWOT* (Modul 6). Slide yang tidak tercantum di PDF (mis. beberapa nomor yang lompat) tidak dibahas di sini.
- Semua angka PT Nusantara Segar bersifat **ilustratif** menurut slide.
- Saran belajar malam ini: (1) kerjakan soal C2 tanpa melihat kunci; (2) hafalkan angka-angka kunci di C1; (3) latih menjelaskan alur kasus Nusantara Segar dan Kopi Nusa Rasa secara lisan dalam satu menit masing-masing.

Semoga sukses kuisnya! 🎯
