---
layout: page
root: ..
title: Get ShowYourWorking
---

This page shows how to download and run ShowYourWorking - getting the user to the point where they can start using the "How To Use" documentation in [Use](../user/index.html)

## Downloading and running ShowYourWorking

You can have an installation of {{ site.software_name }} for your personal use up and running very quickly using these instructions.

## Installation

The {{ site.software_name }} platform consists of:

* A front end app (ng-chem) which is pulled in as a subrepository to this one.

* A set of python modules forming a set of web services.

Currently installation scripts are available and tested only for Ubuntu 14.04 and Anaconda python. A legacy install script for centos 6 is also available.

Follow these steps to install:

1) Clone the project to the desired folder, for this example I will use /srv/showyourworking and assume that you wish to install and run {{ site.software_name }} as your default ubuntu user

    cd /srv
    sudo mkdir showyourworking
    sudo chown -R $USER /srv/showyourworking 
    cd showyourworking
    git clone  --recursive  https://github.com/thesgc/chembiohub_ws.git .


2) Choose what url you would like ChemBio Hub to run on, in this case I choose localhost/showyourworking and include it as the first argument to the install script

3) Run the script to install all of the python dependencies 

    bash scripts/install_linux64.sh showyourworking Ubuntu


4) Run the command to setup the database and the index

    bash scripts/setup_database_and_index.sh showyourworking "$USER"


5) The showyourworking platform should now be available at localhost/showyourworking with the default username and password set up. (User = admin, Password = pass)

For more details on what has been installed see [Running the python server and database in production](https://github.com/thesgc/chembiohub_ws/wiki/Running-the-python-server-and-database-in-production).

## Getting Started Once Installed

Once you have got the system up and running, you will need to add more users and change your password.

This can be done via the standard django admin interface.

> Important: Every new user added must be given the "add project" permission via the django admin in order to see the add project functionality.

Currently, an invite user functionality is present in the top toolbar. 
Emails are sent and contain links to the standard reset password views.
This is not fully integrated with the "edit User Roles" function.

The default project types are the ones that are loaded during the "setupdatabase_and_index" script. In order to change these, use the django admin. Project types are meant to be the "base classes" from which users build the fields of their projects. This can be used to keep the number of field definitions manageable.

If you wish to set up a template for a project type to prepopulate the fields, find the custom field config id of the other project you want to attach to the project type and put that ID into the admin interface for the new project type.

In the skinningconfig admin it is possible to change some of the default configuration of the app as described below:

    File errors from backend    -> Whether the file upload message should be the backend exception or not
    Enable smiles input         -> Whether there should be a SMILES input box (if you are using your system for chemistry)
    Data manager email          -> Contact details for who to email if you have a problem with the system.
    Data manager name
