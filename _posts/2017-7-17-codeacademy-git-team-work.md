---
layout: post
title: Codeacademy git Teamwork
---

Codeacademy git kullanım notları üzerine güzel bir özet. Teamwork üzerine güzel anlatım var.
####İşin özünde:
1. deponun bir kopyasını al. git clone
2. Herhangi bir değişiklik var mı diye kontrol et. git fetch
3. Değişiklikleri birleştir. git merge
4. Yerel deponda yeni bir dal oluştur. git branch branch_name
5. Yeni dala geç. git checkout branch_name
6. Yine bir fetch merge yap ki bu arada birileri bişeyler eklediyse sıkıntı çıkmasın :)
7. Yaptığın değişiklikleri gönder. git push origin branch_name
8. Bunlardan sonra gönderdiğin değişiklikleri origin/master yetkilisi kimse merge eder artık :)


We also learned the following commands

`git clone`: Creates a local copy of a remote.

`git remote -v`: Lists a Git project's remotes.

`git fetch`: Fetches work from the remote into the local copy.

`git merge origin/master`: Merges origin/master into your local branch.

`git push origin <branch_name>`: Pushes a local branch to the origin remote.
