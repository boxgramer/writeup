# Pertanyaan Reflektif untuk Web Hacking

## Sebelum Melakukan Hacking
- Apa asumsi yang saya buat tentang sistem ini?
- Sudahkah saya membaca dan memahami dokumentasi yang relevan?
- Apa tujuan akhir dari eksploitasi ini?
- Apakah ada teknologi atau framework tertentu yang bisa menjadi titik lemah?
- Apakah sistem ini memiliki interaksi API eksternal?
- Apakah ini sistem berbasis file, form, atau API?
- Adakah pola unik dalam request/response yang bisa dimanfaatkan?
- Jika saya jadi developer sistem ini, bagian mana yang kemungkinan saya anggap "cukup aman padahal tidak"?
- Apa yang *tidak* di-filter oleh sistem ini?
- Apakah sistem ini memercayai input user lebih dari seharusnya?

> "Jangan serang seperti hacker. Pikirkan seperti developer yang lelah dan deadline-nya mepet."

## Setelah 30 Menit Stuck
- Apa hal paling sederhana yang belum saya coba?
- Apakah saya sudah memahami alur aplikasi dari awal sampai akhir?
- Apakah ada logika yang terlihat "normal" padahal bisa dimanipulasi?
- Adakah fitur yang tidak terlihat tapi aktif di background?
- Apakah saya hanya fokus pada 1 endpoint saja?

> "Kadang, solusi paling ampuh tersembunyi dalam kesederhanaan."

## Setelah 1 Jam Stuck
- Apakah saya sudah mencoba semua entry point?
- Adakah teknik lain yang biasa saya abaikan?
- Apa yang terjadi jika saya input sesuatu yang tidak masuk akal?
- Sudahkah saya memeriksa semua header yang dikirim dan diterima?
- Apakah respon server berubah tergantung parameter tertentu?
- Adakah perbedaan respon waktu antara input valid dan aneh?
- Sudahkah saya eksplorasi behavior dari JavaScript di sisi klien?
- Sudahkah saya coba semua metode HTTP (PUT, DELETE, dll)?

> "Dalam satu jam kamu bisa gagal banyak kali. Tapi satu ide gila bisa jadi kunci."

## Setelah 2 Jam Stuck
- Apa pola request-response yang terlihat mencurigakan?
- Apakah saya terlalu terpaku pada satu teknik eksploitasi?
- Apakah saya bisa mengubah peran user (guest, user, admin)?
- Adakah interaksi antar parameter yang belum saya eksplorasi?
- Sudahkah saya coba analisis parameter yang dikirim lewat JavaScript?

> "Setiap jam bertambah, setiap detail semakin penting."

## Setelah 3 Jam Stuck
- Sudahkah saya menulis semua hal yang telah dicoba?
- Adakah anomali dalam struktur URL atau URI?
- Adakah dependency eksternal yang mungkin bocor?
- Sudahkah saya uji file upload dengan semua kombinasi aneh?
- Apakah sistem ini memberi error message yang informatif jika dibuat gagal?

> "Tiga jam tanpa hasil bukan kegagalan, itu proses validasi."

## Setelah 4 Jam Stuck
- Apakah saya telah mereplikasi seluruh flow aplikasi dan mencari celah dari tiap langkah?
- Apakah ada bagian dari aplikasi yang hanya aktif di waktu tertentu atau via event tertentu?
- Adakah interaksi dengan storage (cookies, localStorage, session)?
- Apakah rate limit atau caching bisa dimanipulasi?

> "Jangan hanya eksploitasi apa yang terlihat. Gali apa yang disembunyikan."

## Setelah 5 Jam Stuck
- Apakah saya bisa menggunakan wordlist atau bruteforce untuk endpoint tersembunyi?
- Apakah ada file statis (sitemap, robots.txt, backup file) yang bisa dimanfaatkan?
- Adakah teknik lama yang relevan dengan sistem ini?
- Apakah saya harus mencoba sudut pandang attacker non-tradisional (exfil, chaining, SSRF)?

> "Setiap jam membawa sudut pandang baru. Semakin lama bertahan, semakin dalam pemahaman."

## Setelah 6 Jam Stuck
- Apakah saya melewatkan sesuatu karena terlalu fokus?
- Apakah teknik chaining bisa diterapkan (kombinasi bug kecil menjadi besar)?
- Apakah saya bisa mengotomatisasi uji coba saya dengan skrip?
- Apakah perlu jeda sejenak untuk memunculkan perspektif baru?

