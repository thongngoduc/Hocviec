# **Hướng dẫn sử dụng MobaXterm để SSH vào server linux**
Đối với các hệ điều hành của họ Linux như CentOS, Ubuntu, Fedora, Debian … thì việc điều khiển thông thường thực hiện qua thao tác dòng lệnh CLI. Để thực hiện việc này, người dùng sẽ sử dụng các phần mềm như Putty, MobaXterm, XShell để thực hiện SSH tới port mặc định 22 của máy chủ. Trong hướng dẫn này, mình sẽ hướng dẫn với các bạn sử dụng MobaXtem.

**1. Các tình năng hay của MobaXtem**

MobaXterm có những tính năng hay ho hơn so với việc sử dụng Putty, nó giúp người dùng thao tác tốt hơn khi điều khiển các máy chủ linux, bao gồm:

- Hỗ trợ mở nhiều cửa sổ để làm việc.
- Hỗ trợ tích hợp việc FTP hoặc SFTP để truyền file từ máy người dùng lên máy chủ.
- Hỗ trợ các thao tác zoom màn hình CLI hoặc thay đổi màu sắc bắt mắt hơn.
- Hỗ trợ các phương thức kết nối như FTP, Telnet, RDP (remote desktop với các máy là windows)
- Hỗ trợ các công cụ dùng để scan port, scan network.
- Lưu phiên đăng nhập sau lần đầu truy cập vào SSH hoặc các giao thức khác.

**2. Cách sử dụng MobaXterm**

**2.1. Tải MobaXterm**

MobaXtem cung cấp 2 phiên bản, phiên bản free – Home Edition và phiên bản mất phí – Professional Edition. Đối với người dùng thông thường, chỉ cần tải bản free là đủ (bản free) cho phép lưu 10 section SSH đầu tiên (có thể hiểu là 10 máy chủ).

Khi tải bản free, bạn có thể chọn dạng portable (giải nén và dùng ngay) hoặc dạng install (tải và cài đặt). Thực hiện tải bản free – Home Edition ở link dưới: https://mobaxterm.mobatek.net/download-home-edition.html

Trong hướng dẫn này sẽ chọn dạng file cài đặt đối với bản Home Edition

![https://news.cloud365.vn/wp-content/uploads/2019/10/mobaxterm1-1024x443.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.001.png)

*Hình 1. 1   Tải MobaXterm Home Edition (bản Free) – tải file dạng cài đặt*

Sau khi tải về, tiếp tục thực hiện các thao tác cài đặt. Trong quá trình cài đặt thực hiện các tùy chọn mặc định là đủ để sử dụng.
###
### **2.2. Sử dụng MobaXterm để truy cập SSH**
Sau khi cài đặt xong, tiến hành mở MobaXterm, ta sẽ có giao diện dưới.

![https://news.cloud365.vn/wp-content/uploads/2019/10/mobaxterm2.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.002.png)

*Hình 2. 1   Giao diện của MobaXterm*

Thưc hiện thao tác để mở cửa sổ kết nối SSH tới server của bạn. Ta chọn tab Section=> New section. Ngoài ra, có thể thực hiện tổ hợp phím Ctl + Shif + N , ta cũng có kết quả tương tự.

![https://news.cloud365.vn/wp-content/uploads/2019/10/mobaxterm3-1.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.003.png)

Cửa sổ mới hiện ra sau thao tác trên sẽ có dạng như bên dưới. Chọn tab SSH

![https://news.cloud365.vn/wp-content/uploads/2019/10/mobaxterm4-1024x737.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.004.png)

*Hình 2. 2    Cửa sổ hiển thị yêu cầu người dùng nhập vào để truy cập SSH.*

Tại cửa sổ trên, tiến hành nhập địa chỉ IP và port của máy chủ. Thường thì mặc định giá trị port SSH sẽ là 22 nếu như bạn không có thay đổi gì. Trong hướng dẫn này mình sẽ kết nối tới IP có địa chỉ là 103.124.92.133 với các thông tin như sau:

- Remote host: điền địa chỉ IP, trong hướng dẫn này là 103.124.92.133
- Port: Điền port SSH của máy chủ, mặc định là: 22
- Trường còn lại bỏ trống.

Sau khi nhập xong, chọn OK.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba4-1024x690.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.005.png)

Sau khi chọn OK, ta sẽ có giao diện để nhập user và mật khẩu của máy chủ. Thường sẽ sử dụng user có tên là root và mật khẩu được cung cấp trước đó.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba5-1024x381.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.006.png)

*Hình 2. 3   Nhập tài khoản và mật khẩu.*

Lưu ý, khi nhập mật khẩu sẽ không hiển thị dấu \* như các ứng dụng khác, bạn có thể chép mật khẩu ra notepad và paste lại ở màn hình trên.


![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba6-1024x605.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.007.png)

*Hình 2. 4   Màn hình sau khi nhập đúng mật khẩu cho tài khoản root*

Ở màn hình trên, ta chọn Yes để mỗi lần đăng nhập lại ta không cần khai báo lại mật khẩu. Cũng lưu ý việc này nên cân nhắc vì mật khẩu sẽ được lưu trên máy của bạn. Trong hướng dẫn của cửa sổ trên cho phép xóa các mật khẩu được lưu này nếu bạn muốn.

Sau khi chọn YES ta sẽ có màn hình dưới.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba7-1024x572.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.008.png)

*Hình 2. 5   Màn hình CLI sau khi đăng nhập thành công.*

Ta có thể kiểm tra phiên bản hệ điều hành bằng lệnh cat /etc/\*-release. Kết quả sẽ hiển thị dạng như bên dưới.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba8-1024x761.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.009.png)

