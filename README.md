# LAN_File_Conveyor
#### 这是一款局域网文件传输的系统，无需安装任何APP就可以传送文件到局域网的任何一台设备上，只需要双方都打开这个网页即可
### 部署方式
###### 将client文件夹放到/www/LAN_File_Conveyor目录下
###### 先安装Nginx，然后将file.conf文件拷贝到nginx的v_host中，并根据实际情况修改
###### 将server文件夹放到/www/LAN_File_Conveyor目录中，然后进入到server，并运行
````
npm install
````
###### 将transfer.service放到/usr/lib/systemd/system/目录中，并输入
````
systemctl daemon-reload
systemctl start transfer
systemctl enable transfer
````
