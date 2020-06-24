# Vagrant provision Class

Today's learning objectives:

- provisioning
- setting up a working app

## Sudo code of what we want to do:

# Question you might ask
Someone from the team is hadding you code. Don't just accpet, ask for context. Examples:

- what language
- what frameworks?
- are there tests?
- is a specific package that need to be installed? is the a package list of some sort?
- specific versions?
- specific packages or versions that don't work?
- any other info?

## response you got today!
- amazing thank you for asking! Well we have a good readme.

- it's all built on js node (ohhh okay look out for this terminology)

- and there are some test you can run from the host machine.
just bundle install and run the rake file! (smile)

- I want to create machine and set up a work app in it. I want it in a VM because it will be a standardize environment.

What steps do I need to take?

## Well I know the enviroment will be:

- ubuntu/xenial64 (done)

- I will need nodejs
check how to install stuff in it (the dependencies)

- I want it on port 80

- I will need a reverse proxy to get my app talking on port 80

- I will need my app in my vm! (right?) so I can install and run it's code

# Steps to get working 

- Download ruby 

Then I can install bundle.

- In project folder file (this file) open bash

- Then type in 
```bash
 gem install bundler
```
- Now start up VM (make sure the provisions have ran)

- Go to "environment\spec-tests" (using bash), and type in : 
```bash
rake spec
```
- Installing nodejs, this will be in provision https://www.techiediaries.com/ubuntu/install-nodejs-npm-on-ubuntu-20-04/

```
curl -sL https://deb.nodesource.com/setup_11.x | sudo -E bash -
sudo apt install curl
sudo apt-get install -y nodejs
```
- The last test is to install pm2, in provision

```
npm install -g pm2
```
# How to sync folders 

```
config.vm.synced_folder "folder_path_to_origin_folder", "path_in_main"
```




