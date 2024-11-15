### setup sshkey
- ```ls -al ~/.ssh```                                      // Lists the files in your .ssh directory, if they exist
- ```ssh-keygen -t rsa -C "your_email@example.com"```     // Creates a new ssh key, using the provided email as a label and Enter file in which to save the key (/home/you/.ssh/id_rsa):
- ```eval "$(ssh-agent -s)"```                            // start the ssh-agent in the background
- ```ssh-add ~/.ssh/id_rsa```
- ```cat ~/.ssh/id_rsa.pub```                             // read public key and pair to github & paste into github sshkey
- ```ssh -T git@github.com```                             // verify pairing github n ur device
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
