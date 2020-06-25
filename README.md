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

# Steps to get working

 

### Prerequisites

 

- Download Ruby

 

```bash
gem install bundler
```
<!-- installs bundler -->

 

```bash
bundle install
```
<!-- installs ruby dependencies -->

 

### Activating Virtual Machine

 

1. git clone repo
<!-- to take all the code & the initialized vagrant -->

 

2. in root of repo run

 

```bash
vagrant up
```
<!-- to start up vagrant  -->

 

3. That's it!



