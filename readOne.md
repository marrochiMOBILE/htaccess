# htaccess
.htaccess adalah file konfigurasi tingkat direktori yang didukung oleh beberapa server web, yang digunakan untuk konfigurasi masalah akses situs web, seperti pengalihan URL, pemendekan URL, kontrol akses, dan banyak lagi. 'Titik' sebelum nama file menjadikannya file tersembunyi di lingkungan berbasis Unix.



#### ``` Options -Indexes ``` 
Artinya gini jika user membuka folder itu didalamnya tidak ada index.php/index.html maka jangan tampilkan isi foldernya dan block accessnya.

### ``` Options -Multiviews  ```
untuk membuka beberapa option

#### ``` RewriteEngine On  ```
untuk mengaktigkan Rewrite Engine

##### ``` RewriteCond %{REQUEST_FILENAME} !-d ```
untuk mengabaikan url yg sama dengan nama folder

##### ``` RewriteCond %{REQUEST_FILENAME} !-f ```
untuk mengabaikan url yg sama dengan nama file

##### ``` RewriteRule ^(.*)$  index.php?url=$1 [L] ```
ini adalah regex 

