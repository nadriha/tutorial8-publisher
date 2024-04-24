# Tutorial 8

* How many data your publlsher program will send to the message broker in one
run?  
  Program mengirimkan total lima pesan ke message broker  
  

* The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber
program, what does it mean?  
  penggunaan URL yang sama oleh publisher dan subscriber berarti mereka berinteraksi dengan message broker yang sama, yang memungkinkan mereka untuk berkomunikasi melalui message yang dikirim oleh publisher dan diterima oleh subscriber.

![image](https://github.com/nadriha/tutorial8-publisher/assets/116888619/e9f49418-3c43-493a-bd4f-f8f7937afe00)

![image](https://github.com/nadriha/tutorial8-publisher/assets/116888619/33cb0234-b571-4ee5-85d4-8f27c149dfaa)
Saat menjalankan perintah `cargo run` di publisher dan subscriber, Publisher mengirimkan data berupa 5 message broker yang diterima oleh Subscriber.

![messageImage_1713941627533](https://github.com/nadriha/tutorial8-publisher/assets/116888619/d605685c-bc56-4c15-840e-c1c53566be78)
Spike dalam message rate terjadi ketika banyak pesan dikirim dalam waktu singkat. Hal tersebut terjadi karena program publisher dijalankan berulang kali secara cepat sehingga menyebabkan penumpukan jumlah pesan dalam queue, segingga terjadi lonjakan tajam (spike) dalam message rate yang diterima broker.