> "Kamu sudah bertahan 6 jam. Sekarang bukan soal menyerah, tapi naik level."

## Setelah 1 Hari Stuck
- Sudahkah saya mencatat semua eksperimen sebelumnya?
- Apa yang bisa saya pelajari dari traffic normal situs ini?
- Apa yang belum saya injeksi?
- Sudahkah saya cek response error dengan hati-hati?
- Adakah pola hidden endpoint di site map?
- Jika ini adalah CTF, exploit seperti apa yang biasanya dipakai?
- Apakah saya hanya menggunakan satu alat saja?
- Adakah teknik chaining yang bisa saya coba?

> "Gagal seharian itu wajar. Tapi gagal tanpa data itu rugi."

## Setelah 1 Minggu Stuck
- Apakah saya sudah lihat lab serupa dan belajar struktur eksploitnya?
- Apa kemungkinan besar developer salah konfigurasi?
- Apa kata orang lain tentang framework atau library ini di forum security?
- Adakah sistem fallback, dev mode, atau legacy API yang saya abaikan?
- Apakah saya terlalu terpaku pada satu celah?
- Bagaimana saya bisa membuat server 'berbicara lebih jujur'?
- Apakah saya bisa membuat eksploitasi tidak langsung (exfiltrasi via mail, dns, img, dll)?

> "Kalau jalur depan ditutup, masuk lewat jendela. Kalau jendela dikunci, bongkar genteng."

## Setelah 1 Bulan Stuck
- Apakah saya perlu menunda dan pelajari teknik baru dulu?
- Adakah tools lain yang lebih detail (Ffuf, wfuzz, nuclei, dirsearch)?
- Apakah saya memerlukan proxy custom atau plugin tambahan?
- Apakah pendekatan saya terlalu mirip dengan tutorial?
- Bisakah saya kolaborasi dengan orang lain atau mentor?
- Apakah ada teknik dari tahun-tahun lalu yang tidak umum tapi relevan?

> "Satu bulan stuck = satu bulan memupuk mental hacker."

## Setelah 3 Bulan Stuck
- Apa insight terbesar dari semua catatan eksplorasi saya?
- Adakah shortcut keyboard atau logika UI yang bisa dipaksa?
- Apakah saya mencoba menyerang dari sisi user yang berbeda (admin, guest)?
- Apakah saya bisa memanipulasi waktu, sequence, atau state?
- Adakah race condition yang bisa dicoba?
- Sudahkah saya periksa semua kode JS yang disisipkan dari CDN atau sumber luar?

> "Jika kamu bertahan 3 bulan, kamu sudah bukan sekadar peserta. Kamu sedang bertumbuh."

## Setelah 6 Bulan Stuck
- Apakah saya memahami arsitektur sistem ini secara menyeluruh?
- Apa kemungkinan blind vector yang belum terlihat efeknya?
- Adakah interaksi antar fitur yang bisa dieksploitasi?
- Apakah saya perlu membuat script otomatis untuk eksperimen massal?
- Apakah saya perlu belajar lebih dalam soal OS, SSRF, atau sandboxing?

> "Setengah tahun tidak sia-sia, jika kamu terus mencatat dan bereksperimen."

## Setelah 1 Tahun Stuck
- Apakah bug ini memang belum ada yang bisa tembus selama ini?
- Bisakah saya menulis artikel atau tool dari eksperimen yang gagal?
- Apakah ada celah di supply chain, dependency, atau CI/CD?
- Apakah bug ini hanya bisa diketahui via pentest blackbox atau dengan sumber log lain?
- Apakah saya harus ganti pendekatan total dari yang selama ini saya coba?

> "Satu tahun pencarian tidak gagal. Mungkin kamu sedang menuju bug jutaan rupiah."

## Setelah 2 Tahun Stuck
- Apakah saya satu-satunya orang yang peduli dengan bug ini?
- Apakah sudah saatnya saya publikasikan log dan insightnya untuk komunitas?
- Apakah ada pendekatan AI atau fuzzer generatif yang bisa bantu?
- Apakah bug ini memang bukan celah, tapi fitur yang belum dipahami?
- Apa yang sudah saya pelajari yang bisa membentuk saya jadi hacker lebih hebat?

> "Ketika dunia lupa, hacker sejati tetap menggali."

