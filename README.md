# Praktikum1 Pemrograman Mobile
Nama: Khansa Nur Khalisah
NIM: H1D023106
Shift: B/E

# Tugas 1- Pertemuan 2
# Dokumentasi
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/35df2a5a-c1cd-44f8-bcde-3475c00422d2" />

# Penjelasan
# Aplikasi Tugas 2 Pemrograman Mobile: 
Proyek ini merupakan hasil dari Pertemuan 2 mata kuliah Pemrograman Mobile. Aplikasi menampilkan halaman sederhana berisi gambar, teks sambutan, deskripsi, dan tombol untuk pindah ke halaman berikutnya.

# Fitur Utama:
a. Menampilkan gambar gedung teknik di bagian atas.
b. Menampilkan teks sambutan (welcome text) di tengah layar.
c. Menampilkan deskripsi singkat tentang Prodi Informatika.
d. Terdapat tombol "Next" untuk berpindah ke halaman berikutnya.

# Techstech yang Digunakan:
a. Android Studio
b. Kotlin
c. Material Design 3 (Material Components)
d. LinearLayout untuk layout utama

# Struktur Layout (activity_main.xml):
a. LinearLayout → Layout utama.
b. ImageView (img_gedung_teknik) → Menampilkan gambar gedung teknik.
c. TextView (tv_welcome) → Menampilkan teks sambutan.
d. TextView (tv_description) → Menampilkan deskripsi singkat.
e. MaterialButton (btn_to_page2) → Tombol untuk menuju halaman kedua.

# Tugas2 - Pertemuan 3

# 🎥 Demo Aplikasi
[⬇️ Download Demo Video](https://github.com/sasaaa1504/H1D023106_KhansaNurKhalisah_Pertemuan1_PraktikumPemob/raw/master/app/video/demo1.mp4)



# 📱 IF Unsoed Mobile

Aplikasi Android sederhana untuk menampilkan **profil lulusan Informatika Unsoed** serta menyediakan navigasi cepat ke beberapa kontak penting.

# ✨ Fitur Utama
- Halaman Utama (MainActivity) → tombol untuk menuju halaman profil lulusan.  
- Halaman Profil (Halaman2Activity) →  
  - Logo & gedung Unsoed  
  - CardView deskripsi profil lulusan  
  - Menu kontak (telepon, email, lokasi, Instagram)  
  - Tombol kembali  

# 🏗️ Struktur Proyek
- **Activity**
  - MainActivity.kt  
  - Halaman2Activity.kt  
- **Layout**
  - activity_main.xml  
  - activity_halaman2.xml  
  - layout_menu.xml  
- **Drawable**
  - ic_phone, ic_email, ic_location, ic_himpunan  
  - teknik_unsoed_2, lambang_unsoed  

# ⚙️ Implementasi
## View Binding
```kotlin
binding = ActivityHalaman2Binding.inflate(layoutInflater)
setContentView(binding.root)

# 📘 Tugas 4 - Pertemuan 4  

## 🎥 Demo Aplikasi  
[⬇️ Download Demo Video](https://github.com/sasaaa1504/H1D023106_KhansaNurKhalisah_Pertemuan1_PraktikumPemob/raw/master/app/video/demo 2.mp4)

---

## 📱 Book Search App (MVVM + Retrofit)  
Aplikasi Android sederhana yang menerapkan **arsitektur MVVM** dan **networking dengan Retrofit** untuk menampilkan daftar buku dari **OpenLibrary API**.  

---

## ✨ Fitur Utama  
- 🔎 **Koneksi ke API OpenLibrary** dengan Retrofit  
- 📚 **Pencarian buku** berdasarkan kata kunci  
- 📝 **Tampilan daftar buku** menggunakan RecyclerView  
- 📖 **Detail data buku**: Judul, Penulis, Tahun Terbit  
- 🔄 **Integrasi ViewModel & LiveData** (data otomatis ter-update)  
- 🛠️ **LogCat Debugging** untuk monitoring request & error  

---

## 📂 Struktur Proyek  

### 🔹 Activity / View  
- `DaftarBukuActivity.kt` → Activity utama untuk menampilkan daftar buku  
- `activity_daftar_buku.xml` → Layout utama dengan RecyclerView  
- `list_buku.xml` → Layout item untuk daftar buku  

### 🔹 ViewModel  
- `MainViewModel.kt` → Mengatur logika bisnis & komunikasi dengan API  

### 🔹 Model & Networking  
- `SearchResponse.kt` → Data class response dari API  
- `BookDoc.kt` → Data class detail buku  
- `OpenLibraryApi.kt` → Interface API Retrofit  
- `RetrofitInstance.kt` → Konfigurasi Retrofit  

### 🔹 Adapter  
- `BookAdapter.kt` → Adapter RecyclerView untuk menampilkan data buku  

### 🔹 Utils  
- `Constants.kt` → Menyimpan konstanta (BASE_URL API)  

---

## 🛠️ Teknologi yang Digunakan  
- **Kotlin**  
- **Retrofit2 + Gson Converter**  
- **ViewModel & LiveData (AndroidX Lifecycle)**  
- **RecyclerView**  
- **Kotlin Coroutines**  






