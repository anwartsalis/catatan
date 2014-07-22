#Overview

Moco: Reading Socially

Moco adalah sebuah platform media sosial untuk mengakses e-Bookstore & e-Pustaka, membangun jaringan/komunitas sesama pembaca, dan juga tentunya sebagai e-Reader untuk membaca eBook. Moco dapat diakses di berbagai medium perangkat mulai dari desktop dan PC berbasis situs (web-based), netbook dan tab based hybrid (tab-base application), dan mobile (smartphone-based application).

Agar Moco dapat dijalankan di berbagai perangkat tersebut maka di kembangkan API (Application Programming Interface). Dokumentasi ini akan memberikan penjelasan teknis kepada para developer dalam menggunakan servis-servise dari Moco API untuk mengembangan aplikasi klien pada masing-masing perangkat yang telah disebutkan di atas.

Berikut ini adalah beberapa hal yang perlu diperhatikan untuk dapat menggunakan servis-servis dari Moco API:

Base URL API

Berikut ini adalah base url untuk API Moco:

Production

1 |
http://store.aksaramaya.com/apis/

Development

1 |
http://webstore.aksaramaya.com/apis/


Meta Header API Response

code|Keterangan|Format meta data
----|----------|----------------
404|Data not found|{“meta”:{“code”:404,”error_message”:”Not Found”}}
401|Unauthorized client app|{“meta”:{“code”:401,”error_message”:”Unauthorized”}}
400|Bad request|{“meta”:{“code”:400,”error_message”:”Bad request”}}
200|Success|{“meta”:{“code”:200,”confirm”:”success”}}
