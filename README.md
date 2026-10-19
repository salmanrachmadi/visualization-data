# visualization-data

Repositori tugas mata kuliah **Visualisasi Data Lanjut (CAK7AGB4)**, Program Studi Magister Informatika, Telkom University.

- **Nama:** Salman Rachmadi
- **NIM:** 203012420009

## Isi repositori

Repositori ini memuat seluruh pengerjaan mata kuliah:

- **Tugas mingguan**, di folder dan branch `week<N>` (misalnya `week4`, `week5`).
- **Midterm project**, di folder dan branch `midterm`.
- **Final project**, di folder dan branch `final`.

## Alur branch

- `master` berisi informasi repositori ini dan semua pekerjaan yang sudah selesai.
- Setiap pekerjaan dikerjakan di branch tersendiri sesuai namanya: `week<N>`, `midterm`, atau `final`.
- Setelah pekerjaan selesai, branch-nya di-push lalu di-merge ke `master` (langsung atau lewat pull request).

```bash
git checkout master
git pull origin master
git checkout -b <branch>       # week<N>, midterm, atau final
# ... kerjakan, commit ...
git push -u origin <branch>
# setelah selesai: buka pull request ke master, atau merge manual
git checkout master
git merge <branch>
git push origin master
```

## Struktur folder

Setiap pekerjaan punya folder sendiri bernama sesuai branch-nya dan berisi tiga bagian:

```
<branch>/
├── <panduan>/    panduan tugas (PDF) dan laporan akhir
├── <dataset>/    dataset tugas
└── <notebook>/   notebook pengerjaan beserta gambar yang dihasilkan
```

Nama subfolder bisa sedikit berbeda antarpekerjaan (misalnya `task/` atau `tasks/`, `data/` atau `datasets/`).

## Menjalankan notebook

Butuh Python 3 dengan `pandas`, `numpy`, `matplotlib`, `seaborn`, dan Jupyter. Tugas tertentu bisa butuh pustaka tambahan, misalnya `statsmodels` untuk analisis deret waktu.

Notebook membaca dataset lewat path relatif (misalnya `../data/...` atau `../datasets/...`), jadi jalankan dari folder notebook pekerjaan yang bersangkutan.
