# Smart Parking System with Firebase and Blynk Monitoring

## Deskripsi Proyek
Proyek ini bertujuan untuk membuat sistem parkir pintar yang dapat mendeteksi ketersediaan tempat parkir menggunakan sensor ultrasonik. Data real-time akan dikirim ke Firebase untuk keperluan analisis dan disajikan dalam aplikasi Blynk untuk pengguna.

## Komponen di Wokwi
- **NodeMCU ESP8266 atau ESP32** (untuk Wi-Fi dan komunikasi data)
- **Sensor Ultrasonik HC-SR04** (untuk mendeteksi kendaraan pada tempat parkir)
- **LED RGB** (indikator status tempat parkir: hijau untuk kosong, merah untuk terisi)
- **LCD I2C 16x2** (menampilkan jumlah tempat parkir yang tersedia)
- **Push Button** (untuk simulasi masuk/keluar kendaraan)
- **Buzzer** (untuk notifikasi saat kendaraan masuk/keluar)
- **Resistor** (untuk LED dan button)

## Fitur Utama
- **Firebase Integration**: Data jumlah tempat parkir yang tersedia disimpan dan di-update ke Firebase.
- **Blynk Integration**: Tampilan kondisi parkiran (penuh/kosong) dan jumlah slot di aplikasi Blynk.
- **Indikator Visual**: LED RGB menunjukkan status tempat parkir secara langsung.
- **Notifikasi Audio**: Buzzer berbunyi jika ada kendaraan yang masuk atau keluar.
- **User Interface**: Informasi jumlah tempat parkir tersedia ditampilkan pada LCD.

## Alur Kerja
1. **Pendeteksian Kendaraan**: 
   - Sensor Ultrasonik mendeteksi apakah ada kendaraan di tempat parkir dan mengirimkan data status ke Firebase.
   
2. **Update Data ke Firebase**:
   - Data ketersediaan tempat parkir (kosong/terisi) diperbarui di Firebase secara real-time.

3. **Tampilan di Aplikasi Blynk**:
   - Status parkir dan jumlah tempat parkir yang tersedia dapat dilihat oleh pengguna di aplikasi Blynk.

4. **Indikator Visual**:
   - LED RGB menyala hijau jika tempat parkir kosong, merah jika terisi.
   
5. **Notifikasi Suara**:
   - Buzzer memberikan notifikasi ketika kendaraan memasuki atau keluar dari tempat parkir.

6. **Display LCD**:
   - LCD menampilkan jumlah tempat parkir yang tersedia secara real-time.

