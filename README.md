# visualization-data

Repositori tugas mata kuliah **Visualisasi Data Lanjut (CAK7AGB4)**, Program Studi Magister Informatika, Telkom University.

- **Nama:** Salman Rachmadi
- **NIM:** 203012420009

## Alur branch

- `master` berisi informasi repositori ini dan semua tugas yang sudah selesai.
- Setiap tugas dikerjakan di branch tersendiri yang dinamai sesuai tugasnya, misalnya `week4` untuk tugas minggu ke-4.
- Setelah tugas selesai, branch-nya di-push lalu di-merge ke `master`.

Tugas berikutnya mengikuti alur yang sama. Contoh untuk tugas minggu ke-4:

```bash
git checkout master
git checkout -b week4        # mulai tugas
# ... kerjakan, commit ...
git push -u origin week4     # push branch tugas
git checkout master
git merge week4              # setelah tugas selesai
git push origin master
```

## Daftar tugas

| Branch | Tugas | Status |
| --- | --- | --- |
| `week4` | Tugas 1 — Audit Data dan Exploratory Data Analysis | Dikerjakan |

## Struktur folder

Setiap tugas punya folder sendiri dengan susunan yang sama:

```
week4/
├── task/       panduan tugas
├── data/       dataset
└── notebook/   notebook pengerjaan
```

## Menjalankan notebook

Butuh Python 3 dengan `pandas`, `numpy`, `matplotlib`, `seaborn`, dan Jupyter. Notebook membaca dataset lewat path relatif (`../data/...`), jadi jalankan dari folder `notebook/` tugas yang bersangkutan.
