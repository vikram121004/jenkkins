Install java
sudo apt install openjdk-17-jre java-version



curl-fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
/usr/share/keyrings/jenkins-keyring.asc> /dev/null
echo deb {signed-by=/usr/share/keyrings/jenkins-keyring.asc]\
https://pkg.jenkins.io/debain binary /|sudo tee \
/etc/apt/sources.list.d/Jenkins.list> /dev/null
sudo apt get update
sudo apt-get install jenkins
