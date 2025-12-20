# Decision Log – QA Automation

## Tujuan

Catatan ini menjelaskan **kenapa saya memilih test case tertentu untuk diotomasi**
dan kenapa ada beberapa yang tidak.

## Daftar Test Case

1. Login valid
2. Login invalid
3. Checkout flow
4. Animasi hover tombol
5. Sorting produk

## Keputusan

### 1. Login valid

**Keputusan:** diotomasi  
**Alasan:** ini pintu masuk sistem, critical flow, semua user melewati langkah ini

### 2. Login invalid

**Keputusan:** diotomasi  
**Alasan:** feedback ke user, rawan regression, harus selalu diuji

### 3. Checkout flow

**Keputusan:** diotomasi  
**Alasan:** bisnis utama, transaksi penting, user experience harus dijaga

### 4. Animasi hover tombol

**Keputusan:** tidak diotomasi  
**Alasan:** visual saja, mudah flaky, low value

### 5. Sorting produk

**Keputusan:** tidak diotomasi (sementara)  
**Alasan:** tidak critical, bisa manual dulu, baru otomatis jika sering bug
