Nama: Zita Nayra Ardini 
NPM: 2406404913 
Kelas: Pemrograman Lanjut B

# Reflection notes
a. Apa itu AMQP?
AMQP (Advanced Message Queuing Protocol) adalah protokol standar terbuka untuk message-oriented middleware. Protokol ini memungkinkan komunikasi asinkron antar aplikasi atau komponen yang berbeda, dengan dukungan fitur seperti routing, queuing, reliability, dan keamanan. Dalam tutorial ini, RabbitMQ menggunakan AMQP sebagai protokol utama untuk mengirim dan menerima pesan antara publisher, message broker, dan subscriber.

b. Apa arti guest:guest@localhost:5672?
String guest:guest@localhost:5672 adalah URL yang digunakan oleh publisher dan subscriber untuk terhubung ke message broker RabbitMQ. Bagian guest:guest menunjukkan username dan password default bawaan RabbitMQ, sedangkan localhost merujuk pada alamat host tempat broker berjalan. Angka 5672 adalah port default untuk protokol AMQP (non-TLS). Karena URL ini sama persis pada kode publisher dan subscriber, artinya kedua program terhubung ke broker yang sama, sehingga mereka dapat bertukar pesan melalui queue dengan nama yang sama (user_created).
