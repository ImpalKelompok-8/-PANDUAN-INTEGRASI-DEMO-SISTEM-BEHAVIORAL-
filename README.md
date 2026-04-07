========================================================================
            PANDUAN INTEGRASI & DEMO SISTEM (BEHAVIORAL)
========================================================================

Mahasiswa wajib memastikan seluruh artefak perancangan TERINTEGRASI. 
Gunakan checklist di bawah ini sebagai standar kelulusan review.

------------------------------------------------------------------------
[1] SYNC: DFD LEVEL 1 -> CLASS DIAGRAM
------------------------------------------------------------------------
Setiap proses dalam DFD harus memiliki representasi logika di Class Diagram.
   [ ] Representasi Class: 1 Data Store di DFD = 1 Class Entity.
   [ ] Representasi Method: 1 Lingkaran Proses di DFD = 1 Method/Fungsi.
       Contoh: Proses "3.1 Update Stok" di DFD wajib muncul sebagai 
       fungsi 'updateStok()' di dalam Class Inventory.

------------------------------------------------------------------------
[2] SYNC: ERD -> LIVE DATABASE
------------------------------------------------------------------------
Database bukan sekadar tabel kosong, tapi harus bisa didemokan live.
   [ ] Struktur: Nama tabel & field wajib sama persis dengan ERD.
   [ ] Data Dummy: Isi minimal 10 record data logis per tabel.
   [ ] Query Ready: Siapkan file .sql berisi query (SELECT/INSERT/UPDATE)
       yang mewakili setiap proses bisnis utama.

------------------------------------------------------------------------
[3] SYNC: MOCKUP PROTOTYPE -> BEHAVIORAL FLOW
------------------------------------------------------------------------
Mockup harus membuktikan bahwa aliran data (Data Flow) berjalan.
   [ ] Clickable: Flow navigasi antar layar harus jalan.
   [ ] Input/Output: Tunjukkan di mana user menginput data (Process In)
       dan di mana sistem menampilkan data dari database (Process Out).
   [ ] Validation: Tunjukkan respon sistem jika input salah.

------------------------------------------------------------------------
[4] SKENARIO LIVE DEMO (MATRIKS TRACEABILITY)
------------------------------------------------------------------------
Saat demo, mahasiswa harus bisa menunjukkan hubungan berikut:
   "Saya klik tombol [SIMPAN] di MOCKUP (UI), aksi ini menjalankan 
    fungsi [saveData()] di CLASS DIAGRAM, yang kemudian mengeksekusi 
    query [INSERT INTO...] ke DATABASE."
========================================================================
