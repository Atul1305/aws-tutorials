## AWS-CLI <br>
Command start with aws. You can perform all actions you can do through AWS Console.

<br>
**Points** <br>
* Roles are more secure than storing your access key and secret key on individual EC2 instances.<br>
* Roles are easier to manage. <br>
* Roles can be assigned to any EC2 instance after it is created using both  the console and commandline. <br>
* Roles are universal - Can be used in any region. <br>

<br>

**Boot Strap Scripts** <br>
Way of automating EC2 instances deployments. All commandline commands can be write in Scripts. An example script is shown below that can be write under 'Configure instances' at the time of creating an EC2 instance. <br>

It always begin with (path of interpreter) - #!/bin/bash
<br>

## Example Script ## <br>
yum update -y <br>
yum install httpd -y <br>
service httpd start <br>
chkconfig httpd on  <br>
cd /var/www/html <br>
echo"<html><h1>Welcome</h1></html>" > index.html <br>
aws s3 mb s3://jdjgf6474 <br>
aws s3 cp index.html s3://jdjgf6474 <br>

