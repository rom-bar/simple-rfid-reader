# simple-rfid-reader
MFRC522 rfid reader from https://playground.arduino.cc/Learning/MFRC522


MFRC522 bisa dibeli murah dengan harga dibawah 50k saja.
sehingga cocok untuk percobaan simple.

kode disini adalah untuk reader data (dump) dari rfid keychain/card yang di dapatkan
dari paket MFRC522 . biasanya satu paket MFRC522 berisi 1 reader, 1 card dan 1 keychain

kode sudah di modifikasi agar bisa dipakai di NodeMCU v1.
dengan konfigurasi pin sebagai berikut:

MFRC522 --> NodeMCU

RST/Reset   --> D1

SPI SS/SDA  --> D2

SPI MOSI    --> D7

SPI MISO    --> D6

SPI SCK     --> D5

nb: pin SS/SDA dan RST biasanya pada tutorial lain menggunakan pin yang berbeda, karena memang configurable bisa dicoba untuk di ganti ke pin lain. jika di ganti ke pin lain, pada kode SS_PIN dan RST_PIN harus di update juga.

langkah-langkah:
- buka arduino IDE
- install library MFRC522(menu sketch-include library-manage libraries-search MFRC522)
- buka file .ino pada repo ini atau open folder atau copy paste isi file simple-rfid-reader.ino
- upload
- buka serial monitor dan set pada '9600'
- test dan lihat log pada serial monitor
