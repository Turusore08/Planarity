# Planarity
Disini saya akan merangkum pembelajaran teori graf pertemuan ke sebelas ini dengan Bahasa Bayi

## Pengertian Planarity
Planarity adalah kondisi dimana edge digambar dalam 2D tidak bertabrakan atau bertumpukan atau bahasanya itu saling memotong
 ***Bahasa Bayi-nya***
Kalian memiliki sebuah trek tamiya. Trek tamiya yang tidak saling bertabrakan adalah trek tamiya yang rapi. trek tamiya yang menyilang itu trek tamiya yang jelek 

**Contoh**:
  - `K4` (graf lengkap 4 simpul) adalah planar.
    
    `K4` misalnya kalian punya 4 kelereng dan kalian taruh di tanah. lalu kalian mencoba menggambar garis dengan catatan garisnya ga boleh berpotongan dan keempat kelereng tersebut saling terhubung
  - `K5` dan `K3,3` **non-planar**.
    
    `K5` kalian punya 5 kelereng dan kalian taruh di tanah. kalian ga bakal bisa menggambar garis yang menghubungkan ke 5 kelereng tersebut tanpa ga berpotongan.

    `K3` kalian punya 3 kelereng biru dan 3 kelereng merah. kalian harus menghubungkan setiap satu kelereng biru ke 3 kelereng merah lainnya. kalian ga bisa tanpa ga berpotongan.
    
**Rumus Euler** (untuk graf planar terhubung):

`V - E + F = 2`
(V = simpul, E = sisi, F = wilayah/wajah)

---

## 🌟 Complete Bipartite Graph (`K_{m,n}`)
- **Definisi**: Graf dengan:
1. Dua himpunan simpul terpisah (A dan B).
2. **Setiap** simpul di A terhubung ke **semua** simpul di B.
3. Tidak ada sisi di dalam A atau B.
- **Contoh**:
- `K3,3`: Non-planar (monster Kuratowski!).
- `K2,3`: Planar.
- 
***Bahasa bayi***

 `K_{2,3}` Kalian memiliki 2 guru dan 3 teman. setiap guru harus bisa menjabat 3 teman kalian
---

## ✨ Teorema Kuratowski
- **Statement**: 
> "Graf non-planar jika dan hanya jika mengandung subgraf homeomorfik ke `K5` atau `K3,3`."
- **Homeomorfik**:
- Boleh: Tambah/hapus simpul **derajat-2** di tengah sisi.
- Tidak boleh: Putus sisi atau tambah sisi baru.
- **Contoh**:
- Graf utilitas (`K3,3`) adalah non-planar.
- Graf Petersen mengandung subgraf homeomorfik ke `K3,3`.

---

## 🌀 Kurva Jordan (Jordan Curve)
- **Definisi**: Garis tertutup di bidang yang:
1. Tidak memotong diri sendiri.
2. Membagi bidang jadi **interior** dan **exterior**.
- **Teorema Kurva Jordan**:
> "Setiap Kurva Jordan membagi bidang menjadi 2 wilayah terhubung."
- **Contoh**:
- ✅ Lingkaran, segitiga.
- ❌ Angka "8", huruf "X".

---

## � Contoh Aplikasi
1. **PCB Design**: Hindari jalur listrik bersilangan (butuh graf planar).
2. **Network Routing**: Pastikan koneksi tidak overlap.

---

## 📚 Sumber Visual
- [K5 dan K3,3](https://en.wikipedia.org/wiki/Complete_graph)
- [Graf Petersen](https://en.wikipedia.org/wiki/Petersen_graph)

---
