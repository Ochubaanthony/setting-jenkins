Pre-requisites:
Azure Virtual machine is setup and running in Azure Cloud
ssh terminal to connect to Azure VM
Make sure 8080 port is opened in Networking-->Add inbound port role
Change Host Name to Jenkins
sudo hostnamectl set-hostname Jenkins
Perform update first
sudo apt update
Install Java 11
sudo apt install default-jdk -y
Verify Java Version
java -version
Maven Installation
Maven is a popular build tool used for building Java applications. Please click here to learn more about Maven. You can install Maven by executing below command:
sudo apt install maven -y
you can type mvn --version
Now lets start Jenkins installation
Add Repository key to the system


Update Ubuntu package
sudo apt update

Install Jenkins
sudo apt install jenkins -y


Access Jenkins in web browser

On Azure portal open port 8080 from Network
click on create port rule inbound
protocol TCP
CLICK on Add 

two ways to verified  "Terminal and Broswer
terminal 
curl localhost:8080

broswer
paste the public IP :8080
Copy the username and paste on the terminal
sudo cat /var/lib/jenkins/secrets/initialAdminPassword

copy the password generated and paste on the broswer
choose install suggested plugins