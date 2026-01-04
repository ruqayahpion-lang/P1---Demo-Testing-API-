# P1---Demo-Testing-API-
Mata Kuliah  
Dosen Pengampu  
Praktikum  
Nama Mahasiswa 
NIM   
Kelas   
Tanggal Praktikum 
:Web Service Engineering  
:Muhayat, M.IT  
:P1 - Demo Testing API 
:Ruqayah 
:230104040208 
:TI23A 
:15-09-2025 
A. Tujuan Praktikum 
1. Mengenal konsep dasar API (Application Programming Interface). 
2. Melakukan pengujian request HTTP (GET, POST, PUT, DELETE) menggunakan 
Postman. 
3. Menganalisis perbedaan hasil request terhadap server API JSONPlaceholder. 
B. Dasar Teori 
• API adalah antarmuka yang memungkinkan komunikasi antar sistem atau aplikasi. 
• HTTP Methods:  
o GET → Mengambil data dari server. 
o POST → Menambahkan data baru ke server. 
o PUT → Memperbarui data yang sudah ada. 
o DELETE → Menghapus data dari server. 
• JSON (JavaScript Object Notation) adalah format data ringan berbentuk key–value 
yang digunakan secara luas dalam API modern. 
C. Langkah Percobaan dan Hasil 
1. GET All Post 
• Endpoint: https://jsonplaceholder.typicode.com/posts 
• Method: GET 
• Hasil: Berhasil menampilkan seluruh data postingan (100 data). 
2. GET Post by ID 
• Endpoint: https://jsonplaceholder.typicode.com/posts/1 
• Method: GET 
• Hasil: Berhasil menampilkan 1 data postingan dengan ID = 1. 
3. GET Comments by PostID 
• Endpoint: https://jsonplaceholder.typicode.com/comments?postId=1 
• Method: GET 
• Hasil: Berhasil menampilkan daftar komentar berdasarkan postId=1.
4. POST Create Post 
• Endpoint: https://jsonplaceholder.typicode.com/posts 
• Method: POST 
• Body (JSON):  
• { 
•   "title": "Belajar API", 
•   "body": "Ini percobaan pertama", 
•   "userId": 1 
• } 
• Hasil: Berhasil membuat data baru dengan response 201 Created.
5. PUT Update Post 
• Endpoint: https://jsonplaceholder.typicode.com/posts/1 
• Method: PUT 
• Body (JSON):  
• { 
•   "id": 1, 
•   "title": "Belajar API Update", 
•   "body": "Isi sudah diperbarui", 
•   "userId": 1 
• } 
• Hasil: Berhasil memperbarui data pada id=1 dengan status 200 OK. 
6. DELETE Post 
• Endpoint: https://jsonplaceholder.typicode.com/posts/1 
• Method: DELETE 
• Hasil: Berhasil menghapus data pada id=1 dengan response kosong {} dan status 200 
OK. 
C. Analisis 
Dari hasil uji coba CRUD API: 
1. GET menampilkan data baik seluruh koleksi maupun berdasarkan parameter tertentu. 
2. POST berhasil membuat data baru, walaupun JSONPlaceholder hanya memberikan 
simulasi (tidak benar-benar menyimpan data). 
3. PUT memperbarui data dengan struktur JSON sesuai request. 
4. DELETE memberikan response kosong namun status 200 OK menandakan operasi 
berhasil. 
Hal ini membuktikan bahwa API mendukung operasi CRUD penuh sesuai standar HTTP   
methods. 
F. Kesimpulan 
1. Postman dapat digunakan untuk menguji API dengan berbagai metode HTTP. 
2. JSONPlaceholder menyediakan endpoint simulasi CRUD API. 
3. Setiap metode HTTP (GET, POST, PUT, DELETE) memiliki fungsi berbeda yang 
dapat diuji secara praktis.
