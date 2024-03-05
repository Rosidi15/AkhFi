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

1.) NodeMCU(ESP8266) untuk nirkabel/lan atau NodeMCU(ESP32) untuk nirkabel/lan

2.) Koin Aseptor

3.) Mikrotik

4.) Akses Point

5.) PCB Kostum Node MCU (Opsional untuk nirkabel)

6.) Power Supply (12v untuk nodeMCU melalui step down, 24v lagi untuk Mikrotik)

7.) W5500 untuk berbasis Lan

8.) step down LM2596 atau DC ke DC apa pun yang dapat dikonversi ke 5v


---
> # **Arsitektur** 


![alt text](docs/JuanFi-Architecture.PNG?raw=true)

---

## ESP32 LAN Based Connection Diagram

![alt text](/docs/esp32-lan-diagram.jpg)

## ESP32 Wireless Based Connection Diagram

![alt text](/docs/esp32-wireless-diagram.jpg)

## ESP8622 Wireless Based Connection Diagram

![alt text](/docs/esp8622-wireles-diagram.jpg)

## ESP8622 LAN Based Connection Diagram

![alt text](/docs/esp8622-lan-diagram.jpg)


<br>

> # **Mem-flash perangkat keras**

# Cara flash ESP8622

Berikut petunjuk untuk mem-flash ESP8622 menggunakan custom pyflasher. Ikuti langkah-langkah berikut agar berhasil mem-flash modul ESP8622 dengan firmware yang diperlukan.

## Step 1: Download File Fleshing ESP8622

Unduh file flashing ESP8622 yang diperlukan untuk pengaturan Anda:

