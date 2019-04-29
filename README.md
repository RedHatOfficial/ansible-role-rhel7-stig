# DISA STIG for Red Hat Enterprise Linux 7

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-stig.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-stig)
[![Ansible Role](https://img.shields.io/ansible/role/39712.svg)](https://galaxy.ansible.com/RedHatOfficial/rhel7_stig)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-role-rhel7-stig.svg)](https://github.com/RedHatOfficial/ansible-role-rhel7-stig/releases/latest)

Ansible Role for DISA STIG for Red Hat Enterprise Linux 7  

Profile Description:  
This profile contains configuration checks that align to the   
  DISA STIG for Red Hat Enterprise Linux V1R4.   
    
  In addition to being applicable to RHEL7, DISA recognizes this   
  configuration baseline as applicable to the operating system tier of   
  Red Hat technologies that are based off RHEL7, such as:   
  - Red Hat Enterprise Linux Server   
  - Red Hat Enterprise Linux Workstation and Desktop   
  - Red Hat Enterprise Linux for HPC   
  - Red Hat Storage  
  
The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

## Requirements

- Ansible version 2.5 or higher

## Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

## Dependencies

N/A

## Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel7_stig` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel7_stig }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

## License

BSD-3-Clause

## Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
