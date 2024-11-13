### setup
- ```git init```                                     // Inisialisasi repositori Git baru
- ```git config --global user.name "Your Name"```     // Setel nama pengguna global
- ```git config --global user.email "your.email@example.com"``` // Setel email pengguna global
- ```git add .```                                     // Tambahkan semua perubahan ke staging
- ```git commit -m "Initial commit"```                // Commit perubahan dengan pesan
- ```git remote add origin <repository-url>```        // Tambahkan remote repository
- ```git branch -M main```                            // Ubah nama branch utama ke 'main'
- ```git push -u origin main```                       // Push data ke branch 'main' di GitHub

### Branch management
- ```git checkout -b <nama_branch>```                // Buat dan pindah ke branch baru
- ```git branch -d <nama_branch>```                   // Hapus branch lokal
- ```git branch -D <nama_branch>```                   // Paksa hapus branch lokal
- ```git push origin --delete <nama_branch>```        // Hapus branch di remote (GitHub)
- ```git checkout <nama_branch>```                    // Pindah ke branch lain yang sudah ada

### Pull & Push changes
- ```git pull origin <nama_branch>```                 // Tarik (pull) perubahan dari GitHub
- ```git push origin <nama_branch>```                 // Push perubahan ke branch di GitHub

### Undo & Reset changes
- ```git reset --hard <commit_id>```                  // Reset ke commit tertentu, menghapus perubahan
- ```git reset --soft <commit_id>```                 // Reset ke commit tertentu, simpan perubahan di staging
- ```git checkout -- <filename>```                    // Buang perubahan di file tertentu
- ```git revert <commit_id>```                       // Revert commit tertentu (membuat commit baru yang membatalkan perubahan)