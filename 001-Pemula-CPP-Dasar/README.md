# 1. Tingkat Pemula - C++ Dasar

**Tujuan**: Mempelajari sintaksis C++, tipe data, alur kontrol (control-flow) dan konsep pemrograman dasar.

## 1.1 Pengantar C++

### Apa itu C++?

C++ adalah bahasa pemrograman serbaguna yang dikembangkan sebagai perluasan dari bahasa pemrograman _C_.

Dikembangkan oleh _Bjarne Stroustrup_ di laboratorium _Bell_ pada awal 1980-an.

Bahasa yang dirancang untuk memberikan performa tinggi, fleksibilitas dan efisiensi, sangat cocok untuk aplikasi skala besar, dari pengembangan sistem/perangkat lunak hingga game, simulasi real-time dan lainnya.

**Fitur Utama C++**:

1. **Pemrograman Berorientasi Objek (Objek-Oriented Programming/OOP)**:

   - **Object-Oriented Programming (OOP)**:
     - C++ mendukung pemrograman berorientasi objek, yang memungkinkan developer untuk membaangun struktur kode berdasarkan _class_ dan _object_. Hal ini meningkatkan _reusabilitas_, _modularitas_, dan _skalabilitas_.
     - Konsep utama OOP dalam C++ meliputi:
       - **Classes** dan **Objects**: Class digunakan untuk mendefinisikan tipe data yang akan digunakan sebagai blueprint dari object yang akan dibuat. Object sebagai contoh dari kelas.
       - **Inheritance**: Memungkinkan _properties_ dan _methods_ diwariskan dari class lain, untuk meningkantkan reusabilitas kode.
       - **Encapsulation**: Memungkinkan penggunaan interface tunggal untuk merepresentasikan bermacam format data (tipe data).
       - **Abstraction**: Menyembunyikan kompleksitas dan detail, hanya menampilkan fitur penting saja dari sebuah object.

2. **Prosedural Programming**:

   - C++ mempertahankan pemrograman prosedural dari C, yang memungkinkan developer untuk membuat kode berdasarkan fungsi dan prosedur untuk mengoperasikan data.

3. **Pemrograman Generik**:

   - C++ mendukung template yang digunakan dalam pemrograman generik, yang difungsikan untuk meningkatkan _reusabilitas_ dan _keamanan_ kode.

4. **Manajemen Memori Tingkat Rendah**:

   - C++ memungkinkan akses langsung ke memori lewat pointers, sangat berguna untuk pemrograman sistem dan aplikasi dengan kinerjan tinggi.

5. **Standard Template Library (STL)**:

   - STL merupakan pustaka C++ yang mengoleksi _class_ dan _functions_, termasuk (seperti _vectors_, _list_, dan _maps_), algoritma (seperti _sorting_ dan _searching_), dan iterator.

6. **Performa**:

   - C++ dikenal sebagai bahasa pemrograman yang memiliki performan dan efisiensi yang tinggi.

7. **Portabilitas**:

   - C++ dapat di kompilasi dan dijalankan dibergagi platform (seperti _Windows_, _Linux_, _Mac_, dan _Raspberry Pi_), dengan sedikit penyesuaian compiler.

8. **Dukungan Pustaka yang Kaya**:
   - C++ memiliki pustaka yan kaya, seperti _STL_ yang dapat digunakan untuk berbagai keperluan, termasuk input/output, multithreading, networking, dan lainnya.

**Keunggulan C++**:

- _performa_: Performa dan efisiensi C++ memungkinkan untuk membangun aplikasi besar dengan kinerja tinggi.
- _kontrol_: Kemampuan manajeman memori tingkat rendah.
- _Versatilitas_: Dapat dikompilasi dan dijalankan diberbagai platform,
- _Dukungan Pustakan dan Komunitas_: Memiliki dukungan pustaka yang luas, serta komunitas besar karena C++ banyak diajarkan ditingkat universitas.

**Kekurangan C++**:

