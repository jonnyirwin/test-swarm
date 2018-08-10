# Test Swarm #

An empty 3-node (though can be atered in the Vagrantfile to add more nodes) Docker Swarm.  Used for trialling Docker Swarm and for following along with the excellent [Udemy Docker Mastery](https://www.udemy.com/share/1001eQBksceF1W/) course.

## Pre-requisites ##

You need to have the following installed:

* [Ansible](https://www.ansible.com/)
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)

## Usage ##

Clone this repository.  In the folder the repository is cloned into (assuming the above dependencies are installed), type:

'''
vagrant up
'''

When this task completes, a 3-node docker swarm should be up and running (with 1 manager and 2 worker nodes).

To access the manager node, type:

'''
vagrant ssh manager
'''

And to access the 2 worker nodes type:

'''
vagrant ssh worker-1
'''

or

'''
vagrant ssh worker-2
'''

As this is designed for testing purposes only, docker commands can be ran without `sudo`.
