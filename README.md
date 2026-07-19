# Biodata Interaktif — Akmal Fahreza

Tugas Praktik 2: "Biodata Interaktif" — X PPLG SMT 2

Kartu biodata yang ditampilkan secara dinamis lewat JavaScript menggunakan **variabel** dan **innerHTML**. Satu file HTML mandiri (`biodata-interaktif.html`).

## Cara Menjalankan

1. Unduh file `biodata-interaktif.html`.
2. Buka langsung di browser (klik dua kali, atau seret ke jendela browser).
3. Klik tombol **"Tampilkan Biodata"** — data akan langsung muncul di dalam kartu.

## Fitur Sesuai Instruksi

| Instruksi | Implementasi |
|---|---|
| **Variabel** | Data biodata disimpan di 5 variabel: `nama`, `tempatLahir`, `alamat`, `hobi`, `citaCita` |
| **innerHTML** | Saat tombol diklik, `output.innerHTML` diisi dengan template string berisi baris-baris biodata |
| **Menampilkan biodata** | Data yang tampil: Nama, Tempat Lahir, Alamat, Hobi, dan Cita-cita |

## Kode Inti

```javascript
// 1. Variabel biodata
const nama = "Akmal Fahreza";
const tempatLahir = "Tangerang Selatan";
const alamat = "Pamulang, Tangerang Selatan";
const hobi = "Renang";
const citaCita = "Investment Banker";

btn.addEventListener('click', function () {
  // 2. Menyusun konten biodata dengan innerHTML
  output.innerHTML = `
    <div class="row"><span class="label">Nama</span><span class="value">${nama}</span></div>
    <div class="row"><span class="label">Tempat Lahir</span><span class="value">${tempatLahir}</span></div>
    <div class="row"><span class="label">Alamat</span><span class="value">${alamat}</span></div>
    <div class="row"><span class="label">Hobi</span><span class="value">${hobi}</span></div>
    <div class="row"><span class="label">Cita-cita</span><span class="value">${citaCita}</span></div>
  `;
});
```

## Cara Mengganti Data

Buka file dengan text editor, cari 5 baris `const` di bagian `<script>`, lalu ganti nilainya sesuai kebutuhan. Tidak perlu mengubah bagian lain.

## Catatan

Field **tanggal lahir** belum diisi secara spesifik karena datanya belum diberikan — tinggal tambahkan variabel baru (misalnya `tanggalLahir`) dan satu baris baru di dalam `innerHTML` jika ingin melengkapinya.
