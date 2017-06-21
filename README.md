ansible-xnat
============

Deploys an instance of [XNAT](http://www.xnat.org) 1.7.1 

XNAT is an open source imaging informatics platform, developed by the Neuroinformatics Research Group at Washington University. It facilitates common management, productivity, and quality assurance tasks for imaging and associated data. Thanks to its extensibility, XNAT can be used to support a wide range of imaging-based projects.

Quickstart
----------

Install Ansible

    pip install ansible

If you use [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](http://www.vagrantup.com/downloads.html), just run the following command within the root of this repo:

	vagrant up

If you want to deploy on bare metal:

    ansible-playbook site.yml 192.168.0.1,


License
-------

GPLv3

Author Information
------------------

Roman Valls Guimera
Gregor Lenz