- _Kompleksitas_: C++ dapat dinilai lebih kompleks dan sulit untuk dipelajari, terutama untuk pemula.
- _Memori Manjeman Manual_: Perlu perhatian tinggi perihal manajeman memori, memungkinkan munculnya isu dan kebocoran memori.

### Perbedaan C, C++ dan Java!

1. **Sejarah dan Tujuan**:

   **C**:

   - Dikembangakn oleh _Denis Ritchie_ pada awal 1970-an.
   - Dirancang untuk pemrograman sistem dan pengembangan sistem operasi (seprti _UNIX_).
   - Fokus pada pemrograman prosedural dan manipulasi memori tingkat rendah.

   **C++**:

   - Dikembangkan oleh _Bjarne Stroustrup_ pada awal 1980-an sebagai perluasan dari bahasa _C_.
   - Menambahkan fitur pemrograman berorientasi objek (_OOP_) ke dalam C.
   - Dirancang untuk aplikasi yang membutuhkan kinerja tinggi dan kontrol resource.

   **Java**:

   - Dikembangkan oleh _James Gosling_ dan tim di _Sun Microsystems_ pada pertengahan 1990-an.
   - Dirancang untuk portabilitas dan keamanan, dengan moto "_Write Once, Run Anywhere_" (_WORA_).
   - Fokus pada pemrograman berorientasi objek dan pengembangan aplikasi web, mobile dan enterprise.

2. **Paradigman Pemrograman**:

   **C**:

   - _Pemrograman Prosedural_: Berfokus pada fungsi dan prosedur untuk memecahkan masalah menjadi langkah-langkah kecil.
   - Tidak mendukung pemrograman berorientasi objek.

   **C++**:

   - _Multi Paradigma_: Mendukung pemrograman prosedural, berorientasi objek dan generik.
   - Memiliki fitur OOP seperti _class_, _object_, _inheritance_, _polymorphism_ dan _encapsulation_.

   **Java**:

   - _Berorientasi Objek Murni_: Hampir semua elemen dalam Java adalah objek (Kecuali tipe data primitif).
   - Mendukung OOP dengan fitur seperti class, object, inheritance, polymorphism, dan encapsulation.
   - Juga mendukung pemrograman fungsional melalui fitur seperti lambda expression (di Java 8 dan seterusnya).

3. **Manajemen Memori**:

   **C**:

   - _Manual_: Developer perlu mengelola memori secara manual menggunakan fungsi `malloc()`, `calloc()`, dan `free()`.
   - Rentan terhadap kebocoran memori dan kesalahan akses memori.

   **C++**:

   - _Manual_ dan _Otomatis_: Mendukung manajemen memori manual menggunakan `new` dan `delete`, tetapi juga menyediakan fitur seperti RAII (Resource Acquisition Is Initialization) untuk manajemen memori otomatis.
   - Masih rentan terhadap kebocoran memori jika tidak dikelola dengan baik.

   **Java**:

   - _Otomatis_: Menggunakan _Garbage Collection_ untuk mengelola memori secara otomatis.
   - Developer tidak perlu mengalokasikan atau membebaskan memori secara manual, mengurangi risiko kebocoran memori.

4. **Portabilitas**:

   **C**:

   - _Portable dengan Batasan_: Kode C dapat dikompilasi dengan batasan untuk berbagai platform, dengan penyesuaian disetipa platform tertentu.
   - Tidak memiliki lingkungan runtime yang seragam.

   **C++**:

   - **Portable dengan Batasan**: Sama seperti C, C++ juga dapat dikompilasi dan dijalankan diberbagai platform dengan penyesuaian compiler.
   - Tidak memiliki lingkungan runtime yang seragam.

   **Java**:

   - **Sangat Portable**: Kode java dikompilasi ke _bytecode_ yang dapat dijalankan di _Java Virtual Machine_ (_JVM_) di platform apapun.
   - Prinsip "_Write Once, Run Anywhere_" (WORA) membuat Java sangat portable.
