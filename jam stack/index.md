---
judul: JAM Stack
tagar: ['arsitektur perangkat lunak', 'web'] # tagar untuk menandai entri ensiklopedia sejenis
kategori: ['Perangkat Lunak','Teknologi Web'] # pengategorian untuk sub bidang keilmuan tertentu.
sinonim: ['JAM stack', 'JAM'] # sisnonim dari judul untuk memudahkan pencarian
---

JAM (Javascript, API, Markup) Stack  adalah arsitektur teknologi web yang dibangun dengan Bahasa Markup, Javascript sisi browser dan API yang berfokus pada pengolahan sisi klien.

Tujuan dari JAM Stack yaitu memisahkan _business logic_ dan _data layer_ untuk meningkatkan kinerja, skalabilitas, kemudahan perawatan dan fleksibilitas dalam rekayasa dari platfom Web<cite>[\[1\]](#JAMORG)</cite>.

Cara kerja utama dari JAM stack yaitu _pre-rendering_ dan _decoupling_. 

_Pre-rendering_ adalah pendekatan membuat semua asset dan halaman website dibentuk menjadi halaman statis saat proses publikasi.

_Decopuling_ adalah pemisahan komponen sistem dan layanan secara menyeluruh, _decoupling_ dalam JAM Stack bertujuan untuk memisahkan layanan dalam kerja web site, sehingga setiap komponen bisa di ubah secara mandiri dan mudah dirawat <cite>[\[2\]](#JAMRES)</cite>.


## Sejarah

Kemunculan JAM Stack dimulai pada tahun 2016 oleh Mathias Biilman, CEO sekaligus Founder Netlify <cite>[\[3\]](#BIINET)</cite>.

## Teknologi

Ada beragam pilihan pendekatan teknologi yang ada untuk menerapkan arsitektur, _Static Site Generation_ dan _Single Page Application_.

Alat yang umum digunakan untuk teknologi _Static Site Generation_ yang disebut dengan _generator_ yakni Jekyll, Hugo, Zola dan Next.

Alat yang umum digunakan untuk teknologi _Single Page Application_ dengan pendekatan _Client Side Rendering_ yakni React, Vue, Angular dan Svelte.

### Javascript

Web yang dibangun dengan JAM stack membutuhkan javascript untuk keperluan komponen Web di sisi klien seperti _fetching API_ dan sebagainya.

### API

API menjadi fungsi sederhana untuk melakukan beragam operasi yang dibungkus menjadi endpoin sederhana yang akan digunakan oleh website menggunakan javascript di browser klien, seperti AJAX. 

Tidak hanya untuk dikonsumsi oleh javascript, API juga bisa digunakan untuk manjemen konten sehingga 
ketika ada konten baru yang ditambahkan, alat _generator_ web akan mengambil data dari sini untuk menjadi konten web.

Pemanfaatan API seperti membuat newsletter, fitur komentar, _headless CMS_ dan sebagainya.

### Markup 

Markup bertugas sebagai kerangka tampilan utama dari web yang dihasilkan oleh alat _Static-site generator_ ataupun _framework javascript_ dengan pendekatan _Client side rendering_.

Markup akan berisi javascript untuk melakukan operasi dengan API maupun interaksi antar komponen markup. 

Contoh bahasa markup yakni _Hyper Text Markup Language_ (HTML).

### Referensi

Daftar dibawah hanya sebagai contoh.

<ol>
    <li id="JAMORG">
        Halaman resmi JAM Stack. <a href="https://jamstack.org">jamstack.org</a>
    </li>
    <li id="JAMRES">
        <a href="https://jamstack.org/glossary/decoupling/">Decoupling - Netlify Glossary </a>
    </li>
    <li id="BIINET">
        Mathias Biilman Netlify Blog. <a href="https://www.netlify.com/authors/matt-biilmann/">https://www.netlify.com/authors/matt-biilmann/</a>
    </li>
</ol>