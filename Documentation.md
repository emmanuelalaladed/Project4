# DOCUMENTTION-Project 4
## Step1: Install NodeJs

1. Update and upgrade the Ubuntu inux Operating system

*sudo apt update* and *sudo apt upgrade*

2. Add certificate

 *sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates*

 *curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -*

 3. Install NodeJS

     *sudo apt install -y nodejs*


## Step2: Install MongoDB, Node Package Manager and Body-Paser
# Note: The latest Ubuntu did not support the old Mongodb, therefore I installed the latest Mongodb 6.0 database.

1. Update the systtem and insytall the certificate

 *sudo apt update*
 *sudo apt install wget curl gnupg2 software-properties-common apt-transport-https ca-certificates lsb-release*

 2. Configure MongoDB Repo

 *echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list*

 3. Install MongoDB 6.0 on Ubuntu 22.04
 *wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1f-1ubuntu2.16_amd64.deb*
 *sudo dpkg -i ./libssl1.1_1.1.1f-1ubuntu2.16_amd64.deb* 
 *sudo apt update*
 *sudo apt install mongodb-org*

 4. After installation of MongoDB, start and enable MongoDB. Also verify the MongoDB version
  *sudo systemctl enable --now mongod*
  *systemctl status mongod*

5.  Install npm - Node Package Manager
 *sudo apt install -y npm*
6. Install body-parser
 *sudo npm install body-parser*

7. Create a directory "Books" and initialize npm project
 *mkdir Books && cd Books*
 *npm init*

8. Create a file "server.js" inside  directory "Books" using  *vi editor*
 *vi server.js*
9. Paste the web server code into the "server.js" file as shown below

10. My Code
 