# Panduan Kontribusi

Terima kasih sudah menyempat waktu membaca halaman ini. Ada hal yang perlu kamu patuhi dan ikut sebelum melakukan
kontribusi, hal ini diindahkan agar menciptakan ensiklopedia yang berkualitas dan menjaga proses gotong royong dalam
menyusun ensiklopedia.

## Apa yang bisa masuk Entri Ensiklopedia

Entri ensiklopedia adalah artikel terkait keilmuan komputasi, baik berupa definisi, teori, praktik dan sebagainya, tetapi tidak terbatas pada itu kamu juga bisa menambahkan:

- Definisi

Definisi menjelaskan istilah yang muncul dalam ilmu komputasi, seperti algoritme, program, basis data dan sebaginya.

- Teori

Teori terkait ilmu komputasi berserta kasus pemakaianya, seperti algoritme pengurutan, struktur data pohon , teknik penguraian, sistem distribusi dan semacamnya.

- Tokoh

Tokoh adalah orang yang memiliki kontribusi terhadap perkembangan dan perluasan wawasan ilmu komputasi. Tokoh tidak harus seorang akademisi, bisa siapa saja, influencer, konten kreator dan programmer yang punya kontribusi besar tapi memang tidak terlihat.

- Teknologi Komputasi

Teknologi komputasi adalah teknologi yang digunakan baik akademik ataupun oleh industri dalam keilmuan komputasi, seperti bahasa pemrograman, design pattern dan sebagainya.

- Fenomena

Bagian ini cukup kontroversial tetapi perlu, hal ini menrangkum fenomena terkait keilmuan dan penerapan ilmu komputasi, seperti rilis distro linux lokal dan sebagainya.

## Ketentuan Entri Ensiklopedia

Setiap kontributor wajib membaca ketentuan ini untuk

1. Entri ensiklopedia diharapkan memiliki referensi ke buku, halaman resmi, catatan dan sumber yang dapat dipercaya.
2. Entri diharapkan mengikuti kaidah tata bahasa indonesia yang berlaku serta tidak mengandung kalimat yang melanggar [Etika Kontributor](CODE_OF_CONDUCT.md).
3. Tidak diperkenankan menyalin atau menjiplak isi ensiklopedia dari sumber ensiklopedia lain, seperti Wikipedia.
4. Tidak harus membuat entri sempurna, bila merasa ada yang kurang lakuan pemerikasaan entri oleh sejawat dengan membuka _pull request_ dini sebelum selesai dan komunikasikan disana.
5. Semua kontribusi ini akan masuk kedalam lisensi Creative Common Atribusi atas nama Kontributor Komputapedia. 

## Menambahkan Entri Ensiklopedia

Kontribusi pada repositori ini dapat dilakukan dengan langkah berikut:

1. Lakukan _forking_ repositori ini di https://github.com/komputapedia/ensiklopedia.
2. Lalu buka hasil _fork_ repository, salin alamat repositori _fork_ kamu dan lakukan `git clone` di terminal / konsol komputer kamu.
    - Berikut ini perintahnya `git clone https://github.com/username github kamu/ensiklopedia`
      - Contoh bila menggunakan username saya (edelsora) maka, `git clone https://github.com/edelsora/ensiklopedia`.
3. Setelah proses `git clone` selesai, buka folder hasil proses tersebut di teks editor anda.
    1. Jika kamu ingin menambahkan sebuah entri ensiklopedia, maka
        - Buat folder dengan nama  judul entri
        - Salin berkas `TEMPLATE_ENSIKLOPEDIA.md` ke dalam folder, dan ubah namanya menjadi `index.md`.
        - Ubah isi `index.md` sesuai dengan keterangan yang ada didalamnya.
        - Setelah selesai mengisi entri, pastikan lakukan perintah ini :
            - `git add nama folder entri ensiklopedia/*`, ini untuk menambahkan isi ensiklopedia anda ke `stagging git` kamu.
                - contohnya: `git add algoritme/*`
            - `git commit -am "entri-baru(nama ensiklopedia): menamabkah entri ensiklopedia (nama ensiklopedia)`, ini untuk mencatat hasil perubahan terbaru yang akan di kirim ke GitHub.
                - contohnya: `git commit -am "entri-baru(algoritme): menamabkah entri ensiklopedia (algoritme)`
            - `git push`, untuk mengirimkan perubahan ke GitHub
        - Buka halaman repositori hasil _fork_ anda di GitHub dengan browser anda, lalu klik tulisan `Contribute` yang akan membuat _pull request_ baru ke repositori utama ensiklopedia.
        - Jangan lupa tambahkan reviewer ya, supaya hasil kontribusi kamu bisa cepat diperiksa dan masuk _mainline_ ensiklopedia.

    2. Jika kamu ingin memperbaiki sebuah entri ensiklopedia, maka
        - Buka folder yang memiliki nama sesuai dengan judul, lalu buka file `index.md`
        - Ubah isi `index.md` sesuai dengan perbaikan yang ada ingin ajukan.
        - Setelah selesai mengisi entri, pastikan lakukan perintah ini :
            - `git add nama folder entri ensiklopedia/*`, ini untuk menambahkan isi ensiklopedia anda ke `stagging git` kamu.
                - contohnya: `git add algoritme/*`
            - `git commit -am "perbaikan(nama ensiklopedia): jelaskan apa yang kamu perbaiki`, ini untuk mencatat hasil perubahan terbaru yang akan di kirim ke GitHub.
                - contohnya: `git commit -am "perbaikan(algoritme): memperbaharui referensi`
            - `git push`, untuk mengirimkan perubahan ke GitHub
        - Buka halaman repositori hasil _fork_ anda di GitHub dengan browser anda, lalu klik tulisan `Contribute` yang akan membuat _pull request_ baru ke repositori utama ensiklopedia.
        - Jangan lupa tambahkan reviewer ya, supaya hasil kontribusi kamu bisa cepat diperiksa dan masuk _mainline_ ensiklopedia.
4. Saatnya kamu menunggu umpan balik dari hasil periksa _pull request_ kamu oleh reviewer, mungkin akan ada beberapa komen yang bisa menjadi masukan baik.
5. Jika semua umpan balik sudah cukup dan mendapat penerimaan dari reviewer, maka hasil kontribusimu akan masuk ke _mainline_ repositori utama dan memungkinkan profil GitHub kamu masuk daftar kontribusi di halaman utama Komputapedia.

> Forking adalah penyalinan repositori secara menyeluruh ke akun kamu, jadi repositori ini akan ada
> di daftar repositori anda.