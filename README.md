# labpy05
Nama : Sayyid Sulthan Abyan <p>
NIM : 312410496 <p>
Kelas : TI.24.A.5 <p>
Mata kuliah : Bahasa Pemrograman <p>
# 
1. Header dan Kelas Student:
     > print("\nProgram Input Nilai")
       print("===================")
      
       class Student:
           def __init__(self, nim, nama, tugas, uts, uas):
               self.nim = nim
               self.nama = nama
               self.tugas = tugas
               self.uts = uts
               self.uas = uas
               self.akhir = self.calculate_final_grade()
      
           def calculate_final_grade(self):
               return round((self.tugas * 0.3) + (self.uts * 0.35) + (self.uas * 0.35), 2)
      - Kode ini mencetak judul program dan mendefinisikan kelas Student yang memiliki atribut nim, nama, tugas, uts, uas, dan akhir.
      - calculate_final_grade adalah metode yang menghitung nilai akhir berdasarkan bobot tugas (30%), UTS (35%), dan UAS (35%).



   
