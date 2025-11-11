# tugas_so_saira
# LAPORAN PRATIKUM
## Nama: Sasa Saira Kiay Mojo
## NIM: 05301425015
## MK : Sistem Operasi (project 1)
## Kelas : Sistem Informasi -A
## Script Membuat Struktur Direktori
### Script ini akan membuat folder baru dan mengisi setiap folder dengan file sample
https://drive.google.com/file/d/1n9z3aYPCjlhpLa7ADP5JwMM2xAFH0tcx/view?usp=sharing

mkdir documents images archives logs
touch biru.txt merah.txt kuning.txt hijau.log hitam.csv / gambarsatu.jpg gambardua.png laporankeuangan.docx catatanhidup.md / arsipsatu.zip arsipdua.tar.gz dataone.json datatwo.json / script11.sh script22.sh catatanmati.txt error.log / fotokatanya.jpeg audiokatanya.mp3 testtest.txt
ls

## Script Mengorganisasi File
### Script ini akan mengorganisasi setiap file sesuai ekstensinya 
https://drive.google.com/file/d/1NG3LvMvNWHLD4Vkao6Xbei5NA4xDRnYb/view?usp=sharing

mv *.txt *.md documents/
mv *.jpg *.png *.jpeg images/
mv *.zip *.tar.gz archives/
mv *.log logs/
ls

## Fungsi Pencarian
### Saya telah menambahkan fitur pencarian agar mudah mencari file tertentu
https://drive.google.com/file/d/1VVQ9iuhpbMfx2iTJzGi0DcSj3w8t3-ZP/view?usp=sharing

find . -name "*.txt"
find . -size +1k
grep -R "ERROR" .

## Generet Laporan
### disini saya membuat script agar setiap perubahan pada file contohnya ukuran file, jumlah, dan tanggal di buat atau diubah. akan masuk pada file report.txt sebagai laporan
https://drive.google.com/file/d/1QjKUM4vS9nrXM6hnVjxkDnKFYs-62Y-t/view?usp=sharing
https://drive.google.com/file/d/1o-89EawfOLplM76MFsoUM8JqDGX1kt-0/view?usp=sharing
https://drive.google.com/file/d/16AEKOgfYSXe57dHoLoI_SY-RxEaZqZbR/view?usp=sharing

echo "=== laporan file system ===> report.txt
date >> report.txt
echo >> report.txt
echo "jumlah file:" >> report.txt
ls -R | wc -1>> report.txt
echo "" >> report.txt
echo "ukuran masing-masing folder:" >> report.txt
dush >> report.txt
echo >> report.txt
echo "jumlah baris di semua file teks:" >> report.txt
wc 1 documents/*.txt >> report.txt
cat report.txt
