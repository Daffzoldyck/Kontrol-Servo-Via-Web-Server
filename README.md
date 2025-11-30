# Kontrol Servo via Web Server

Proyek ini memungkinkan Anda untuk mengontrol posisi sebuah servo motor melalui halaman web yang di-host oleh ESP32 itu sendiri. Tidak memerlukan platform pihak ketiga.

## Kebutuhan Hardware

-   ESP32
-   Servo Motor (misalnya SG90)
-   Breadboard dan Kabel Jumper

## Koneksi

-   **Servo Motor:**
    -   Kabel **Merah (VCC)** -> **5V** (atau VIN) ESP32
    -   Kabel **Coklat/Hitam (GND)** -> GND ESP32
    -   Kabel **Oranye/Kuning (Signal)** -> **GPIO 13** ESP32

## Cara Penggunaan

1.  **Setup Software:**
    -   Install library `Servo` dari Arduino IDE Library Manager (jika belum ada).

2.  **Upload Kode:**
    -   Buka file `web_servo_control.ino`.
    -   Ganti `YOUR_WIFI_SSID` dan `YOUR_WIFI_PASSWORD`.
    -   Upload kode ke ESP32.

3.  **Jalankan:**
    -   Buka **Serial Monitor** pada Arduino IDE (set baud rate ke 115200).
    -   ESP32 akan terhubung ke WiFi dan menampilkan alamat **IP-nya**.
    -   Buka browser di komputer atau ponsel yang terhubung ke jaringan WiFi yang sama.
    -   Ketik alamat IP yang muncul di Serial Monitor ke address bar browser.
    -   Anda akan melihat halaman web dengan slider. Geser slider untuk menggerakkan servo.
