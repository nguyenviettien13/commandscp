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
	```
    
- Cài đặt gói ssh trên các máy cần trao đổi dữ liệu:(ubuntu server 12.04,Desktop 12.04)
    
     	````
      		sudo apt-get install -y openssh-server
     	````
     
- Kiểm tra ip của máy:
   
    	````
       		ifconfig -a 
    	````

