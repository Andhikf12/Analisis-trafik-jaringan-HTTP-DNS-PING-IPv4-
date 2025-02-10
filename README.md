Nama  : Andhika Fajjriansyah<br>
NIM   :09030282327035<br>
Kelas : TK4B<br>

# Analisis trafik jaringan (HTTP DNS,PING) ((IPv4)<br>

**langkah langkah Percobaan**<br>
1.Pastikan Komputer/Laptop sudah terhubung ke internet.<br>

<img src="https://github.com/user-attachments/assets/9514779a-a62b-48be-a0e2-674947dea7bf" alt="image"
width="400"><br>

2.cek alamat IP Shopee dengan mengguanakan cmd dengan command "ping shopee.co.id"<br>

<img src="https://github.com/user-attachments/assets/6d3af90c-2592-4efd-899c-f5310e39c10c" alt="image"
width="400"><br>

3.Buka aplikasi Wireshark, lalu pilih interface yang terhubung ke internet.<br>

<img src="https://github.com/user-attachments/assets/3b00d1ee-7fcf-411c-be02-fa1faa1b88be" alt="image"
width="400"><br>

4.jalankan wireshark dan masukan ip shopee kedalam wireshark dengan cara ip.dst==202.181.90.156 
dan tunggu sekitar 10 menit berbarengan dengan anda membuka shopee sambil browsing<br>

<img src="https://github.com/user-attachments/assets/ff89131c-ae1c-49eb-99ab-11ac102e961f" alt="image"
width="400"><br>

5.setelam melakukan browsing,lanjut buka wireshark dan matikan pencarian nya  <br>

<img src="https://github.com/user-attachments/assets/af35720e-9043-43f0-b943-d23f033e77b3" alt="image"
width="400"><br>

6.Selajutnya lihat properties dari packet capture yang dilakukan. Dengan menekan 
Statistics > Caputre File Properties, atau dapat langsung menekan Ctrl+Alt+Shift+C 
keyboard secara bersamaan dan.<br>

<img src="https://github.com/user-attachments/assets/fac800dc-2553-42df-bb37-845f86640d01" alt="image"
width="400"><br>
7.Perhatikan bagian Statistics pada halaman Capture File Properties. Pada halaman ini 
kita dapat melakukan perhitungan Throughput, Packet Loss, Delay, dan Jitter. <br>

<img src="https://github.com/user-attachments/assets/7c0163aa-146a-4900-841b-8021352b64ba" alt="image"
width="400"><br>

8. Hitungan Throughput, Packet Loss, Delay, dan Jitter yang didapatkan dari 
Statistics Wireshark yang jalankan di Komputer/Laptop masing-masing <br>
 
  -throughput: <br>
  bytes	:Time span =hasil bytes<br>
  32998227: 734.435 = 44,93008503135063 x 8 : 359,440680250805<br>

  -packet loss : <br>
  [((paket di kirim -paket diterima) : paket terkirim) x 100]<br>
	=( 60180-60.174):60180)x100)<br>
	=(6 : 60180)x100<br>
	=0.009<br>
 
untuk mengitung nilai delay kita harus mencarinya menggunakan exsel,maka dari pada itu kita harus mendownload filenya dengan cara mendownload file csv. 

<img src="https://github.com/user-attachments/assets/37d479dd-f649-496b-b8e8-2eb9b3bf1a8f" alt="image"
width="400"><br>

untuk mencari nilai delaynya yaitu dengan cara 

<img src="https://github.com/user-attachments/assets/cde4dbeb-edfd-4d14-8d56-72d98354c40a" alt="image"
width="400"><br>

delay :<br>
time 2-time 1 = hasil delay<br>

total delay = sum (blok semua hasil delay lalu enter)<br>
            = 734,434708<br>
rata rata delay= (total ddelay / jumlah paket )<br>
	       = 0,012203967 s x 1000 = 12,203967 ms<br>
        
<img src="https://github.com/user-attachments/assets/cd1ddf29-9876-4794-a2f8-9eaea63fcd72" alt="image"
width="400"><br>

jitter = SUM (blok semua  jitter lalu enter )<br>
       = -0,074246 <br>           
rata rata jiter = (total jitter / jumlah paket lalu enter)<br>
		= 1,23373E-06 x 1000=0.00123373 ms<br>
