# Karto Web App

[![Netlify Status](https://api.netlify.com/api/v1/badges/692954fe-90fe-4ea4-80af-533bffbf97bb/deploy-status)](https://app.netlify.com/sites/karto/deploys)


## 0. Requirement

- [Git](https://git-scm.com/downloads)
- [npm](https://nodejs.org/en/) (sudah sepaket dengan Node.js) 


## 1. Memulai

Buka terminal / cmd, arahkan ke direktori tempat penyimpanan projectnya nanti. lalu jalankan:
```bash
# Clone repository ke local dan simpan di folder baru app
$ git clone https://github.com/kartoyo/app.git

# Masuk ke folder hasil clone
$ cd app/

# Gunakan npm untuk menginstall semua yang dibutuhkan
$ npm install
```


## 2. Development

```bash
# serve with hot reload at localhost:3000
$ npm run dev
```


## 3. Test Build Local

```bash
# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```


## 4. Upload perubahan

```bash
# Pastikan udah berada di branch masing-masing (bukan master)
$ git branch --show-current

# Kalo belum di branch masing-masing dan belum bikin branch
$ git checkout -b <nama-branch>

# Kalo udah bikin branch tapi belum di branch masing-masing
$ git checkout <nama-branch>

# Simpan semua perubahan ke git. Setelah commit, perubahan akan secara permanen disimpan di branch yang sedang aktif
$ git add .
$ git commit -m "Masukkan pesan disini"

# Sinkronisasi perubahan dari branch master (skip jika ngga ada)
$ git pull origin master

# Jika udah clone repo sebelum ganti nama, ubah url origin ke nama yang baru
$ git remote set-url origin https://github.com/kartoyo/app.git

# Upload perubahan ke branch masing-masing
$ git push origin <branch-mu>

# Jika branch di Github belum ada, tambahkan -u
$ git push -u origin <branch-mu>

# Jika terlanjur commit & push tapi ada perubahan baru yang pengen digabungin ke commit terakhir:
$ git add .
$ git commit --amend
$ git pull origin master # opsional seperti diatas
$ git push --force origin <branch-mu>
```


## 5. Dokumentasi
- [Nuxt.js docs](https://nuxtjs.org)
- [Vuetify.js docs](https://vuetifyjs.com)
