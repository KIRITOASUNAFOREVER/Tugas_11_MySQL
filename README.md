# Tugas_11_MySQL

### 1. Buatlah user baru dengan nama Niomic dengan password c0b4d1b4c4!
```mysql
CREATE USER 'Niomic'@'localhost' IDENTIFIED BY 'c0b4d1b4c4';
```

![Nomor1](Nomor1.PNG)

### 2. Ubah password menjadi indonesiaku dengan perintah update set
```mysql
UPDATE User SET Password = PASSWORD('indonesiaku') WHERE User = 'Niomic';
```

![Nomor2](Nomor2.PNG)

### 3. Berikan hak akses ke user Niomic untuk tabel mahasiswa pada database belajar
```mysql
GRANT ALL ON belajar.mahasiswa TO Niomic@localhost;
```

![Nomor3](Nomor3.PNG)

### 4. Hapus user Niomic
###   SEBELUM DIHAPUS
![Nomor4Before](Nomor4Before.PNG)

###   SETELAH DIHAPUS
```mysql
DROP USER 'Niomic';
```

![Nomor4](Nomor4.PNG)
