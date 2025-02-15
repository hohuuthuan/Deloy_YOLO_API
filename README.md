# Deloy_YOLO_API

# Cấu hình web cho tệp tin index.php
C:\xampp\apache\conf\extra\httpd-vhosts

<VirtualHost *:80>	
    DocumentRoot "C:/xampp/htdocs" 
    ServerName localhost
</VirtualHost>

<VirtualHost *:80>    
    DocumentRoot "D:\Deloy_YOLO_API" 
    ServerName ttnt.localhost

    <Directory "D:\Deloy_YOLO_API"> 
        Options Indexes FollowSymLinks Includes ExecCGI
        AllowOverride All
        Require all granted
    </Directory>    
</VirtualHost>

# Khởi động API
python yolov8_predict.py

# Mở chrome gõ đường dẫn
ttnt.localhost

