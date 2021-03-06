﻿# Welcome to items catalog app -V1 - The linux system project!

a customized linux server for a secured system to have our items catalog app

# Linux server information:
#### IP :  *18.197.82.52*
#### The host app url: *http://18.197.82.52.xip.io/*
### Software installed  : 
All the installed packages are included in the requirements.txt file .
### Configuration :
Configuration changes included :
- enforcing ssh authentication on the remote server.
- disabling the default **22** ssh port and enabling **2200** for ssh
- configuring ufw to allow http on **80** /ssh on **2200**/ntp on **123** connections 
- disabling any remote connections to the database for security concerns

### Third-party resources used:
the third-party resources included **Amazon's Lightsail Instance** and the **xip.io** to access the application
### location of ssh key for grader user is : 
*~/.ssh/authorized_keys*
### Grader user's SSH key is included into the "Notes to Reviewer" field
### Github repository : https://github.com/Ducky93/catalog

## Project description :
this project is a web app providing the service of managing different catalogs with their contained items .

## Dependencies/Pre-requisites:
the app can be run on a vagrant machine attached within the compressed folder .
if you won't be using the vagrant machine then should have python 2 or 3 installed on your machine .
and the user is required to have a google account because we won't allow the application to accept any other registration method .. yes we are sponsored by google :) .
## Setup/Installation
to setup the project you will need to unzip the folder provided,then on command line use the following commands : 
`vagrant up`
then
`vagrant ssh`
once you are logged in the vagrant machine use : 
`cd/vagrant`
then
`python main.py`
the application should be running now on localhost port 5000

## Usage
it's pretty straight forward how to use the app , you can view the currently added categories or items by clicking on the link on their names , that will take you to the page relevant to the item/category you have clicked on..
but you won't be able to edit/add/delete any items or categories unless you are logged in using your own google account .

### API
to use our api here are the end points to use to get the same information provided through the application : 
 - /api/          getting all  the categories in our database
 - /api/catalog/          getting all  the categories in our database
 - /api/catalog/category name/item name/ get a certain item in a catalog
 - /api/catalog/category name/items/ get all the items available in a
   category 

hope you do enjoy the app, wait for version 2 released on 26/6/2099 :)!



