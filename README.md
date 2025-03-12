# MyQR
## QR Code Scanner untuk Login Hotspot MikroTik

### Deskripsi
MyQR adalah solusi sederhana untuk memindai QR Code sebagai metode login di hotspot MikroTik. Dengan menambahkan tombol pada halaman login dan konfigurasi di MikroTik, pengguna dapat terhubung dengan lebih mudah.

### Cara Penggunaan

1. Tambahkan tombol di file `login.html` untuk mengarahkan ke halaman pemindaian QR Code:

```html
<button onclick="window.location='https://wahyusudrajad.github.io/myqr';">QR Code</button>
```

2. Tambahkan aturan berikut di MikroTik melalui Terminal agar halaman pemindaian QR Code dapat diakses tanpa login:

```sh
/ip hotspot walled-garden ip
add action=accept comment="Mikhmon QR Code Scanner" disabled=no dst-host=wahyusudrajad.github.io/wahyusudrajad
```

### Sumber Daya
Dibangun dengan teknologi dari [WebQR](https://wahyusudrajad.github.io/myqr).

---

🚀 Dibuat oleh [Wahyu Sudrajad](https://github.com/wahyusudrajad)