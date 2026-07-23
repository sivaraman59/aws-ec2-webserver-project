# AWS EC2 Web Server Project

## Objective
Deploy a web server on an Amazon EC2 instance.

## Services Used
- Amazon EC2
- Security Group
- Key Pair

## Steps
1. Launch EC2 instance
2. Connect using SSH
3. Install Apache
4. Start Apache service
5. Create index.html
6. Access website using Public IP

## Commands Used

```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
```

```bash
echo "<h1>Hello AWS</h1>" | sudo tee /var/www/html/index.html
```
## Screenshots

### EC2 Instance Running
![EC2](screenshots/01-ec2-instance-running.png)

### SSH Login
![SSH](screenshots/02-ssh-login.png)

### Apache Service Running
![Apache](screenshots/03-httpd-service-running.png)

### Website Output
![Website](screenshots/04-hello-aws-webpage.png)

## Result

Successfully deployed a web server on Amazon EC2.
