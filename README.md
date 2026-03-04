# GIT BASICS

## **1. Git system initialization**
```sh
$ git init
```

## **2. Save into staging area (temporary changes)**
```sh
$ git add [filepath...]
```

### **3. Commit (permanent changes)**
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