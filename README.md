# Digitalisasi Dokumen: OCR Struk dan Nota Belanja

Proyek kelompok **Pengolahan Citra Digital 2026** · kelas `ti23ka` · topik **T4**

[![Cek proyek](https://github.com/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t4/actions/workflows/cek-proyek.yml/badge.svg)](https://github.com/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t4/actions/workflows/cek-proyek.yml)

**Lingkup kelompok kami:** Struk dengan total tertulis (currency random)

Meluruskan dan membersihkan foto struk, lalu membaca teks dan mengambil isian penting. Anggota dan perannya ada di [ANGGOTA.yml](ANGGOTA.yml); cara kerja kelompok ada di [PANDUAN.md](PANDUAN.md).

## Notebook

| Notebook | Tahap | Isi | Buka |
| --- | --- | --- | --- |
| `01_dataset_preprocessing.ipynb` | 1 | Statistik dataset, cek anotasi, preprocessing, gambar sebelum–sesudah | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t4/blob/main/notebooks/01_dataset_preprocessing.ipynb) |
| `02_metode_klasik.ipynb` | 2 | 2 metode klasik dan metriknya | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t4/blob/main/notebooks/02_metode_klasik.ipynb) |
| `03_metode_modern.ipynb` | 2 | Inferensi model pralatih dan metriknya | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t4/blob/main/notebooks/03_metode_modern.ipynb) |
| `04_evaluasi.ipynb` | 2 | Tabel perbandingan, uji ablasi, kasus gagal | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prodi-TI-IBIKesatuan/pcd2026-ti23ka-t4/blob/main/notebooks/04_evaluasi.ipynb) |

## Dataset (Tahap 1)

- Jumlah citra: 200
- Foto sendiri: Alex: 29, Rhainy, Steven, Tania : 15
- Sumber data tambahan dan lisensinya: Receipt Computer Vision Model by savan, via Roboflow : https://universe.roboflow.com/savan-x6w9q/receipt-rlnml/browse?queryText=&pageSize=100&startingIndex=200&browseQuery=true , license CC BY 4.0 
- Langkah preprocessing: [isi, ringkas dan berurutan]

Rincian dataset, format anotasi, dan tautan Drive: [data/README.md](data/README.md). Contoh sebelum–sesudah ada di [outputs/figures/](outputs/figures/).

## Hasil (Tahap 2)

| Metode | Jenis | CER | Akurasi isian |
| --- | --- | --- | --- |
| [isi: nama metode klasik 1] | klasik | [isi] | [isi] |
| [isi: nama metode klasik 2] | klasik | [isi] | [isi] |
| [isi: nama model] | modern | [isi] | [isi] |

- **Uji ablasi:** [isi: parameter atau langkah yang diubah, dan pengaruhnya pada metrik]
- **Kasus gagal:** [isi: minimal 3 contoh dan penyebabnya, gambar di outputs/figures/]
- **Kesimpulan:** [isi: metode mana yang terbaik untuk lingkup kami dan mengapa]

## Demo

Aplikasi: [isi: tautan https://huggingface.co/spaces/...]

Unggah foto struk, tampilkan dokumen yang sudah diluruskan, teks, tanggal, dan total. Kode aplikasi ada di [app/](app/).

## Sumber dan atribusi
Tuliskan setiap kode, model, dataset, atau bantuan AI yang dipakai beserta sumbernya. Pemakaian tanpa sumber dihitung plagiarisme.

| Yang dipakai | Sumber | Dipakai untuk |
| --- | --- | --- |
| Dataset (hanya gambar) | Receipt Computer Vision Model by savan, via Roboflow : https://universe.roboflow.com/savan-x6w9q/receipt-rlnml/browse?queryText=&pageSize=100&startingIndex=200&browseQuery=true | Dataset Tambahan |
| PaddleOCR | https://github.com/PaddlePaddle/PaddleOCR | Ekstrasi Teks dari gambar dataset untuk dijadikan anotasi |
