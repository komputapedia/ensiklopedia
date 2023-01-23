---
judul: SAFE Stack
tagar: ['Paradigma fungsional', 'Arsitektur web', 'MVU'] # tagar untuk menandai entri ensiklopedia sejenis
kategori: ['Perangkat Lunak', 'Teknologi Web'] # pengategorian untuk sub bidang keilmuan tertentu.
sinonim: ['SAFE-Stack'] # sisnonim dari judul untuk memudahkan pencarian
deskripsi: "Padanan teknologi web full-stack berbasis F# yang menawarkan kehandalan, produktivitas dan flesibilitas"

tanggal_pembuatan: "2022-12-10"
tanggal_pembaharuan: "2023-01-23"
---

<img alt="Logo dari SAFE Stack" src="https://safe-stack.github.io/images/illustrations/safe-stack.png" width="200" height="200" />

SAFE stack merupakan padanan teknologi (_techstack_) web berbasis bahasa F# yang menawarkan kehandalan, 
produktif dan fleksibilitas. SAFE sendiri merupakan gabungan dari 4 pustaka teknologi <cite>[\[1\]](#SAFEST)</cite>:

- S, Saturn kerangka kerja web bagian belakang 
- A, Azure platform hosting.
- F, Fable Transpilator F# ke Javascript.
- E, Elmish kerangka kerja web bagian depan berbasis MVU (Model-view-update) 

### Arsitektur Teknologi

Arsitektur ini bersifat _full-stack_ yang berarti keseluruhan aplikasi baik antarmuka ataupun lojik aplikasi di dikte menggunakan satu pendekatan teknologi: Bahasa F#.

Elmish sebagai bagian antarmuka aplikasi akan berhubungan dengan Saturn sebagai lojik aplikasi menggunakan _Fable.Remoting_ dengan protokol _Remote Procedure Call_ (RPC) untuk transfer data antar _client-server_ <cite>[\[2\]](#SAFEOV)</cite>.

SAFE Stack juga memiliki dukungan pendekatan _Server-side Rendering_.

### Referensi


<ol>
    <li id="SAFEST">
        Halaman Resmi SAFE-Stack, <a href="https://safe-stack.github.io">https://safe-stack.github.io</a>.
    </li>
    <li id="SAFEOV">
        SAFE-Stack Overview, SAFE Stack <a href="https://safe-stack.github.io/docs/overview/">https://safe-stack.github.io/docs/overview/</a>.
    </li>
</ol>