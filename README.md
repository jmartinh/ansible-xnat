ansible-xnat
============

Deploys an instance of [XNAT](http://www.xnat.org) and applies the dHCP customisations to it.

XNAT is an open source imaging informatics platform, developed by the Neuroinformatics Research Group at Washington University. It facilitates common management, productivity, and quality assurance tasks for imaging and associated data. Thanks to its extensibility, XNAT can be used to support a wide range of imaging-based projects.

Quickstart
----------

Download the version of XNAT you want to install from [here](https://bitbucket.org/xnatdev/xnat-web/downloads/) or build it from the sources.

You should place the downloaded/generated war in this repository's top folder, next to the `site.yml` playbook. Naming should follow the following convention:

  xnat-web-{{ xnat-version }}.war


Install Ansible

  pip install ansible

If you use [VirtualBox](https://www.virtualbox.org/wiki/Downloads) and [Vagrant](http://www.vagrantup.com/downloads.html), just run the following command within the root of this repo:

	vagrant up

If you want to deploy on bare metal

    ansible-playbook site.yml 192.168.0.1,

After the playbook finishes, access under this URL:

	http://localhost:8080


for a Vagrant based setup, or replace with the corresponding URL/IP for a bare metal setup.

License
-------

GPLv3

Author Information
------------------

Roman Valls Guimera

Gregor Lenz