- [**File Berbasis Nirkabel ESP8622 **]([Berbasis Nirkabel.rar](https://github.com/Rosidi15/AkhFi/blob/main/ESP8622%20Berbasis%20Nirkabel.rar)) - Untuk pengaturan nirkabel.
- [**File Berbasis Lan ESP8622 **]([Berbasis Lan.rar](https://github.com/Rosidi15/AkhFi/blob/main/ESP8622%20Berbasis%20Lan.rar)) - Untuk pengaturan berbasis LAN.

## Step 2: Buka NodeMCU-PyFlasher

1. Hubungkan ESP8622 Anda ke PC Anda.
2. Buka NodeMCU-PyFlasher.exe aplikasi.

## Step 3: Mem-flash AkhFi-FlashFile1.bin

1. Di antarmuka PyFlasher:
   - Pilih file `AkhFi-FlashFile1.bin`.
   - Pastikan offset diatur ke `0x000000`.
   - Klik `Flash Nodemcu` tombol tersebut dan tunggu hingga proses flashing selesai.

![Flash File 1](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-FlashFile1.PNG?raw=true)

## Step 4: Mem-Flash AkhFi-FlashFile2.bin

1. In the PyFlasher interface:
   - Select the file `AkhFi-FlashFile2.bin`.
   - Set the offset to `0x200000`.
   - Click the `Flash Nodemcu` button and wait for the flashing process to complete.

![Flash File 2](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-FlashFile2.PNG?raw=true)

## Step 5: Menyelesaikan Proses Flashing

Setelah mem-flash kedua file, ESP8622 Anda sekarang siap. Mulai ulang NodeMCU untuk memulai pengaturan.

Selamat! Anda telah berhasil mem-flash perangkat ESP8622 dan siap untuk melanjutkan dengan Pengaturan AkhFi Setup.

</details>

<br>


# Petunjuk Flashing ESP32

Ikuti petunjuk ini untuk mem-flash perangkat keras ESP32 menggunakan esptool.exe. Proses ini akan memuat firmware yang diperlukan ke modul ESP32.

## Step 1: Download File Flesing ESP32

Unduh file flashing ESP32 yang diperlukan untuk pengaturan Anda:

- [**File Berbasis Nirkabel ESP32 **]([Berbasis Nirkabel.rar](https://github.com/Rosidi15/AkhFi/blob/main/ESP32%20Berbasis%20Nirkabel.rar)) - Untuk pengaturan nirkabel.
- [**File Berbasis Lan ESP32 **]([Berbasis Lan.rar](https://github.com/Rosidi15/AkhFi/blob/main/ESP32%20Berbasis%20Lan.rar)) - Untuk pengaturan berbasis LAN.

## Step 2: Jalankan Skrip Flashing

1. Klik Duakali `start_flash.bat`.
2. Hubungkan ESP32 Anda ke PC Menggunakan Kabel DAta USB.
![Connect ESP32](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-Lan-FlashFile1.PNG?raw=true)

3.Prompt perintah akan muncul, meminta Anda untuk memilih port COM yang tersedia untuk ESP32 Anda.
![Select COM Port](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-Lan-FlashFile2.PNG?raw=true)

## Step 3: Pilih Port Com

1. Pilih port COM yang sesuai untuk ESP32 Anda (misalnya, COM9).
2. Tekan "Enter."

![Select COM Port](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-Lan-FlashFile3.PNG?raw=true)

3. Pesan penghubung akan muncul, menunjukkan alat tersebut mencoba terhubung ke ESP32.
![Connecting](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-Lan-FlashFile4.PNG?raw=true)

## Step 4: Mulai Flash

1. Tekan dan tahan tombol flash pada ESP32 selama 3-5 detik.
2.Proses flashing akan dimulai.

![Initiate Flashing](https://github.com/ivanalayan15/JuanFi/blob/master/docs/JuanFi-Lan-FlashFile5.PNG?raw=true)

## Step 5: Tunggu Hingga Selesai

Tunggu hingga proses flashing selesai.

## Step 6: Selesai

Setelah proses flashing selesai, Anda dapat memutuskan sambungan ESP32 dari PC Anda. Perangkat sekarang siap untuk Pengaturan.

Selamat! Anda telah berhasil mem-flash perangkat ESP32 dan siap untuk melanjutkan dengan Pengaturan AkhFi SetUp.


</details>

<br>

> # Seting Portal

## 1. Hubungkan ke AkhFi Setup

### Untuk Yang Berbasis Nirkabel Esp32/Esp8622

1. Cari SSID "AkhFi Setup" di perangkat Anda.
2. Hubungkan ke SSID
3. Akses panel admin di browser Anda di http://172.217.28.1/login .

![Wireless Setup](/docs/JuanFi-Step01.PNG)

### Untuk Berbasis Lan Esp32/Esp8622

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

![Admin Panel Login](/docs/JuanFi-Step02.PNG)

## 8. Konfigurasi Sistem

Isi Vendo Name dengan Nama Portal Anda Contoh :"Portal Sabrina", Kemudian Scan Nama SSID Wifi Anda,pasword dikosongkan, Kemudian Mode Pilih DHCP (jika Berbasis Nirkabel) Pilih Statik (Jika Berbasis Lan), Kemudian isi Ip mikrotik Sesuai dengan Ip Mikrotik Anda begitu juga dengan username dan paswordnya.

> **Note:** Change the password of the **operator** account to prevent unauthorized access to the vendo.

![Configure System](/docs/JuanFi-Step03.PNG)

### Configure Promo Rates

![Configure Promo Rates](/docs/JuanFi-Step04.PNG)

> # Mikrotik Setup

## 1. Setup Mikrotik Hotspot

Set up the Mikrotik hotspot server according to your configuration. You can find tutorials online for setting up a hotspot server in Mikrotik.

## 2. Add this initial script in your terminal

Execute on mikrotik terminal

```bash
/system scheduler add interval=1d name="Reset Daily Income" on-event="/system script set source=\"0\" todayincome " policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=00:00:00;
/system scheduler add interval=30d name="Reset Monthly Income" on-event="/system script set source=\"0\" monthlyincome " policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=00:00:00;
```

```bash
/system script add dont-require-permissions=no name=todayincome owner=admin policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon source="0";
/system script add dont-require-permissions=no name= monthlyincome owner=admin policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon source="0";
```

```bash
/ip hotspot walled-garden ip add action=accept disabled=no dst-address-list=JuanfiVendo
/ip firewall filter add action=accept chain=input place-before=0 comment=JuanfiVendo src-address-list=JuanfiVendo
```

## 3. Make NodeMCU IP Address Static

Set the IP address of your vendo (NodeMCU) to static to prevent it from changing addresses.

![Static IP Address](/docs/JuanFI-Mikrotik-Step1.PNG)

Copy the mac-address and ip-address of your vendo
and set the address-list to JuanfiVendo

![Static IP Address](/docs/JuanFi-Mikrotik-Step1.2.PNG)

## 4. Add IP Bindings Exception on Hotspot

Ensure the vendo's MAC address and IP address are added to IP bindings exceptions to prevent unauthorized usage.

![IP Bindings Exception](/docs/JuanFi-Mikrotik-Step2.PNG)


## 5. Modify vendoIpAddress in config.js

Modify the `vendoIpAddress` in the [config.js](/mikrotik-template/assets/js/config.js) file to match your setup.

![Modify vendoIpAddress](/docs/JuanFi-Mikrotik-Step5.PNG)

## 6. Upload HTML Portal to Mikrotik

Upload the [HTML portal](/mikrotik-template/) to your Mikrotik files. You can find different portal designs in our [Facebook Group Community](https://www.facebook.com/groups/1172413279934139).

## 7. Create User for NodeMCU API Access

Create a user for NodeMCU API access. The default user for NodeMCU is **pisonet** with password **abc123**. You can change it as needed.

![NodeMCU API User](/docs/JuanFi-Mikrotik-Step3.PNG)

---

## **8.) Please add this script in the hotspot user profile on login event** (credits to kristoff for adding sales)

Execute on mikrotik terminal
Put on the on login script (with telegram support) please change accordingly with your hotspot folder(hex or haplite)

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

### enable JuanFi online monitoring 0 = DoNotSend,  1=send data to api
:local apiSend 0;
### derive from the JuanFi online monitoring, create account in genman.projectdorsu.com
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

![alt text](/docs/JuanFi-Mikrotik-Step4.PNG?raw=true)

> ## **Miscellaneous Scripts**

You can create a scheduler to restart (System - > Scheduler) add your desired schedule and put this script or modify the existing template scripts below in your desired settings

- **38vz2rb6nk** - this is the API KEY you generate in admin panel
- **10.10.10.251** - this is your ESP IP Address

Replace those value with your own setting

### **Restart vendo scheduler**

Sample Script that run at 3am:

```bash
  /system scheduler add interval=1d name="Restart Vendo" on-event="/tool fetch http-method=post http-header-field=\"X-TOKEN: 38vz2rb6nk\" url=\"http://10.10.10.251/admin/api/restartSystem\"" policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=03:00:00;
```

### **Night Light schedulers**

Sample Script that turn on nightlight at 6 pm:

```bash
 /system scheduler add interval=1d name="Turn ON Night Light" on-event="/tool fetch http-method=post http-header-field=\"X-TOKEN: 38vz2rb6nk\" url=\"http://10.10.10.251/admin/api/toggerNightLight\?toggle=1\"" policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=18:00:00;
```

### **Sample Script that turn off nightlight at 6 am:**

```bash
 /system scheduler add interval=1d name="Turn OFF Night Light" on-event="/tool fetch http-method=post http-header-field=\"X-TOKEN: 38vz2rb6nk\" url=\"http://10.10.10.251/admin/api/toggerNightLight\?toggle=0\"" policy=ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon start-date=Sep/28/2021 start-time=06:00:00;
```


# **Mikrotik Hotspot Portal**

![alt text](/docs/Mikrotik-hotspot.PNG?raw=true)

# **Admin Panel Dashboard**

![alt text](/docs/JuanFi-Step05.PNG?raw=true)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[Untuk Pembelian Lisensi Bisa Hubungi Kami](https://wa.link/8ksewt)
