Intro
======
This is the starting point for a session held at [DevOpsCon Berlin 2016](http://devopsconference.de).

* [Abstract](http://devopsconference.de/session/zero-downtime-deployment-with-ansible/)
* [Tutorial slides](http://steinim.github.io/slides/devopscon/zero-downtime-ansible)

Install Ansible
=============

Mac:
----
Install Python setuptools: https://pypi.python.org/pypi/setuptools#installation-instructions

If you prefer not to install packages to your global `site-packages` you can install and use virtualenv: http://virtualenv.readthedocs.org/en/latest/

```sudo easy_install pip```

```sudo pip install paramiko PyYAML jinja2 passlib```

```sudo pip install ansible```

Then, if you're going to update ansible later, just do:

```sudo pip install ansible --upgrade```

Other:
------
http://www.ansibleworks.com/docs/intro_installation.html

Install VirtualBox and Extension Pack
======================================
https://www.virtualbox.org/wiki/Downloads

Install Vagrant
===============
http://docs.vagrantup.com/v2/installation/

Install [vagrant-cachier plugin](https://github.com/fgrehm/vagrant-cachier) to speed up apt with a shared cache between boxes:

```vagrant plugin install vagrant-cachier```

Install [vagrant-hostmanager plugin](https://github.com/smdahlen/vagrant-hostmanager) to manage the /etc/hosts file on guest machines and the host:

```vagrant plugin install vagrant-hostmanager```

Clone this repo, and start the virtual machines:

```
git clone https://github.com/steinim/devopscon-zero-downtime-ansible.git
cd devopscon-zero-downtime-ansible
vagrant up
```

Provision with Ansible
=======================
```ansible-playbook site.yml```

Install Java and Maven (Optional)
======================
http://www.oracle.com/technetwork/articles/javase/index-jsp-138363.html

http://maven.apache.org/download.cgi

Build the Java app
------------------
```cd helloworld-java-app```

```mvn clean install```

Getting started
----------------
http://www.ansibleworks.com/docs/intro_getting_started.html

Ansible Modules
----------------
http://www.ansibleworks.com/docs/modules.html

