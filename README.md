# Persiapan-Pertemuan-5

## Apa itu MultiThreading?
MultiThreading adalah kemampuan suatu program atau sistem operasi untuk mendukung lebih dari satu pengguna pada satu waktu tanpa memerlukan beberapa salinan program yang berjalan di komputer.
MultiThreading juga dapat menangani beberapa permintaan dari pengguna yang sama.

## Perbedaan Thread dan Runnable
### 1. Thread
- Thread adalah sebuah kelas di java yang mewarisi langsung dari object.
- Untuk menjalankan thread menggunakan Thread, kita perlu membuat subclass dari Thread dan meng-override metode run().

### 2. Runnable
- Runnable adalah interface, bukan kelas.
- Thread class behavior yang sudah tidak terpakai tidak akan dapat untuk digunakan lagi.
- Untuk menggunakannya, kita harus membuat kelas yang mengimplementasikan Runnable dan mengimplementasikan metode run().

### Kesimpulan
- Jika kita tidak perlu mewarisi kelas lain dan ingin membuat thread langsung gunakan Thread.
- Jika kita ingin memisahkan logika bisnis dari kontrol thread atau perlu mewarisi kelas lain gunakan Runnable.

## Penggunaan `Thread.sleep()`
`Thread.sleep()` metode ini digunakan untuk menghentikan sementara eksekusi thread yang sedang dieksekusi selama sejumlah milidetik atau nanodetik tertentu.
