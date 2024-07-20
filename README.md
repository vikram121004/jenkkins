install jenkins java through


curl -fsSL https://pkg.jenkins.io/debianstable/jenkins.io-2023.key | sudo tee \
 /usr/share/keyrings/jenkins-keyring.asc >
/dev/null
echo deb [signed-by=/usr/share/keyrings/jenkinskeyring.asc] \
 https://pkg.jenkins.io/debian-stable binary/ |
sudo tee \
 /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
