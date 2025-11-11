# LAPORAN PRATIKUM

## Nama: Rifaldi Syafikri Abdullah
## NIM: 05301425019
## MK : Sistem Operasi (project 2)
## Kelas : Sistem Informasi -A

### Script ini akan membuat folder baru dan mengisi setiap folder dengan file sample
https://drive.google.com/file/d/1leht-sc4bq_UtKWBPqcDZHP8EjHX7RzY/view?usp=sharing

mkdir documents images archives logs
touch spiscript1.sh script2.sh catatan2.txt error.log \ foto.jpeg audioku.mp3 testtderman.txt ironman.txt captain.txt file1.log file2.csv \gambar11.jpg gambar22.png laporan.docx catatnku.md \arsip.zip arsip2.tar.gz datapne.json datatwo.json \ script1.sh script2.sh catatan2.txt error.log \foto.jpeg audioku.mp3 testt.txt
ls

## Script Mengorganisasi File
### Script ini akan mengorganisasi setiap file sesuai ekstensinya 
https://drive.google.com/file/d/1mewkCbko1LO_0SbzLYGQK-yF58e46c_b/view?usp=sharing
mv *.jpg *.png *.jpeg images/
mv *.zip *.tar.gz archives/
mv *.log logs/
ls

## Fungsi Pencarian
### Saya telah menambahkan fitur pencarian agar mudah mencari file tertentu
https://drive.google.com/file/d/1-xZ7OgMTEmVH2Zytu8KKT43rdM0YEQOw/view?usp=sharing

find . -name "*.txt"
find . -size +1k
grep -R "ERROR" .

## Generet Laporan
### disini saya membuat script agar setiap perubahan pada file contohnya ukuran file, jumlah, dan tanggal di buat atau diubah. akan masuk pada file report.txt sebagai laporan
https://drive.google.com/file/d/1weilSwAokRuTRZePMJibtRbR9i7TxuVl/view?usp=sharing
https://drive.google.com/file/d/13G5-ShzYo9Sqjl_NSARHSBqqj4wW_edE/view?usp=sharing
https://drive.google.com/file/d/1uhxVoVB94Vw6_qOCMhTenoAU6365cQZh/view?usp=sharing

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
