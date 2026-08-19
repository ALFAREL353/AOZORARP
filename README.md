
### 👥 Manajemen Grup

| Perintah | Fungsi |
| :--- | :--- |
| `/lp creategroup <nama>` | Membuat grup baru |
| `/lp deletegroup <nama>` | Menghapus grup |
| `/lp listgroups` | Melihat semua grup yang ada |
| `/lp group <grup> info` | Melihat info detail grup |

---

### 👤 Manajemen Pemain

| Perintah | Fungsi |
| :--- | :--- |
| `/lp user <pemain> parent add <grup>` | Masukkan pemain ke grup |
| `/lp user <pemain> parent remove <grup>` | Keluarkan pemain dari grup |
| `/lp user <pemain> parent set <grup>` | Set grup utama (hapus semua grup lain) |
| `/lp user <pemain> parent setprimarygroup <grup>` | Ganti grup utama (tanpa menghapus grup lain) |
| `/lp user <pemain> info` | Lihat semua grup & izin pemain |
| `/lp user <pemain> clear` | Hapus semua data pemain (grup & izin) |

---

### 🔑 Manajemen Izin (Permission)

| Perintah | Fungsi |
| :--- | :--- |
| `/lp group <grup> permission set <izin> true/false` | Beri/cabut izin ke grup |
| `/lp user <pemain> permission set <izin> true/false` | Beri/cabut izin ke pemain |
| `/lp group <grup> permission unset <izin>` | Hapus izin dari grup |
| `/lp user <pemain> permission unset <izin>` | Hapus izin dari pemain |
| `/lp group <grup> permission info <izin>` | Cek status izin di grup |
| `/lp user <pemain> permission info <izin>` | Cek status izin di pemain |

---

### 🏷️ Manajemen Prefix & Suffix

| Perintah | Fungsi |
| :--- | :--- |
| `/lp group <grup> meta addprefix <weight> "teks"` | Tambah prefix di depan nama |
| `/lp user <pemain> meta addprefix <weight> "teks"` | Tambah prefix ke pemain |
| `/lp group <grup> meta addsuffix <weight> "teks"` | Tambah suffix di belakang nama |
| `/lp user <pemain> meta addsuffix <weight> "teks"` | Tambah suffix ke pemain |
| `/lp group <grup> meta removeprefix <weight>` | Hapus prefix berdasarkan weight |
| `/lp user <pemain> meta removeprefix <weight>` | Hapus prefix pemain berdasarkan weight |
| `/lp group <grup> meta removesuffix <weight>` | Hapus suffix berdasarkan weight |
| `/lp user <pemain> meta removesuffix <weight>` | Hapus suffix pemain berdasarkan weight |
| `/lp group <grup> meta clear` | Hapus SEMUA meta (prefix & suffix) |
| `/lp user <pemain> meta clear` | Hapus SEMUA meta pemain |
| `/lp group <grup> meta info` | Lihat semua meta grup |
| `/lp user <pemain> meta info` | Lihat semua meta pemain |

---

### ⚖️ Manajemen Bobot (Weight)

| Perintah | Fungsi |
| :--- | :--- |
| `/lp group <grup> setweight <angka>` | Atur bobot grup (makin tinggi = prioritas) |
| `/lp group <grup> showweight` | Lihat bobot grup saat ini |

---

### 🧬 Warisan (Inheritance)

| Perintah | Fungsi |
| :--- | :--- |
| `/lp group <grup> parent add <grup_induk>` | Buat grup mewarisi grup lain |
| `/lp group <grup> parent remove <grup_induk>` | Hapus warisan |
| `/lp group <grup> parent set <grup_induk>` | Set warisan (ganti semua) |
| `/lp group <grup> parent info` | Lihat warisan grup |

---

### 🌍 Manajemen Global & Server-Specific

| Perintah | Fungsi |
| :--- | :--- |
| `/lp sync` | Sinkronkan semua perubahan |
| `/lp reload` | Reload konfigurasi LuckPerms |
| `/lp info` | Lihat info plugin |
| `/lp verbose on/off` | Mode debug untuk cek izin |
| `/lp tree` | Lihat tree izin |

---

### 🔧 Web Editor

| Perintah | Fungsi |
| :--- | :--- |
| `/lp editor` | Buka web editor di browser |
| `/lp sync` | Terapkan perubahan dari web editor |

---

### 📝 Contoh Penggunaan Cepat

```bash
# Buat grup
/lp creategroup builder

# Tambah prefix
/lp group builder meta addprefix 20 " &b[Builder] "

# Masukkan pemain ke grup
/lp user alfarel353 parent add builder

# Cek info pemain
/lp user alfarel353 info

# Hapus suffix
/lp group builder meta removesuffix 10

# Lihat semua meta
/lp group builder meta info

# Sinkronkan
/lp sync
```

---

### 🎨 Kode Warna & Efek

| Kode | Warna/Efek | Kode | Warna/Efek |
| :--- | :--- | :--- | :--- |
| `&0` | Hitam | `&a` | Hijau |
| `&1` | Biru Tua | `&b` | Aqua |
| `&2` | Hijau Tua | `&c` | Merah |
| `&3` | Cyan | `&d` | Pink |
| `&4` | Merah Tua | `&e` | Kuning |
| `&5` | Ungu | `&f` | Putih |
| `&6` | Emas | `&7` | Abu-abu |
| `&8` | Abu-abu Tua | `&9` | Biru |
| `&l` | **Tebal** | `&o` | *Miring* |
| `&n` | <u>Garis Bawah</u> | `&m` | ~~Coretan~~ |
| `&k` | Berkedip | `&r` | Reset |

---
