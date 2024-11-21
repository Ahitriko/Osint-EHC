đầu tiên khi đọc challenge thì mình nghĩ có thể kẻ giả mạo sẽ để tên là EHC nhưng khi mình tìm cũng không thấy gì đặc biệt nên mình chuyển sang tìm thử FPTU EHC thì mình có tìm được một tài khoản X 
![image](https://github.com/user-attachments/assets/904860f3-d824-495e-85a2-bbcba9d031cc)
tại profile của FPTU EHC mình thấy được chút thông tin : Remember to check my secret: aHR0cHM6Ly93d3cueW91dHViZS5jb20vd2F0Y2g/dj1kUXc0dzlXZ1hjUQ==
mình thấy đây là dạng mã hóa base64 và thử decode nó và nhận được link youtube 
![image](https://github.com/user-attachments/assets/140f242a-df04-4101-88be-d8004a027475) 
mình để ý tại profile của FPTU EHC còn có một đường dẫn qua linked profile nên mình theo đó 
![image](https://github.com/user-attachments/assets/2a69e8d6-e5be-4bb0-858f-09d35236b315)
tại đây mình thấy được một đoạn mã nữa và khi decode nó mình ra đc flag đầu tiên : EHC{HappyB1rthd4y_
![image](https://github.com/user-attachments/assets/c707f6fe-2561-4154-bbba-9a65abb5e576)
mình còn tìm thêm được một link dẫn qua github nữa 
![image](https://github.com/user-attachments/assets/6f62d8b2-a0de-4038-9650-ee975de9e760)
![image](https://github.com/user-attachments/assets/167f4b18-a6db-449d-8148-64265f688957)
trong repositories Ethical-Hackers-Club thì mình đọc file December 9.md thì mình thấy được một đoạn khá đáng chú ý là : Is it a QR around here???
![image](https://github.com/user-attachments/assets/8329cdc0-06aa-42a7-96d6-45a8b20fb8a3)
mình đã xem các commit và nhận ra một commit đã được sửa đổi có ảnh qr khá đặc biệt là nó khác với các ảnh khác 
![image](https://github.com/user-attachments/assets/abb86b2b-61a1-44e3-b922-dbca73029d1f)
mình tìm được nó khi check commit tại create_D5
và khi mình đã quét qr và nhận được một đoạn mã binary 
01001000 01101111 01110111 00100000 01100011 01100001 01101110 00100000 01111001 01101111 01110101 00100000 01100111 01100101 01110100 00100000 01101000 01100101 01110010 01100101 00111111 00111111 00111111 00100000 01001001 01110011 00100000 01101101 01111001 00100000 01110101 01110011 01100101 01110010 01101110 01100001 01101101 01100101 00100000 01110011 01110101 01110011 01110000 01101001 01100011 01101001 01101111 01110101 01110011 00111111 00111111 00111111 (khúc này máy mình k quét được nhưng mình thử máy khác thì ra như vậy :V)
và khi decode nó ra thì mình nhận được 
![image](https://github.com/user-attachments/assets/0b3a07ed-d040-4498-8cc3-7dbdfbd35f98)
tiếp tục đọc các commit khác thì mình thấy những điều khá thú vị 
![image](https://github.com/user-attachments/assets/df649ad5-ec7a-410a-9c8f-91ccae016dfc) 
![image](https://github.com/user-attachments/assets/91dbaad4-fe23-4db5-bda7-25b59cc78add) (Update D7)
![image](https://github.com/user-attachments/assets/6663e525-4983-4908-9707-e2abb000e428) (D9)

dựa vào đây mình có thể để ý thêm username của tk này là ehcbirthday và sử dụng tại một place same avt
mình nghĩ có thể nó là một loại mail nên mình đã thử khá nhiều tên như ehcbirthday@gmail.com, ehc02122017@gmail.com....
nhưng đều k được, để ý đến đoạn text từ D9 thì mình đã sửa lại thành sinhnhatehc@gmail.com, và khi gửi tin nhắn cho mail này mình đã nhận được một đoạn tin nhắn khá thú vị
![image](https://github.com/user-attachments/assets/f2ef27e5-f53f-47ee-9b39-6553acd736f0)
mình đã check các video thì đều là rockroll và cuối các link này đều giống nhau ,ngoại trừ kí tự cuối link
![image](https://github.com/user-attachments/assets/c4e14818-9fcd-4a7b-b87b-7009a704b458)
lần lượt mình lấy ra sẽ là "calendar"
mình nghĩ là mình có thể tìm được gì đó với gợi ý trên và mình nghĩ đến chính là gg calendar 
mình dùng một web là Epieos và nhập mail sinhnhatehc@gmail.com vô thì mình có được link dẫn đến gg calendar của tk mail này
![image](https://github.com/user-attachments/assets/01876cf4-b177-4a6e-ae02-774b16fc843b)
![image](https://github.com/user-attachments/assets/c313be3a-d688-4906-9553-02ef5633c34b)
tại ngày 02/12 tk này có để một note và khi xem nó mình có link dẫn đến discord
![image](https://github.com/user-attachments/assets/5e68f21f-335b-4710-b322-24f14ce73db4)
khi vào được discord thì mình thấy được một đoạn mã thông báo từ Anh Shidou nhưng khi decode ra mình nhận được một link youtube :))
mình nhớ tại một challenge của một giải ctf nào đó mà mình k nhớ tên (mình có thể ẩn thông tin trong tin nhắn) nên mình đã copy và dán nó qua chỗ khác
![image](https://github.com/user-attachments/assets/c85fbe8f-ac6e-4e4a-9ea1-8e5c3a37ec61)
và mình nhận được một secret : RUhDXw== và decode ra chính là "EHC_"
đến với chatbot thì mìnhd đã thử các lệnh /get fake flag và get real flag
![image](https://github.com/user-attachments/assets/60c3c9c3-d8e9-413b-93a0-23637163538b)
cũng tương tự như trên mình copy các reply của chatbot thì mình nhận được thêm thông tin là 
![image](https://github.com/user-attachments/assets/a0516e49-e3b1-4f38-8cbf-473d10ff06b5)
khi chạy /get fake flag
và mình ib trực tiếp cho con bot này
sau khi mình thử khá nhiều pass như "password","ehcbirthday","sinhnhatehc0212" và mình nhận được thông tin hữu ích khi dùng pass 0212
![image](https://github.com/user-attachments/assets/91755546-ed76-4b2c-93d1-c5989cb7b639)
ban đầu mình cũng k nhìn rõ password bên dưới nên mình tưởng bị sai, nhưng khi để ý lại thì mình thấy có một khoảng trống bên dưới tin nhắn và lờ mờ chữ gì đó và khi ấn vô mình thấy last part của flag : "_02l2@!!}"
![image](https://github.com/user-attachments/assets/2b5b2cbd-59c7-474e-8fe3-a5cf4cadfd4b)

và toàn bộ flag là : "EHC{HappyB1rthd4y_EHC_02l2@!!}"
