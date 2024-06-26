# **Wifi Koin AkhFi**

Wifi Koin AkhFi adalah sistem sumber terbuka inovatif yang dirancang untuk integrasi koin tanpa batas dengan Hotspot MikroTik. Ini memberikan solusi komprehensif untuk mengelola dan memonetisasi akses internet melalui integrasi mekanisme coinlot. Dengan Wifi Koin AkhFi, pemilik hotspot atau RT/RW NET dapat dengan mudah memasukkan sistem koin ke dalam infrastruktur jaringan mereka, memungkinkan mereka menawarkan akses internet berbayar dengan cara yang efisien dan ramah pengguna.




## **Donasi**

Kami sangat menghargai donasi karena membantu mendukung pengembangan dan pemeliharaan Wifi Koin AkhFi. Jika Anda ingin berkontribusi dan menunjukkan dukungan Anda, Anda dapat memberikan donasi dengan cara berikut: ``

- Akun Gcash/Dana : Ahyar Rosiidi - 085934241038


# **Kelompok Komunitas**

Bergabunglah dengan grup komunitas kami yang dinamis untuk terhubung dengan pengguna dan kontributor lain. Bagikan pengalaman Anda, bertukar ide, portal hotspot, dan ikuti perkembangan terkini dan peningkatan Wifi Koin AkhFi.

- Facebook Group: [Wifi Koin AkhFi Community](https://www.facebook.com/groups/943413657180146/)

# **Fitur**

 ### Opsi perangkat Keras

- Berbasis nirkabel
- Berbasis Lan

### Sistem Wifi Koin AkhFi

- Berbasis Mikrotik
- Print Kode Vocer Otomatis
- Koneksi KOde Otomatis
- Layar LCD
- Pembuatan kode di Portal menggunakan LCD, Printer TTL
- Sistem Multi Penjual

### Sistem Admin

- Pengaturan Awal Sistem
- Setting Koneksi Mikrotik, Setting SSID, Setting KoinSlot
- Konfigurasi Daftar Harga (Tarif, masa berlaku)
- Dasbor, Laporan Penjualan
- Konfigurasi Pin Khusus Untuk Login Admin
- konfigurasi sistem Penyalahgunaan KoinSlot

## Bahan-Bahan Yang Dibutuhkan

1.) NodeMCU(ESP32) untuk nirkabel/lan

2.) Koin Aceptor.

3.) Mikrotik

4.) Akses Point.

5.) PCB Kostum Node MCU (Opsional untuk nirkabel)

6.) Power Supply (12v untuk nodeMCU melalui step down, 24v lagi untuk Mikrotik)

7.) W5500 untuk berbasis Lan

8.) step down LM2596 atau DC ke DC apa pun yang dapat dikonversi ke 5v


---
> # **Arsitektur** 


![alt text](https://github.com/Rosidi15/AkhFi/blob/main/Arsitektur%20Wifi%20Koin%20Akhfi.jpg)

---

## Diagram ESP32 Berbasis LAN

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/DIAGRAM%20ESP32%20LAN.jpg)

## Diagram ESP32 Berbasis Wireless

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/DIAGRAM%20ESP32%20WERLES.jpg)


<br>

> # **Mem-flash perangkat keras**

# Petunjuk Flashing ESP32

Ikuti petunjuk ini untuk mem-flash perangkat keras ESP32 menggunakan esptool.exe. Proses ini akan memuat firmware yang diperlukan ke modul ESP32.

## Step 1: Download File Flesing ESP32

Unduh file flashing ESP32 yang diperlukan untuk pengaturan Anda:

