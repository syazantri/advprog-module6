# ✨Reflection🪞
Syazantri Salsabila - AdvProg B - 2206029443 <hr>

1️⃣ Commit 1 Reflection Notes
> ***What is inside the handle_connection method?*** <br>
> Di dalam method ini, ada ```BufReader``` yang me-wrap TcpStream. ```BufReader``` ini bakal nyimpen data berskala besar secara buffering dengan mengelola method calling dari trait std::io::Read. Kemudian data akan dibaca line by line pakai ```.lines()``` sampai line nya habis/empty. Variable yang mengambil line tersebut kita namakan ```http_request``` yang kemudian akan disimpan ke dalam vektor karena kta menggunakan ```Vec<_>``` .