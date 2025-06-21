# Development of an ecommerce website for  "Marketpeak"

## Task 1.1
First i created a directory on my local machine named "Market_Ecommerce", I also initialised the git 
![Git-Directory](./Photos/directory-creation.PNG)

![Git-Init](./Photos/git-init.PNG)

## Task 1.2
 I was able to obtain an ecommerce website template on a website, well it's really not an ecommerce website template but almost.
 ![website-template](./Photos/ecommerce-website-template.PNG)

 ## Task 1.3
 I staged, commit the messages. I added the files from the templates downloaded. I set git global configuration
 ![Global-Config](./Photos/git-config.PNG)
 Commit message ![globa](./Photos/git-commit.PNG)

 
 
 I had no issues during the implementation of version control. Moving on the the AWS Deployment

 # AWS Deployment 
 I have an AWS account already so i just logged into it 
 
 ## Task 2.1 
 I logged in to my ec2 instance using Ubuntu 24.04, connected it using SSH
 ![ec-2](./Photos/Instance-lauch.PNG)

## Task 2.2
I cloned git into linux server for work effeciency, i used HTTPS to clone into it
![ec2-git-cloning](./Photos/ec2%20instance%20git%20cloning.PNG) 

## Task 2.3
I installed a web server using (sudo apt intall apache2). Tried using "sudo yum update -y" but won't go through because i didnt use Red-Hat based Linux, so i used ubuntu. Then i started the web server.
So i started my apache2 
![web-server](./Photos/web-server-starting.PNG) 
then i check the status of the Http server
![status](./Photos/web-server-status.PNG)

## Task 2.4
I configured the website to the Market_ecommerce file using "sudo rm -rf /var/www/html/*
sudo cp -r ~/MarketPeak_Ecommerce/* /var/www/html/" here is a picture of it but the problem was that i couldn't capture the part i used 
"sudo rm -rf /var/www/html/"

![web-configuration](./Photos/i-dont-know.PNG)

Then i reloaded my apache2 ![apache-reload](./Photos/reload-apache2.PNG)

## Task 2.5 
To access the webpage using my public address was successful 

![webpage](./Photos/webpage.PNG)

## Continous Intergration Workflowws
To  start continous integration workflow where i can fix bugs and add more features to my code so i introduced git branching, so i created development branch
![new-branch](./Photos/new-branch.PNG) then i switched to the branch

After the creation of a new branch i switched to the new branch then i added the new features i wanted to add then i staged and commit
![git-stage-&-commit](./Photos/new-features-staging-and-commiting.PNG)

After that i pushed to github for version tracking
![git-push](./Photos/development-pushrequest.PNG)

Then I checked out from development branch
![git-checkout](./Photos/git-checkout.PNG)


After the checking out from the development branch a pull request
![pull-request](./Photos/git-pull-origin-master.PNG)

then i merged the two branches together




