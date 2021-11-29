# App in a Box - Todo 

This is a simple todo application written in containers that uses a MySQL 
backend along with Redis Caching to drive a API and a frontend that powers
a simple little Todo application.  It also spins up Google Cloud infrastructure
to power the application. 

![ToDo architecture](architecture.png)

## Install
You can install this application using the `Open in Google Cloud Shell` button 
below. 

<a
        href="https://ssh.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https%3A%2F%2Fgithub.com%2FGoogleCloudPlatform%2Fappinabox_yesornosite&cloudshell_print=install.txt&cloudshell_open_in_editor=README.md">
        <img alt="Open in Cloud Shell" src="https://gstatic.com/cloudssh/images/open-btn.svg"></a>

Once this opens up, you can install by: 
1. Creating a Google Cloud Project
1. Then typing `./install`

## Cleanup 
To remove all billing components from the project
1. Typing `./uninstall`

## Developement
There is a development setup for this application that uses Docker to run 
everything you need to developer and test it out locally. 

To run:
1. Open a terminal on your local system. 
1. `cd code`
1. `make dev`

This will spin up 4 containers
1. MySQL /database
1. Redis
1. Golang API /middleware
1. Static HTML/JS/CSS site /frontend


This is not an official Google product.