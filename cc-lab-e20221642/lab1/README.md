# Cloud Lab 1: Amazon EC2

**Student name:** CHORK RATANAKDAVID  
**Student ID:** e20221642  
**Learner Lab user name:** voclabs/user/5619240=CHORK_RATANAKDAVID  
**Date completed:** October 22, 2026

## Part 1.1: An Amazon EC2 Walkthrough

### Security group
![Security group](images/01-security-group.png)

### Key pair
![Key pair](images/02-key-pair.png)

### Instance details
![Instance details](images/03-instance-details.png)

### Browser test
![Browser test](images/04-browser-test.png)

### SSH connection
![SSH connection](images/05-ssh-connection.png)

**Did you connect with your own SSH client or with EC2 Instance Connect?**
I connected with my own SSH client using Ubuntu.



## Part 1.2: EC2 Web Solution (Challenge)

### Launch configuration
![Launch configuration](images/06-challenge-launch.png)

### Security group
![Challenge security group](images/07-challenge-security-group.png)

### Running instance
![Challenge instance](images/08-challenge-instance.png)

### Commands on the instance
![Terminal commands](images/09-challenge-terminal.png)


**The command that ran to install the web server and create index.html:**
```bash
sudo dnf update -y
sudo dnf install -y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
echo "Welcome to the EC2 Challenge" | sudo tee /var/www/html/index.html
```
### Browser test
![Welcome to the EC2 Challenge](images/10-challenge-browser.png)