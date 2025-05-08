### 🛡️ **Deskripsi Singkat CTF - Gemastik (Keamanan Siber): Anya Haha Inakute Sabishii**

Tim: **Anya Haha Inakute Sabishii**
Anggota: **Fauzan Aldi**
Kategori yang dikerjakan: *Reverse Engineering*, *Forensics*

CTF ini berisi berbagai tantangan keamanan siber yang membutuhkan keterampilan *reverse engineering*, *file analysis*, hingga *network forensics*. Kami berhasil menyelesaikan beberapa soal penting dengan pendekatan teknikal dan scripting sebagai berikut:

---

#### 🔍 **Reverse Engineering – CodeJugling**

Membongkar program C, menganalisis logika pengecekan flag berbasis operasi XOR, dan menyusunnya ulang ke dalam Python untuk mendapatkan flag.

> **FLAG:** `Gemastik2022{st45iUn_MLG_k07a_b4rU}`

---

#### 🦖 **Reverse Engineering – Dino**

Menganalisis file `.jar` game dinosaurus dan file `highscore.txt`. Mengidentifikasi algoritma checksum, lalu membuat skor palsu yang valid dengan checksum-nya.

> **FLAG:** `Gemastik2022{why_would_you_ever_beat_me}`

---

#### 💎 **Reverse Engineering – Rubyte**

Membongkar metode enkripsi berbasis *binary to Gray code*. Mengimplementasikan dekripsi melalui script Python hingga berhasil mendapatkan isi file terenkripsi.

> **FLAG:** `Gemastik2022{i_still_remember_30_october}`

---

#### 🧾 **Forensik – Traffic Enjoyer**

Menganalisis file `.pcap`, mengekstrak potongan data berbentuk gambar PNG dalam base64 dari trafik HTTP, menyusunnya kembali untuk memperoleh flag.

> **FLAG:** `Gemastik2022{balapan_f1rst_bl00d_is_real_f580c176}`

---

#### 📁 **Forensik – Har**

Menganalisis file HAR (HTTP Archive) dari sesi browser. Mengambil file `.fig` dari URL di dalam trafik, membuka layer tersembunyi di Figma untuk menemukan flag.

> **FLAG:** `Gemastik2022{kinda_wish_this_werent_text}`

---

🧠 Kompetisi ini menuntut analisis menyeluruh terhadap sistem, manipulasi data rendah level, serta ketelitian dalam menyusun eksploitasi secara logis dan otomatis. Setiap tantangan berhasil diselesaikan dengan perpaduan deduksi teknis dan scripting Python.


Tentu! Berikut versi deskripsi write-up CTF **"No Rush n Relax"** dengan tambahan emoji agar tampil lebih menarik namun tetap bergaya teknis:

---

### 🧠 No Rush n Relax – Gemastik CTF Write-up

**🖋️ Author**: *Fauzan Aldi*

📄 Write-up ini mendokumentasikan proses penyelesaian challenge pada kompetisi **Gemastik CTF** dengan judul **"No Rush n Relax"**. Beragam tantangan dari kategori Reverse, Binary, Web, Forensik, hingga Misc berhasil dianalisis dan diselesaikan dengan pendekatan teknikal dan penuh ketelitian 🧩💻.

🔥 Beberapa highlight challenge:

* 🌀 **CodeJugling (Reverse – 500 pts)**
  Tantangan ELF 64-bit yang memanggil 35 subfungsi untuk membentuk flag. Dengan analisis IDA dan teknik reversing sederhana (XOR + literal), flag berhasil disusun 🧬.

* 🦖 **Dino (Reverse – 500 pts)**
  File `.jar` dengan validasi skor berbasis checksum. Setelah dekompilasi dan implementasi ulang algoritma CRC di C++, flag diperoleh dengan manipulasi highscore 🎮✅.

* 🧷 **Baby Heap (Binary – 992 pts)**
  Eksploitasi heap lewat bug UAF (Use After Free) di fungsi edit\_note. Dilakukan tcache poisoning untuk leak heap & libc, lalu overwrite GOT → shell access 💣🛠️.

* 🕵️‍♂️ **Traffic Enjoyer (Forensik – 500 pts)**
  File `.pcap` yang menyimpan data base64 dalam respons HTTP. Setelah decoding dan urutkan berdasarkan index, gambar-gambar kecil dirangkai hingga muncul flag 📡🖼️.

* 🗂️ **Har (Forensik – 500 pts)**
  File `.har` dari web Figma mengarah pada file `.fig`. Setelah dibuka di Figma dan menghapus objek putih, flag tersembunyi terlihat jelas 🎨🔍.

Setiap soal dilengkapi dengan snippet kode eksploit, script solver, dan penjelasan teknik secara rinci. Kompetisi ini mengajarkan banyak hal tentang detail teknikal dan kesabaran dalam mengurai satu per satu byte 🧘‍♂️🔧.
