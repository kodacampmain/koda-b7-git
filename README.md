# GIT BASICS

## **1. Git system initialization**
```sh
$ git init
```

## **2. Save into staging area (temporary changes)**
```sh
$ git add [filepath...]
```

## **3. Commit (permanent changes)**
```sh
$ git commit [option] [argument]
```
&nbsp;&nbsp;&nbsp;&nbsp; 
option:
- ``-m`` : menambahkan pesan commit
```sh
$ git commit -m "type: description"
```
- ``--amend``: memperbaiki pesan commit yang baru saja terjadi

**Commit dengan pesan panjang**
```sh
$ git commit
```

## **4. Remote Repository**
- ``remote`` command
```sh
$ git remote [command] [argument]
```
```sh
# view remote list
$ git remote
# add remote repository
$ git remote add [remote_name] [remote_url]
# view remote url
$ git remote get-url [remote_name]
```

- Sinkronisasi dengan ``push`` dan ``pull``
```sh
# sinkronisasi dari lokal ke remote
$ git push [remote_name] [branch_name]
# sinkronisasi dari remote ke lokal
$ git pull [remote_name] [branch_name]
```

## **5. Config**
## **6. Cloning**
Replikasi identik
```sh
# jika ingin menggunakan nama folder sama dengan nama repo
$ git clone [url]
# jika ingin menggunakan nama folder berbeda dari naam repo
$ git clone [url] [namaFolder]
```
namaFolder diberikan jika menginginkan nama folder yang berbeda dengan nama repo

## **7. History**
- ``log`` = riwayat commit publik
```sh
$ git log
```
- ``reflog`` = riwayat git yang lebih private, tidak hanya riwayat commit namun juga riwayat lain seperti ``pull``, ``reset`` dan ``revert``
```sh
$ git reflog
```
## **8. Undoing Changes**
- ``revert`` = menghilangkan commit dengan commit revert yang baru
```sh
$ git revert [commit_code]
```
- ``reset`` = mundur ke titik commit tertentu
```sh
$ git reset [commit_code]
```

## **9. Branching**
- ``branch``
```sh
$ git branch [option] [argument]
```
```sh
# list branch
$ git branch
# create new branch
$ git branch [branch_name]
# rename branch
$ git branch [-m|-M] [old_branch] [new_branch]
# copy branch
$ git branch [-c|-C] [source_branch] [dest_branch]
# delete branch
$ git branch [-d|-D] [branch_name]
```
- ``checkout``
```sh
# moving between branch
$ git checkout [dest_branch]
# moving to branch (and create it if not exists)
$ git checkout -b [branch_name]
# moving between commit
$ git checkout [commit_code]
```
- ``merge``
```sh
# you have to move to destination branch first
$ git merge [source_branch...]
```
