# InventoryMarketplace
# Sistem Inventory Marketplace & Executive Dashboard

Prototype aplikasi inventory berbasis **PHP native modular + MySQL + Bootstrap**.

## Fitur utama
- Login terpisah untuk **admin** dan **petugas**
- Dashboard admin untuk monitoring KPI dan stok minimum
- Dashboard petugas untuk aktivitas operasional harian
- Master data: admin, petugas, marketplace, rak, item
- Transaksi: item masuk dan item keluar
- Ajuan item dengan persetujuan admin
- Laporan ringkas item masuk, item keluar, dan stok
- Log aktivitas pengguna

## Struktur
- `index.php` : landing page
- `admin/` : area admin
- `petugas/` : area petugas
- `database/inventory_ksi.sql` : database siap import

## Cara menjalankan
1. Salin folder project ke `htdocs` atau web root Anda.
2. Buat database dan import file `database/inventory_ksi.sql`.
3. Sesuaikan koneksi pada file `koneksi.php`.
4. Buka project melalui browser.

## Akun demo
### Admin
- username: `admin`
- password: `admin123`

### Petugas
- username: `petugas`
- password: `petugas123`

## Catatan
Prototype ini mengikuti pola aplikasi referensi Anda:
- **native PHP modular** seperti inventory lama
- **tampilan lebih modern** seperti portal desa
- pemisahan hak akses admin vs petugas sesuai alur laporan


## Revisi struktur terbaru
- Marketplace dihapus dari master item dan item masuk.
- Marketplace hanya dipakai di item keluar untuk mencatat distribusi/update stok per channel.
- Laporan admin ditambah distribusi harian per produk dan rekomendasi pembagian rata stok per marketplace.
- Tombol PDF menggunakan fitur print browser agar bisa disimpan sebagai PDF di WAMP.
