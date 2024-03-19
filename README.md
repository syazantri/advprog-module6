# ✨Reflection🪞
Syazantri Salsabila - AdvProg B - 2206029443 <hr>

1️⃣ Commit 1 Reflection Notes
> ***What is inside the handle_connection method?*** <br>
> Di dalam method ini, ada ```BufReader``` yang me-wrap TcpStream. ```BufReader``` ini bakal nyimpen data berskala besar secara buffering dengan mengelola method calling dari trait std::io::Read. Kemudian data akan dibaca line by line pakai ```.lines()``` sampai line nya habis/empty. Variable yang mengambil line tersebut kita namakan ```http_request``` yang kemudian akan disimpan ke dalam vektor karena kta menggunakan ```Vec<_>``` . 

2️⃣ Commit 2 Reflection Notes <br>
![Commit 2 screen capture](assets/images/commit2.png) 
> ***What have you learned about the new code the handle_connection.*** <br>
> Pada method handlle_connection yang baru, setelah membaca request, method juga akan menghasilkan HTTP response. Isinya adalah status line (```"HTTP/1.1 200 OK"```), header, dan isi dari file ```hello.html``` yang telah diconvert ke String menggunakan ```fs::read_to_string("hello.html").unwrap()```. Konten ini akan menjadi body dari response. Lalu headernya akan berisi content length.