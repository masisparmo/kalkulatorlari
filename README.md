**Web Aplikasi Perencanaan Olah Raga Lari / Jalan (Kalkulator Lari)**
=================================================================

Aplikasi web interaktif yang dirancang untuk membantu pelari dan pejalan kaki merencanakan sesi latihan mereka dengan mudah dan efektif. Dilengkapi dengan dukungan AI dari "Coach AI" untuk memberikan tips latihan yang dipersonalisasi.

Aplikasi ini bisa langsung diakses di [https://kalkulatorlari.isparmo.com/](https://kalkulatorlari.isparmo.com/) 

**Deskripsi**
-------------

Aplikasi ini memungkinkan pengguna untuk membuat rencana latihan berdasarkan dua metrik utama: **pace** (laju) atau **durasi**. Dengan memasukkan target jarak, pengguna dapat menghitung estimasi durasi yang dibutuhkan jika berlatih dengan pace tertentu, atau sebaliknya, menghitung pace yang harus dicapai untuk menyelesaikan jarak dalam durasi yang ditargetkan.

Selain itu, aplikasi ini memberikan wawasan tambahan seperti kategori aktivitas (mulai dari jalan santai hingga sprint), estimasi total langkah kaki, dan yang paling utama, tips latihan yang relevan dari pelatih virtual berpengalaman, "Coach Gem", yang didukung oleh Google Gemini.

**Teknologi yang Digunakan**
----------------------------

Proyek ini dibangun menggunakan teknologi web front-end standar yang ringan dan modern:

*   **HTML5:** Untuk struktur dasar aplikasi web.
    
*   **Tailwind CSS:** Untuk styling yang cepat, responsif, dan modern langsung di dalam markup.
    
*   **JavaScript (ES6+):** Untuk semua logika kalkulasi, interaktivitas DOM, dan integrasi API.
    
*   **Google Fonts:** Menggunakan font "Inter" untuk tipografi yang bersih dan mudah dibaca.
    
*   **Google Gemini API:** Untuk fitur tips latihan yang didukung oleh kecerdasan buatan.
    

**Fitur**
---------

*   **Perencanaan Ganda:** Rencanakan latihan berdasarkan **Target Pace** atau **Target Durasi**.
    
*   **Kalkulasi Otomatis:**
    
*   Hitung estimasi **durasi total** dari jarak dan pace.
    
*   Hitung estimasi **pace per km** dari jarak dan durasi.
    
*   **Estimasi Langkah Kaki:** Dapatkan perkiraan jumlah langkah yang akan Anda tempuh selama sesi latihan.
    
*   **Kategori Aktivitas:** Secara otomatis mengklasifikasikan jenis latihan Anda (misalnya, Lari Tempo, Jalan Cepat) berdasarkan pace yang dihitung.
    
*   **Tips dari Pelatih AI "Coach Ai":** Dapatkan saran latihan yang dipersonalisasi dan memotivasi setelah membuat rencana. Fitur ini memerlukan Kunci API Google Gemini.
    
*   **Desain Responsif:** Tampilan yang optimal di berbagai perangkat, baik desktop maupun mobile.
    
*   **Antarmuka Intuitif:** Alur pengguna yang sederhana dengan tombol Hitung dan Reset yang jelas.
    

**Petunjuk Penggunaan (Setup)**
-------------------------------

Aplikasi ini sangat mudah digunakan karena tidak memerlukan proses build atau instalasi yang rumit.

1.  **Unduh File:** Cukup unduh file index.html dari repositori ini.
    
2.  **Buka di Browser:** Buka file index.html tersebut menggunakan browser web modern apa pun (seperti Google Chrome, Firefox, atau Safari). Atau bisa langsung jalankan dengan mengunjungi link: [https://kalkulatorlari.isparmo.com/](https://kalkulatorlari.isparmo.com/) 
    
3.  **Mulai Merencanakan:**
    

*   Masukkan **Rencana Jarak Tempuh** dalam kilometer.
    
*   Pilih mode perencanaan: **Pace** atau **Durasi**.
    
*   Isi input yang sesuai (menit/detik untuk pace, atau jam/menit/detik untuk durasi).
    
*   Klik tombol **"Hitung Rencana"**.
    

4. **Dapatkan Tips (Opsional):**

*   Setelah hasil perhitungan muncul, klik tombol **"Dapatkan Tips dari Coach Ai"**.
    
*   Sebuah jendela akan muncul meminta **Kunci API Gemini**.
    

**Cara mendapatkan Kunci API Gemini**

Untuk menggunakan fitur Dapatkan Tips dari Coach Ai, Anda memerlukan Kunci API Google Gemini. Anda bisa mendapatkannya secara gratis dengan mengikuti langkah-langkah berikut:

1.  Kunjungi [**Google AI Studio**](https://aistudio.google.com/app/apikey).
    
2.  Masuk dengan akun Google Anda.
    
3.  Klik **"Create API key"** untuk membuat kunci baru.
    
4.  Salin kunci yang telah dibuat dan tempelkan ke dalam jendela yang muncul di aplikasi.
    

Kunci API Anda akan disimpan di localStorage browser untuk kemudahan penggunaan di masa mendatang, sehingga Anda tidak perlu memasukkannya berulang kali

**Penjelasan Dukungan AI**
--------------------------

Ada dua dukungan AI (LLM) yang digunakan:

1.  Dukungan dari **IBM Granite** yang dirunning menggunakan API dalam bahasa Python di lingkungan IDE Google Colab, untuk membuat membuat dokumentasi dari web apps ini.
    
2.  Dukungan Google Gemini sebagai Coach Ai yang bisa memberikan tips atau arahan terkait dengan hasil perencanaan lari atau jalan kaki yang telah dihitung.
    

**Coach Ai** adalah seorang pelatih lari dan jalan kaki virtual yang berpenglaman puluhan tahun di dunia olah raga.

**Bagaimana Cara Kerjanya?**

1.  Setelah Anda menghitung rencana latihan, data seperti jarak, pace, durasi, dan kategori aktivitas dikirimkan ke Coach Ai.
    
2.  Coach Ai, yang telah diinstruksikan untuk bertindak sebagai pelatih berpengalaman, akan menganalisis data ini.
    
3.  Berdasarkan analisis tersebut, Coach Gem akan memberikan 3-5 tips praktis yang relevan dengan rencana spesifik Anda, mencakup aspek pemanasan, strategi saat beraktivitas, dan pemulihan.