*Hình 2. 6    Kết quả lệnh cat /etc/\*-release*

Hoặc có thể kiểm tra bằng các lệnh khác như: ip address

Tới đây bạn đã truy cập SSH thành công và có thể bắt đầu thao tác.


### **2.3. Các thao tác khác với MobaXterm**
Ngoài sử dụng SSH, MobaXterm còn có có thế sử dụng để thực hiện truyền file thông qua sftp. Trong hướng dẫn này mình sẽ hướng dẫn bạn up file từ máy tính cá nhân lên máy chủ thông qua MobaXterm.

Chọn tab sftp theo hình dưới.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba9.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.010.png)

*Hình 2. 7    Tab SFTP*

Chọn biểu tượng upload

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba10.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.011.png)

*Hình 2. 8   Chọn biểu tượng upload*

Chọn file cần upload từ máy tính và chọn Open

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba11.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.012.png)

Sau khi chọn file, tùy thuộc vào dung lượng mà thời gian up sẽ là nhanh hay chậm. Ta có thể quan sát ở màn hình giống như bên dưới.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba12.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.013.png)

*Hình 2. 9  Màn hình theo dõi tỉ lệ up dữ liệu từ máy tính cá nhân lên server.*

Sau khi thực hiện upload xong, ta có thể kiểm tra tại thư mục /root/ của máy chủ xem file đã có hay chưa bằng lệnh ls -alh tại thư mục /root/.

![https://news.cloud365.vn/wp-content/uploads/2019/10/Moba13-1024x674.png](Aspose.Words.942b691c-0902-4b3b-ad79-ad4d5deee29b.014.png)

*Hình 2. 10   Kết quả file đã được đưa lên máy chủ.*
## **3. Kết luận**
Trong hướng dẫn này, mình đã hướng dẫn bạn sử dụng cơ bản về MobaXteam. Bạn có thể trải nghiệm thêm các tính năng khác của nó ở trên các tab, hãy tự trải nghiệm và chia sẻ cùng chúng tôi nếu bạn muốn nhé.

# **TÀI LIỆU THAM KHẢO**
[1]. <https://thachpham.com/tools/mobaxterm-giup-ban-quan-ly-vps-qua-ssh-tot-hon.html>

[2]. <https://news.cloud365.vn/ssh-mobaxterm-huong-dan-su-dung-mobaxterm-de-ssh-vao-server-linux/>

[3] <https://tinhte.vn/thread/moba-xterm-cong-cu-aio-cho-cac-lap-trinh-vien.2807754/>


