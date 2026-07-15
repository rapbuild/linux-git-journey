# Day 4 - Git Diff, Staging Area, and Restore

## Tujuan
Memahami bagaimana Git mengelola perubahan file sebelum disimpan menjadi commit.

## Materi
- **Working Directory** adalah tempat file yang sedang diedit.
- **Git Diff** digunakan untuk melihat perbedaan antara file yang sedang diedit dengan versi yang ada di Staging Area.
- **Staging Area** adalah tempat sementara untuk menyimpan perubahan sebelum dibuat commit menggunakan `git add`.
- **Git Restore** digunakan untuk membuang perubahan yang belum di-commit dan mengembalikan file ke kondisi sebelumnya.

## Command
```bash
git diff
git add <file>
git restore <file>
```

## Konsep Penting
```
Working Directory
        │
     git add
        ▼
 Staging Area
        │
   git commit
        ▼
 Git Repository
```

## Insight
Hari ini aku memahami bahwa Git tidak langsung menyimpan perubahan ketika file diedit. Perubahan berada di Working Directory, kemudian dipilih menggunakan `git add` ke Staging Area, dan baru disimpan menjadi snapshot melalui `git commit`. Aku juga belajar bahwa `git restore` dapat mengembalikan file ke kondisi sebelumnya jika perubahan belum ingin disimpan.
