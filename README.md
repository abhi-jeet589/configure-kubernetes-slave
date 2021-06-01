configure-kubernetes-slave
=========

Kubernetes Slave Configuration Role will help you to configure kubernetes slave that is deployed on any public cloud or local server. For this you are required to just supply the inventory file to the ansible playbook provided with this role.

Requirements
------------

The pre-requisites for this role is that the user must already have an inventory file configured. If the remote system has a private key file required to log into the system, the user must provide the ssh private key file. To know more about such keywords head over to ansible documentation.

Role Variables
--------------

There are no Role variables that need to be specified.

Dependencies
------------

This Role works in tandem with another role namely, Kubernetes-Master-configuration(to configure Master(s)) and Provisioning-Kubernetes-over-AWS(to provision EC2 instances on AWS that are to be configured as the cluster).

Example Playbook
----------------

 - name: "Configure Kuberentes Slaves"
   hosts: slaves
   roles:
   - kubernetes-slave-configuration

Author Information
------------------

You can contact me @ abhijeetkarmakar23@gmail.com
