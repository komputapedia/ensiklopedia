---
judul: Model View Update
tagar: ['arsitektur aplikasi', 'antarmuka'] # tagar untuk menandai entri ensiklopedia sejenis
kategori: ['Perangkat Lunak'] # pengategorian untuk sub bidang keilmuan tertentu.
sinonim: ['MVU', 'model view update','Arsitektur Elm'] # sisnonim dari judul untuk memudahkan pencarian
deskripsi: ""
---

Model-View-Update atau **MVU** adalah arsitektur aplikasi yang bersifat interaktif terhadap perubahan data. Model-View-Update juga dikenal dengan nama The Elm Architecture karena arsitektur ini menjadi komponen utama dari bahasa pemrograman Elm <cite>[\[1\]](#TEA)</cite>.

## Cara Kerja

Model-View-Update memiliki tugas tersendiri dari namanya:

![Kredit Gambar: Halaman Buku Panduan Resmi Bahasa Elm](https://guide.elm-lang.org/architecture/buttons.svg)

Sumber gambar: [Halaman Buku Panduan Resmi Bahasa Elm](https://guide.elm-lang.org/architecture/).

- **Model**, Data status (_state_) dari aplikasi.
- **View**, Fungsi menyajikan tampilan dari aplikasi, seperti HTML.
- **Update**, Fungsi untuk merubah Model dan View melalui pesan (_Msg_).

Pendekatan Model-View-Update berprinsip perulangan tertutup yang bergantung dengan data yang ada didalam *Model*. 

```elm
type Model = Int

init :: Model
init = 0
```

Setiap aplikasi dengan prinsip Model-View-Update memiliki fungsi **init** yang berisi nilai awal dari Model, jika ada perubahan Model maka fungsi **View** akan dipanggil ulang untuk membangun kembali tampilan (_re-rendering_).

```elm
type Msg =
    | Increment
    | Decrement

update :: Model -> Msg -> Model
update model msg =
    case msg of
        | Increment -> model + 1
        | Decrement -> model - 1
```

Perubahan **Model** dilakukan melalui fungsi **Update**, seperti *Increment* atau *Decrement* di tulis didalam fungsi ini. Fungsi **Update** akan dipanggil melalui fungsi **View** untuk memicu perubahan tampilan:

```elm
view :: Model -> Html(Model,Msg)
view model =
    div[][
        button [onClick Increment][ 
            text "+"
        ]
        , text [] [text (String.fromInt model)]
        , button [onClick Increment][
            text "+"
        ]
    ]
```

Sumber contoh kode : <a href="https://guide.elm-lang.org/architecture/buttons.html">Button - The Elm Architecture</a>.

## Pustaka Bahasa

Pendekatan Model-View-Update banyak diadopsi oleh berbagai bahasa pemrograman seperti Redux<cite>[\[3\]](#REDUXD)</cite>, Elmish F# <cite>[\[4\]](#ELMISH)</cite> dan BLoC dari Flutter <cite>[\[5\]](#BLOCFL)</cite>.

### Referensi

Daftar dibawah hanya sebagai contoh.

<ol>
    <li id="TEA">
        <a href="https://guide.elm-lang.org/architecture/">The Elm Architecture</a>
    </li>
    <li id="BUTTEA">
        <a href="https://guide.elm-lang.org/architecture/buttons.html">Button - The Elm Architecture</a>
    </li>
    <li id="REDUXD">
        <a href="https://redux.js.org/tutorials/fundamentals/part-2-concepts-data-flow">
            Redux Fundamentals, Part 2: Concepts and Data Flow
        </a>
    </li>
    <li id="ELMISH">
        <a href="https://zaid-ajaj.github.io/the-elmish-book/#/chapters/elm/the-architecture">
            Ajaj, Zaid. The Elmish Book - The Elm Architecture.
        </a>
    </li>
    <li id="BLOCFL">
        <a href="https://bloclibrary.dev/#/architecture">
            Architecture - BlocLibrary.dev
        </a>
    </li>

</ol>