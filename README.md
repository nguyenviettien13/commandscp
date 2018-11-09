_***Hướng dẫn sử dụng lệnh SCP***_
========
#### Tìm hiểu lệnh SCP.

#### I. SCP là gì?
- SCP (Secure Copy – Sao chép an toàn) là một ứng dụng sử dụng SSH để mã hóa toàn bộ quá trình chuyển tập tin.
- SCP  là lệnh dùng để di chuyển file dữ liệu giữa các máy tính chạy hệ điều hành Linux từ xa chỉ cần biết địa chỉ ip
- SCP dùng ssh để di chuyển dữ liệu, có chế độ bảo mật giống như ssh.
#### Cài đặt sử dụng

##### 2.1 Cài đặt scp
- Scp có sẵn trong các bản dis của hệ điều hành Linux.Nếu chưa có , cài đặt như sau :

	```
		Ubuntu/Debian : sudo apt-get install scp -y
		Fedora/RedHat/Centos: yum install scp -y

- Cài đặt gói ssh trên các máy cần trao đổi dữ liệu:(ubuntu server 12.04,Desktop 12.04)
	```
		sudo apt-get install -y openssh-server

- Kiểm tra ip của máy:
	```
		ifconfig -a

##### 2.2 Sử dụng scp
- Trên hệ điều hành linux: (Ubuntu 16.04):
	- Cú pháp sử dụng chung
	 ```
		scp [-pqrvBC46 ] [-F ssh_config ] [-S program ] [-P port ] [-c cipher ] [-i identity_file ] [-o ssh_option ] [[user@ ] host1 : file1 ] [... ] [[user@ ] host2 : file2 ]
	 ```
	- options:
	 ```
		-c  : Chọn thuật toán mã hóa để sử dụng cho việc mã hóa việc truyền dữ liệu
		-i  : Lựa chọn các tập tin mà từ đó nhận dạng (khóa riêng) cho RSA xác thực được đọc
		-p : backup lại file gốc.
		-r : sao chép lại toàn bộ thư mục.
		-C : nén  file trong khi thực hiện:
		-v : cung cấp thông tin chi tiết của quá trình.
		-1 : Forces scp to use protocol 1.
		-2 : Forces scp to use protocol 2.
	 ```
##### 2.3 Áp dụng
	  - Mô hình
<img src="https://imgur.com/a/osLtjru">
