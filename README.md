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


# Tugas 3 - Pertemuan 4  

# 🎥 Demo Aplikasi  
[⬇️ Download Demo Video](https://github.com/sasaaa1504/H1D023106_KhansaNurKhalisah_Pertemuan1_PraktikumPemob/raw/master/app/video/demo2.mp4)

---

# Book Search App (MVVM + Retrofit)  
Aplikasi Android sederhana untuk menampilkan **daftar buku dari OpenLibrary API** dengan menerapkan **arsitektur MVVM** dan **networking Retrofit**.  

---

# Fitur Utama  
- Halaman Utama (DaftarBukuActivity) → menampilkan daftar hasil pencarian buku  
  - RecyclerView untuk daftar buku  
  - Adapter untuk menghubungkan data ke tampilan  
- Pencarian data buku melalui **API OpenLibrary**  
- Menampilkan detail informasi buku:  
  - Judul  
  - Penulis  
  - Tahun terbit  
- Integrasi **ViewModel + LiveData** untuk update data otomatis  
- Debugging menggunakan **LogCat**  

---

# Struktur Proyek  

# Activity / View  
- `DaftarBukuActivity.kt`  
- `activity_daftar_buku.xml`  
- `list_buku.xml`  

# ViewModel  
- `MainViewModel.kt`  

# Model & Networking  
- `SearchResponse.kt`  
- `BookDoc.kt`  
- `OpenLibraryApi.kt`  
- `RetrofitInstance.kt`  

# Adapter  
- `BookAdapter.kt`  

# Utils  
- `Constants.kt`  

---

# 🛠️ Teknologi yang Digunakan  
- Kotlin  
- Retrofit2 + Gson Converter  
- ViewModel & LiveData (AndroidX Lifecycle)  
- RecyclerView  
- Coroutines  

# Tugas 4 - Pertemuan 5

##  Demo Aplikasi  
[⬇️ Download Demo Video](https://github.com/sasaaa1504/H1D023106_KhansaNurKhalisah_Pertemuan1_PraktikumPemob/raw/master/app/video/demo3.mp4)

---

## Book Detail Fragment App  
Aplikasi Android yang memanfaatkan **Fragment**, khususnya **BottomSheetDialogFragment**, untuk menampilkan detail buku secara dinamis. Proyek ini merupakan kelanjutan dari praktikum sebelumnya (Pertemuan 1–4), dengan fokus pada penggunaan **komponen UI modular** dan **navigasi antara Activity dan Fragment**.  

---

## Fitur Utama  
-  **Menambahkan atribut `coverId`** pada `BookDoc` untuk menampilkan cover buku.  
-  **Custom Drawable & Style** untuk mempercantik tampilan bottom sheet.  
- **Fragment Rinci Buku** dengan `BottomSheetDialogFragment`:
  a. Menampilkan judul, penulis, tahun terbit, dan cover buku.  
  b. Tampilan dialog muncul dari bawah layar (bottom sheet).  
- **Library Glide** digunakan untuk memuat gambar cover dari URL OpenLibrary.  
- **Penerapan konsep OOP** seperti encapsulation, inheritance, dan polymorphism di Fragment.  
- **Navigasi dari RecyclerView → Fragment Detail Buku** saat item diklik.  
- **Integrasi hasil pertemuan 1–4** menjadi satu alur aplikasi lengkap.

---

##  Struktur Proyek  

### Data & Model  
- `BookDoc.kt` → data class dengan atribut `coverId` tambahan.  

### Utils & Drawable  
- `bg_rounded.xml` → custom drawable dengan rounded corner dan border.  
- `styles.xml` → custom style untuk tampilan bottom sheet.  

### Fragment  
- `BookDetailFragment.kt`  
  - Menggunakan `BottomSheetDialogFragment`.  
  - Inisialisasi binding & override `getTheme()`.  
  - Method `loadData()` untuk memuat data buku ke UI.  
  - Lifecycle methods: `onCreateView`, `onViewCreated`, `onDestroyView`.  
- `fragment_book_detail.xml`  
  - Layout detail buku, berisi TextView dan ImageView.  

## Adapter & Event Handling  
- `BookAdapter.kt`  
  - Interface `OnBookClickListener` untuk klik item.  
  - Delegasi event klik ke Activity.  

## Activity  
- `DaftarBukuActivity.kt`  
  - Implementasi `OnBookClickListener`.  
  - Navigasi ke `BookDetailFragment` saat item daftar diklik.  

---

## Teknologi yang Digunakan  
- **Kotlin**  
- **Fragment & BottomSheetDialogFragment**  
- **Glide (Image Loading)**  
- **RecyclerView Adapter + Interface**  
- **View Binding**  
- **OOP (Encapsulation, Inheritance, Polymorphism)**  

---

## Alur Navigasi  
1. Pengguna melihat daftar buku di `DaftarBukuActivity`.  
2. Pengguna klik salah satu item buku.  
3. Adapter memanggil `onBookClick(book)` dan mengirim data ke Activity.  
4. Activity membuka `BookDetailFragment` dengan data buku tersebut.  
5. Fragment menampilkan detail buku dalam bentuk bottom sheet dialog.  

---

## Referensi  
- [Android Developers – Fragments](https://developer.android.com/guide/fragments)  
- [Android Developers – DialogFragment](https://developer.android.com/reference/androidx/fragment/app/DialogFragment)  
- [Android Developers – BottomSheetDialogFragment](https://developer.android.com/reference/com/google/android/material/bottomsheet/BottomSheetDialogFragment)  
- [Android Developers – PreferenceFragmentCompat](https://developer.android.com/reference/androidx/preference/PreferenceFragmentCompat)  
- [Android Developers – ListFragment](https://developer.android.com/reference/android/app/ListFragment)  

---

