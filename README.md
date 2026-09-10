# Dokumentasi MMS ERP
### PT. Megarap Mitra Solusi — Sistem ERP Internal (help.mms.net.id)

Dokumentasi ini menjelaskan cara penggunaan **MMS ERP** secara *step-by-step*, mulai dari proses **Instalasi pelanggan baru** sampai **Penagihan (billing)**, yang melibatkan 4 pihak:

| Pihak | Peran Utama |
|---|---|
| 🏢 **Internal MMS (Pusat)** | Manajemen data karyawan, approval, monitoring, keuangan/finance |
| 🏬 **Cabang** | Eksekusi instalasi & layanan pelanggan di wilayah masing-masing (mis. Cabang Bandar Jaya) |
| 📡 **POP (Point of Presence)** | Titik distribusi jaringan (ODP) dan teknisi lapangan yang memasang & merawat koneksi |
| 🧑‍💼 **Kantor Pemasaran (Marketing)** | Mencari & mendaftarkan calon pelanggan baru, follow-up, dan komisi |

---

## Alur Besar Proses (Instalasi → Penagihan)

```
1. MARKETING (Kantor Pemasaran)
   └─ Input "Calon Customer" (data prospek + lokasi + paket)
        │
        ▼
2. PROSES INSTALASI
   └─ Calon Customer diproses → otomatis membuat "Tiket Instalasi"
        │
        ▼
3. CABANG / POP / TEKNISI
   └─ Tiket instalasi dikerjakan teknisi (Progress Tiket: Survey → Instal → Done/Pending/Failed)
        │
        ▼
4. KONTRAK BERLANGGANAN
   └─ Setelah instalasi selesai, dibuat dokumen kontrak berlangganan pelanggan
        │
        ▼
5. CUSTOMER AKTIF
   └─ Pelanggan masuk "Data Customer" dengan status Instalasi & Kontrak
        │
        ▼
6. PENAGIHAN (INVOICE)
   └─ Tagihan bulanan diterbitkan → dibayar pelanggan → tercatat di "Riwayat Invoice"
        │             │
        │             └─ Jika telat bayar → "Riwayat Blokir" (layanan disuspend)
        ▼
7. KOMISI MARKETING
   └─ Setiap invoice yang terbayar → menghasilkan komisi untuk marketing terkait
```

---

## Daftar Isi Dokumentasi

1. [Pengenalan Sistem & Login](01-Pengenalan-Sistem.md)
2. [Kantor Pemasaran (Marketing) — Calon Customer & Proses Instalasi](02-Kantor-Pemasaran-Marketing.md)
3. [Instalasi — Cabang & POP (Tiket, Progress, ODP)](03-Instalasi-Cabang-POP.md)
4. [Kontrak Berlangganan & Penagihan (Billing)](04-Kontrak-dan-Penagihan.md)
5. [Upgrade/Downgrade Paket & Insentif Marketing](05-Upgrade-Paket-dan-Insentif.md)
6. [Internal MMS — Karyawan, HRD, & Operasional Harian](06-Internal-MMS.md)

Semua tangkapan layar (screenshot) referensi disimpan di folder [`screenshots/`](screenshots/).

> **Catatan:** Dokumentasi ini disusun berdasarkan hasil eksplorasi langsung pada sistem MMS ERP (help.mms.net.id) menggunakan akun dengan level akses **Marketing**. Beberapa menu (misalnya Finance/Keuangan penuh, atau menu khusus Direktur/NOC) mungkin memiliki tampilan tambahan yang hanya terlihat oleh level akses tersebut.
