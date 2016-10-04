# dreamdjango
A shell script that automates the installation of Python 3 on a Dreamhost shared-hosting account and the subsequent installation of Django under a virtual environment.

# COMPATIBILITY

The script has currently only been tested for the following versions of Python and Django:
Python 3.5.2
Django 1.10.1 (installed via pip)

There is no reason why the script wouldn't work for other versions of Python and the corresponding versions of Django that are compatible (this can be achieve by selecting customer installation when prompted).


# DESCRIPTION


This script performs several tasks in the following order:

1. Instllation of the default version of Python, or one that is nominated by the user, to ~/opt/python-version
2. Setup of a virtual envrionment at ~/domain/venvs/projectname
3. Installaiton of Django under the virtual environment
4. Creation of the folders and files necessary for Passenger to recognise the project and function correctly


# PREREQUISITES AND INSTALLATION


To use this script, it is assumed that you have already set up a domain with Passenger enabled and that you have SSH access to the server hosting this domain.  Please consult the Dreamhost knowledge base (https://help.dreamhost.com) if you have not already done so.

PLEASE NOTE THAT THE SCRIPT REMOVES quickstart.html IN THE ~/domain/public FOLDER! MAKE SURE THAT A BACKUP COPY IS CREATED IF YOU WISH TO KEEP A COPY OF IT FOR ANY REASON.

Simply copy this script to any folder on the server, give it execute permission and run the script (source); then follow the prompt and let it do its thing! Once installation has finished, browser to the domain you have specified in during installation and you should be greeted by the Django welcome message.

