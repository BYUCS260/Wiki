# Wiki
How to set up Git for your Web Programming projects (and everything else)

Download git for your OS. It should be installed on most servers. On the koding.com nodes type
which git
If you dont see it in your path (/usr/bin/git) try
sudo yum install git.x86_64
Tell Git your name so your commits will be properly labeled.
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR EMAIL"
Create an account at github.com.
Go to your github.com tab in your web browser, login to your git account, click on the repositories button and the green "New" button to create a new repository. The following page will show you how to set up your project from the command line.
Enter the following commands to set up the project
git init
git add .
git commit -m 'First Commit'
git remote add origin https://github.com/yourUserName/projectname.git
git push -u origin master
Now you should be able to see your project files in the github.com browser window.
If you change something in the github.com version, you can update the copy on your ec2 web server with "git pull".
You may want to use a gui editor like sublime 2 on your laptop. Then push the updates to github and pull them down on your server.
