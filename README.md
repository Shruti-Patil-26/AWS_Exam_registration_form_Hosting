#AWS PHP and MySQL Website Hosting

1.Create EC2 Instance

2.Create RDS Database

3.Connect EC2 Inshance

![Connect_Options](https://github.com/Shruti-Patil-26/AWS_Exam_registration_form_Hosting/blob/7ba9db362ed1aec1cf3f28f85c925378a8ffffce/EC2_connect_option.jpg)


![Final_connect_option](https://github.com/Shruti-Patil-26/AWS_Exam_registration_form_Hosting/blob/7ba9db362ed1aec1cf3f28f85c925378a8ffffce/Final_connect_option.jpg)

4.Use Following Commands

   sudo -i
   
   apt update

   apt install apache2

   sudo apt install php libapache2-mod-php php-mysql

   cd /var/www/html

*Once enter in html folder check php running correctly or not

   create index.php and insert simple php code
       press escape and for save type :wq and press enter

*Create db.inc.php file and insert database details ,for that use Following command
   vi db.inc.php(filename)

*Check rds is connected to ec2 instance by command
   telnet (rds endpoint) 3306

*If not connected then add ec2 instance security group into rds security group inbound rule

*then again check by above command

*Install mysql client use below command
   apt install mysql-client
   
*Then Go to mysql server by below command
   mysql -u admin -h (rds endpoint ) -p

*create databases and tables and exit from mysql;

*Add main php code into either index.php file or create another file and insert into that

Final Output of My Hosting

![](https://github.com/Shruti-Patil-26/AWS_Exam_registration_form_Hosting/blob/7ba9db362ed1aec1cf3f28f85c925378a8ffffce/Login_page.jpg)


![](https://github.com/Shruti-Patil-26/AWS_Exam_registration_form_Hosting/blob/7ba9db362ed1aec1cf3f28f85c925378a8ffffce/Registration_form.jpg)


![](https://github.com/Shruti-Patil-26/AWS_Exam_registration_form_Hosting/blob/7ba9db362ed1aec1cf3f28f85c925378a8ffffce/Final_successful_message.jpg)
