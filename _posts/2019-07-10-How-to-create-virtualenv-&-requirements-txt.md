---
layout: post
title: How to create virtualenv and requirements.txt for python projects
---

Creating a virtualenv for each project will simplify your life, avoiding version and package conflicts across multiple projects. When you are ready to publish, creating a requirements.txt allows other users to replicate your app or script output (you will thank yourself later). 

# How to install virtualenv for python projects:

### Install **pip** first

    sudo apt-get install python3-pip

### Then install **virtualenv** using pip3

    sudo pip3 install virtualenv 

### Now create a virtual environment 

    virtualenv venv 

>you can use any name instead of **venv**

### You can also use a Python interpreter of your choice

    virtualenv -p /usr/bin/python2.7 venv
  
### Active your virtual environment:    
    
    source venv/bin/activate
    
### Using fish shell:    
    
    source venv/bin/activate.fish

### To deactivate:

    deactivate

### Create virtualenv using Python3
    virtualenv -p python3 myenv

### Instead of using virtualenv you can use this command in Python3
    python3 -m venv myenv

# Once your project is ready to publish, let's create an requirements.txt:

### write the file
    pip freeze > requirements.txt
    
### show the file's contents
    cat requirements.txt
