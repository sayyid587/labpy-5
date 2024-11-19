# labpy05
Nama : Sayyid Sulthan Abyan <p>
NIM : 312410496 <p>
Kelas : TI.24.A.5 <p>
Mata kuliah : Bahasa Pemrograman <p>
# ```Program Input Nilai```
1. Header dan Kelas Student:
       print("\nProgram Input Nilai")
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
2. Fungsi Menampilkan Menu dan Daftar Mahasiswa:
   def display_menu():
       print("\n[(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari (K)eluar]: ", end=' ')

   def display_students(students):
       print("\nDaftar Nilai")
       print("=" * 84)
       print(f"| {'NO':<3} | {'NIM':<10} | {'NAMA':<30} | {'TUGAS':<6} | {'UTS':<4} | {'UAS':<4} | {'AKHIR':<5} |")
       print("=" * 84)
       if not students:
          print(f"| {'TIDAK ADA DATA':^80} |")
       else:
           for i, student in enumerate(students, start=1):
               print(f"| {i:<3} | {student.nim:<10} | {student.nama:<30} | {student.tugas:<6} | {student.uts:<4} | {student.uas:<4} | {student.akhir:<5} |")
       print("=" * 84)



   
