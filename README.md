# Summary git & github 

1. **Git** merupakan sebuah VCS (Version Control System) yang fungsinya untuk melakukan sebuah pengaturan versi atau pelacakan perubahan yang ada karena pada dasarnya tidak akan ada code yang sempurna.
2.  VCS awalnya bersifat single user(hanya ada di lokal) 1970an-1982, setelah itu bersifat centralized (ada di server pusat ketika server error tidak bisa edit) 1986-2005, dan terakhir Distributed(ada di lokal dan juga ada di server) ex: git. ada mulai tahin 2005
3. Beberapa comand git yang sering digunakan :  
	 - git add (menambah file dan memasukannya ke staging area),
	 - git status(mengecek status perubahan seperti penambahan dan pengurangan file yang ada), 
	 - git commit(mengcommit file yang ditambahkan tadi ke repository,biasanya disertai dengan sebuah message),
	 -  git diff(mengetahui perubahan yang terjadi dari project), git stash(menyimpan file/kode yang sedang dikerjakan namun belum di commit),
	 -  git log(mengecek semua log perubahan yang ada dari id commit dan lainnya),
	 -  git reset (melakukan pengembalian pada commit tertentu), git push (melakuakn push ke server pada file yang sudah di commit),
	 -  git fetch(mengambil data yang ada dalam server),
	 -  git pull(ambil perubahan yang ada di branch dan di merge ke branch kita), git merge(mengambil perubahan yang ada pada branch lain)



# Praktikum

Berikut step by step yang dilakukan saat praktikum : 
1. Implementasi penggunaan branching yang terdiri dari master, development, featureA, dan featureB
.
[![branch.jpg](https://i.postimg.cc/nzRyPwQ8/branch.jpg)](https://postimg.cc/JDXYyxqK).
2. Implementasi git push untuk push file hello.dart pertama kali
[![git-push.jpg](https://i.postimg.cc/FKBRjGsR/git-push.jpg)](https://postimg.cc/jWytTHf0).
3. Implementasi git pull pada hello.dart.
Pertama kita ubah dulu data pada server seperti gambar berikut : 
[![pull-server.jpg](https://i.postimg.cc/wjWJGXjK/pull-server.jpg)](https://postimg.cc/752fCTzX)
.
Data yang ada dilocal akan berbeda dengan di server setelah dipush  berikut data yang ada di local.
[![pull-local.jpg](https://i.postimg.cc/Xvd2S1GG/pull-local.jpg)](https://postimg.cc/GB3PvQjd)
.
Karena adanya perbedaan data/ file pada local dan  maka dapat dilakukan git pull dengan command berikut : 
.
[![git-pull-cmd.jpg](https://i.postimg.cc/nVPP6P02/git-pull-cmd.jpg)](https://postimg.cc/8sL4vt8f)
.
4. Implementasi git stash
apabila terdapat perbedaan antara data di local dan di server yang belum kita push dapat dilakukan git stash untuk menyimpan perubahan local kita yang masih belum di push agar tidak conflict. syntaxnya sebagi berikut : 
.
[![git-stash.jpg](https://i.postimg.cc/yNr7tT5Z/git-stash.jpg)](https://postimg.cc/hJTF7VKD)
Setelah tersimpan nantinya stash dapat dikembalikan dengan menggunakan command berikut : 
.
[![git-stash-apply.jpg](https://i.postimg.cc/rpRHyCsW/git-stash-apply.jpg)](https://postimg.cc/sBymwWpD).
.
5. Implementasi git merge 
syntax untuk melakukan merge pada branch featureB ke development
.
[![git-merge.jpg](https://i.postimg.cc/fRqLQZSy/git-merge.jpg)](https://postimg.cc/JsJmjfqC)
.
6. Studi kasus penyelesaian conflict.
 misal pada branch development akan diimplementasikan 2 buah fitur yaitu fitur A dan B pertama kita merge fitur B lalu kita merge fitur A namun terdapat conflict karena fitur A dan B terdapat baris sama yang berisi sebuah code berbeda 
 .
 [![conflict-merge.jpg](https://i.postimg.cc/V6VpzGBj/conflict-merge.jpg)](https://postimg.cc/zbT0jkQB)
 .
 dan file conflict seperti berikut : 
 .
  [![conflict-A-and-B.jpg](https://i.postimg.cc/0y7scsGh/conflict-A-and-B.jpg)](https://postimg.cc/0z5FyhBC)
 .
kita dapat menyelesaikannya dengan memilih salah satu file yang benar. misal kita tidak jadi mengimplementasikan fitur A jadi setelah di solve maka akan menjadi sebgai berikut : 
.
[![after-merge.jpg](https://i.postimg.cc/hvKkyzrY/after-merge.jpg)](https://postimg.cc/ZBDs0qXP)
.
Berikut hasil dari insight nya : 
.
[![insight.jpg](https://i.postimg.cc/05mGZXMh/insight.jpg)](https://postimg.cc/xqfb1RPP)