- [**File Berbasis Nirkabel ESP32 **]([Berbasis Nirkabel.rar](https://github.com/Rosidi15/AkhFi/blob/main/ESP32%20Berbasis%20Nirkabel.rar)) - Untuk pengaturan nirkabel.
- [**File Berbasis Lan ESP32 **]([Berbasis Lan.rar](https://github.com/Rosidi15/AkhFi/blob/main/ESP32%20Berbasis%20Lan.rar)) - Untuk pengaturan berbasis LAN.

## Step 2: Jalankan Skrip Flashing

1. Hubungkan ESP32 Anda ke PC Menggunakan Kabel DAta USB.
2. Klik Duakali `start_flash.bat`.
![Connect ESP32](https://github.com/Rosidi15/AkhFi/blob/CARA-FLASH/Flash-ESP32-Langkah-1.jpg)

## Step 3: Pilih Port Com

1. Pilih port COM yang sesuai untuk ESP32 Anda (misalnya, COM7).
2. Tekan "Enteeer."

![Select COM Port](https://github.com/Rosidi15/AkhFi/blob/CARA-FLASH/Flash-ESP32-Langkah-2.jpg)


## Step 4: Tunggu Hingga Selesai

Tunggu hingga proses flashing selesai.

## Step 5: Selesai

![Selesai](https://github.com/Rosidi15/AkhFi/blob/CARA-FLASH/Flash-ESP32-Langkah-3.jpg)

Tekan Tombol apa saja untuk keluar dari CMD
Setelah proses flashing selesai, Anda dapat memutuskan sambungan ESP32 dari PC Anda. Perangkat sekarang siap untuk Pengaturan.

Selamat! Anda telah berhasil mem-flash perangkat ESP32 dan siap untuk melanjutkan dengan Pengaturan AkhFi SetUp.


</details>

<br>

> # Seting Portal

## 1. Hubungkan ke AkhFi Setup

### Untuk Yang Berbasis Nirkabel Esp32

1. Cari SSID "AkhFi Setup" di perangkat Anda.
2. Hubungkan ke SSID
3. Akses panel admin di browser Anda di http://172.217.28.1/login .

![Wireless Setup](https://github.com/Rosidi15/AkhFi/blob/main/Akhfi-SetUp.jpg)

### Untuk Berbasis Lan Esp32

1. Hubungkan Portal Anda ke port ethernet PC/Laptop Anda.
2. Tetapkan alamat IP PC/Laptop Anda sebagai statis ke 172.217.28.10 :
   - IP address: 172.217.28.10
   - Subnet Mask: 255.255.255.0
   - Gateway: 172.217.28.10
   - DNS: 172.217.28.10
3.Akses panel admin di browser Anda di http://172.217.28.1/login .

## 2. Masuk Ke Panel Admin

Gunakan username&pasword Bawaan dibawah ini:

- Username: admin
- Password: admin

![Admin Panel Login](https://github.com/Rosidi15/AkhFi/blob/main/Masuk%20ke%20Panel%20Admin.jpg)

## 3. Konfigurasi Sistem

Isi Vendo Name dengan Nama Pedagang Anda Contoh :"Ahmad Abdallah", Kemudian Scan Nama SSID Wifi Anda,pasword dikosongkan.
![Configure System](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Vendo-1.jpg)

Kemudian isi Ip mikrotik Sesuai dengan Ip Mikrotik Anda begitu juga dengan username dan paswordnya.
![Configure System](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Vendo-2.jpg)
![Configure System](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Vendo-3.jpg)
![Configure System](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Vendo-4.jpg)
![Configure System](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Vendo-5.jpg)

Jika Semuanya Sudah Sesuai kemudian pilih simpan. maka NodemCusudah terhubung dengan mikrotik,, lanjutkan ke pengaturan berikutnya.

### Konfigurasi Daftar Harga
(NB: Langkah ini di Lewatkan Dulu karena Langkah ini tidak akan bisa di lanjutkan sebelum Pengaturan Mikrotik)


![Configure Promo Harga](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Harga.jpg)
![Configure Promo Harga](https://github.com/Rosidi15/AkhFi/blob/main/Pengaturan%20Harga.2.jpg)

> # Pengaturan Mikrotik

## 1. SetUp Mikrotik Hotspot

Konfigurasikan server hotspot Mikrotik sesuai konfigurasi Anda. Mikrotik anda harus sudah di seting terlebih dahulu.

## 2. Tambahkan skrip awal ini di terminal Anda

Jalankan di terminal mikrotik

```bash
/system scheduler add interval=1d name="Reset Daily Income" on-event="/system script set source=\"0\" todayincome " policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=00:00:00;
/system scheduler add interval=30d name="Reset Monthly Income" on-event="/system script set source=\"0\" monthlyincome " policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=00:00:00;
```

```bash
/system script add dont-require-permissions=no name=todayincome owner=admin policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon source="0";
/system script add dont-require-permissions=no name= monthlyincome owner=admin policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon source="0";
```

```bash
/ip hotspot walled-garden ip add action=accept disabled=no dst-address-list=AkhfiPortal
/ip firewall filter add action=accept chain=input place-before=0 comment=AkhfiVendo src-address-list=AkhfiPortal
```

## 3. Jadikan Alamat IP NodeMCU Statis

Atur alamat IP vendo Anda (NodeMCU) menjadi statis untuk mencegahnya mengubah alamat.

![Static IP Address](https://github.com/Rosidi15/AkhFi/blob/main/AkhFI-Mikrotik-Step1.PNG)

Salin alamat mac dan alamat ip vendo Anda
dan atur daftar alamat ke AkhFiVendo

![Static IP Address](https://github.com/Rosidi15/AkhFi/blob/main/AkhFi-Mikrotik-Step1.2.jpg)

## 4.Tambahkan Pengecualian Pengikatan IP di Hotspot

Pastikan alamat MAC dan alamat IP vendo ditambahkan ke pengecualian pengikatan IP untuk mencegah penggunaan yang tidak sah.

![IP Bindings Exception](https://github.com/Rosidi15/AkhFi/blob/main/AkhFi-Mikrotik-Step2.PNG)


## 5.Unggah Portal HTML ke Mikrotik

Upload the [HTML portal](https://github.com/Rosidi15/AkhFi/blob/main/login%20page%20wifi%20koin%20akhfi.rar) to your Mikrotik files. You can find different portal designs in our [Facebook Group Community](https://www.facebook.com/groups/943413657180146).

## 6. Buat Pengguna untuk Akses API NodeMCU

Buat pengguna untuk akses API NodeMCU. Pengguna default untuk NodeMCU adalah **WifiKoin** dengan kata sandi **abc123**. Anda dapat mengubahnya sesuai kebutuhan.

![NodeMCU API User](https://github.com/Rosidi15/AkhFi/blob/main/AkhFi-Mikrotik-Step3.jpg)

---

## **7.) Silakan tambahkan skrip ini di profil pengguna hotspot pada acara login** (kredit kepada kristoff untuk menambahkan penjualan)

Jalankan di terminal mikrotik
Pasang skrip login (dengan dukungan telegram) silakan ubah sesuai dengan folder hotspot Anda (hex atau haplite)

```bash
### enable telegram notification, change from 0 to 1 if you want to enable telegram
:local isTelegram 0;
###replace telegram token
:local iTBotToken "xxxxxxxxxx:xxxxxxxxxxxxx-xxxxxxxxxxxxxxx-xxxxx";
###replace telegram chat id / group id
:local iTGrChatID "xxxxxxxxxxxxxx";
### hotspot folder for HEX put flash/hotspot for haplite put hotspot only
:local HSFilePath "hotspot";
### enable Random MAC synchronizer
:local isRandomMacSyncFix 0;

### enable AkhFi online monitoring 0 = DoNotSend,  1=send data to api
:local apiSend 0;
### derive from the AkhFi online monitoring, create account in genman.projectdorsu.com
:local URLvendoID 5;

# Get User Data
:local aUsrNote [/ip hotspot user get $user comment];
:local aUsrNote [:toarray $aUsrNote];
:local iUsrTime [:totime ($aUsrNote->0)];
:local iSaleAmt [:tonum ($aUsrNote->1)];
:local iExtCode ($aUsrNote->2);
:local iVdoName ($aUsrNote->3);
:local iTimeMin [/ip hotspot user get $user limit-uptime];
:local iUserReg [/system scheduler find name=$user];

# Check User Data
:if (($iTimeMin>0) and ($iUsrTime>=0) and (($iUserReg="") or ($iExtCode=1))) do={
  /ip hotspot user set $user comment="";
  :local iFileMac;
  :local mac $"mac-address";
  :for i from=0 to=([:len $mac] - 1) do={
    :local chr [:pick $mac $i]
    :if ($chr = ":") do={ :set $chr "" }
    :set iFileMac ($iFileMac . $chr)
  }
# api tracking
  { /do {
  :local URLamount "$amt";
  :local URLcomment "ScriptOnLoginFINAL";
  :local URLip [:put [:tostr $address]];
  :local URLusr [$user];
  :local URLmac [$"mac-address"];
  :local URLipmac "$URLusr_$URLip_$URLmac";
  :local URLactive [/ip hotspot active print count-only];
  :if ($apiSend!=0)  do={
  /do {
  :local fixUrl [("https://juanfiapi.projectdorsu.com/serve.js\?s=stats&i=OE-IBX-12345&m=direct&payload=$URLvendoID")];
  :local apiUrl "$fixUrl_$URLamount_$URLipmac_$URLactive_$URLcomment";
  :log debug "API SendInfo: $apiUrl ";
  /tool fetch mode=https http-method=get url=$apiUrl keep-result=no
  :delay 1s;
  } on-error={:log error "API Vendo ERROR: $apiUrl ";} }
  } on-error={:log error "APIvendoRoutineError";} }
# Extend User
  :if (($iUserReg!="") and ($iExtCode=1)) do={
    :local iTimeInt [/system scheduler get $user interval];
    :set iTimeInt ($iTimeInt+$iUsrTime);
    :if ($iTimeMin>$iTimeInt) do={ :set iTimeInt ($iTimeMin+$iUsrTime) };
    /system scheduler set $user interval=$iTimeInt;
  }
# ADD User
  :local iDateBeg [/system clock get date];
  :local iTimeBeg [/system clock get time];
  :if ($iUserReg="") do={
    :local iTimeInt $iUsrTime;
    :if ($iTimeMin>$iUsrTime) do={ :set iTimeInt ($iTimeMin+$iUsrTime) };
    :do { /system scheduler add name="$user" interval=$iTimeInt \
      start-date=$iDateBeg start-time=$iTimeBeg disable=no \
      policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon \
      on-event=("/ip hotspot user remove [find name=$user];\r\n".\
                "/ip hotspot active remove [find user=$user];\r\n".\
                "/ip hotspot cookie remove [find user=$user];\r\n".\
                "/system scheduler remove [find name=$user];\r\n".\
                ":do {/file remove \"$HSFilePath/data/$iFileMac.txt\"} on-error={};\r\n")
    } on-error={ log error "( $user ) /system scheduler add => ERROR ADD!" };
    :local x 10;:while (($x>0) and ([/system scheduler find name="$user"]="")) do={:set x ($x-1);:delay 1s};
  };
# Save Data File
  :if ([/file find name="$HSFilePath/data"]="") do={
    :do {/tool fetch dst-path=("$HSFilePath/data/.") url="https://127.0.0.1/"} on-error={ };
  }
  :local iValidUntil [/system scheduler get $user next-run];
  :if ([/system scheduler find name=$user]!="") do={
    /file print file="$HSFilePath/data/$iFileMac.txt" where name="dummyfile";
    :local x 10;:while (($x>0) and ([/file find name="$HSFilePath/data/$iFileMac.txt"]="")) do={:set x ($x-1);:delay 1s};
    /file set "$HSFilePath/data/$iFileMac" contents="$user#$iValidUntil";
  }
# Update Today Income
  :local iSaveAmt [:tonum [/system script get todayincome source]];
  :local iDailySales ($iSaleAmt + $iSaveAmt);
  /system script set todayincome source="$iDailySales";
# Update Monthly Income
  :local iSaveAmt [:tonum [/system script get monthlyincome source]];
  :local iMonthSales ( $iSaleAmt + $iSaveAmt );
  /system script set monthlyincome source="$iMonthSales";
# Telegram
  :if ($isTelegram=1) do={
    :local xVendo;
    :for i from=0 to=([:len $iVdoName] - 1) do={
      :local chr [:pick $iVdoName $i]
      :if ($chr = " ") do={ :set $chr "%20" }
      :set xVendo ($xVendo . $chr)
    }
    :local iUActive [/ip hotspot active print count-only];
    :local iMessage ("<<======New Sales======>>%0A".\
                     "Vendo: $xVendo %0A".\
                     "Voucher: $user %0A".\
                     "IP: $address %0A".\
                     "MAC: $mac %0A".\
                     "Amount: $iSaleAmt %0A".\
                     "Extended: $iExtCode %0A".\
                     "Total Time: $iTimeMin %0A %0A".\
                     "Today Sales: $iDailySales %0A".\
                     "Monthly Sales: $iMonthSales %0A".\
                     "Active Users: $iUActive %0A".\
                     "Valid Until: $iValidUntil %0A".\
                     "<<=====================>>");
    /tool fetch url="https://api.telegram.org/bot$iTBotToken/sendmessage\?chat_id=$iTGrChatID&text=$iMessage" keep-result=no;
  }
};
# Random Mac
:if ($isRandomMacSyncFix=1) do={
  :local cmac $"mac-address";
  :foreach AU in=[/ip hotspot active find user="$user"] do={
    :local amac [/ip hotspot active get $AU mac-address];
    :if ($cmac!=$amac) do={  /ip hotspot active remove [/ip hotspot active find mac-address="$amac"]; }
  }
}


```

Put on the on logout script

```bash
:if ($cause="session timeout") do={
  /system scheduler set [find name=$user] interval=5s;
}
```

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/Secrip%20login.png)


# **Mikrotik Hotspot Portal**
sebelum Pembelian Lisensi

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/Tampilan%20Panel%20Admin.jpg)

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/Pembelian%20Lisensi.jpg)

Setelah Pembelian Lisensi

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/Pembelian%20Lisensi-1.jpg)

![alt text](https://github.com/Rosidi15/AkhFi/blob/main/Tampilan%20Admin%20setelah%20di%20seting.jpg)


## License

[Untuk Pembelian Lisensi Bisa Hubungi Kami](https://wa.link/8ksewt)
