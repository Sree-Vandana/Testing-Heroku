# Testing-Heroku

The Main goal of this is to test and learn <b>how deploy my existing web page using Heroku.</b></br>
</br>
The "09-bootstrap-form.html" and "09-bootstrap-form.css" are files from my (Fullstack-webdev-HW folder)<!--[https://github.com/Sree-Vandana/Fullstack-webdev-HW/tree/master/hw1]--> (which is private Repo for now)</br>
I am using visual studio code for all my Fullstack-web-development Projects. All this is done using Terminal in Visual Studio Code.</br> 
</br>
<b>I followed the following steps:</b></br>
</br>
<b>STEP 1:</b> Created a Heroku Account; create a New Project (my project name is "test-heroku-bootstrap-form") and Installed Heroku CLI (these steps and links are clearlly mentioned in the Heroku account i created, under <i>apps/test-heroku-bootstrap-form/deploy</i>)</br>
<b>STEP 2:</b> In visual studio code Terminal enter "heroku login" it will redirect to its website where you can click 'Login' and you will be logged-in, in your visual studio terminal.</br>
<b>STEP 3:</b> After logging-in, enter "heroku git:clone -a test-heroku-bootstrap-form" this command in the terminal (can find these command in your Heroku account under <i>apps/test-heroku-bootstrap-form/deploy</i> )</br>
This command will set our project repository as a remote repository that Heroku has, in its services. </br>
<b>STEP 4:</b> Commit your code to the repository and deploy it to Heroku using Git, using these commands.</br>
$ git add .</br>
$ git commit -am "make it better"</br>
$ git push heroku master</br></br>
<b>NOTE:</b><i> when entered "git push heroku master" i got Built Failure Errors. This is because Heroku could not find BuiltPack to support my HTML and CSS files. while creating account i set my language prefference as "Node". So, i changed my Built-Pack to php using <b>"set heroku/php"</b> in my visual studio terminal and added a index.php file in my repo which contains only one statement <b>" \<?php header ( 'Location: /09-bootstrap-form.html' ); ?\> "</b> (without quotes). then repeated STEP 4 commands and it pushed successfully.</i></br>
</br>
In my Heroku account, under "/apps/test-heroku-bootstrap-form" when clicked "Open app" I got my Bootstrap-Form deployed.</br>
<b>This is the link:</b> https://test-heroku-bootstrap-form.herokuapp.com/09-bootstrap-form.html
