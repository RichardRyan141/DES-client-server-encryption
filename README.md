# DES-client-server-encryption

Di code dianggap bahwa client memiliki IP 10.6.1.2 dan server memiliki IP 10.6.1.3  

Hal yang bisa dicustom
1) IP Server
   Dapat diubah di line 573 pada client.cpp ```server_address.sin_addr.s_addr = inet_addr("10.6.1.3");```
   Dan juga harus diubah di line 575 pada server.cpp ```server_address.sin_addr.s_addr = inet_addr("10.6.1.3");```
2) Key
   Dapat diubah di line 592 pada client.cpp ```key = "0F1E2D3C4B5A6978";```
   Dan juga harus diubah di line 607 pada server.cpp ```key = "0F1E2D3C4B5A6978";```
   Key harus berupa 16 karakter yang hanya mengandung 0-9, a-f atau A-F
3) Host to Host
   Apabila ingin diubah menjadi komunikasi host to host, maka dapat di uncomment baris 651-653 pada server.cpp kemudian mencomment baris 633-649
