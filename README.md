# Criminal Justice Information Services (CJIS) Security Policy

[![Build Status](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-cjis.svg?branch=master)](https://travis-ci.org/RedHatOfficial/ansible-role-rhel7-cjis)
[![Ansible Role](https://img.shields.io/ansible/role/39706.svg)](https://galaxy.ansible.com/RedHatOfficial/rhel7_cjis)
[![GitHub release](https://img.shields.io/github/release/RedHatOfficial/ansible-role-rhel7-cjis.svg)](https://github.com/RedHatOfficial/ansible-role-rhel7-cjis/releases/latest)

Ansible Role for Criminal Justice Information Services (CJIS) Security Policy

Profile Description:
This profile is derived from FBI's CJIS v5.4
Security Policy. A copy of this policy can be found at the CJIS Security
Policy Resource Center:

https://www.fbi.gov/services/cjis/cjis-security-policy-resource-center

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

# Requirements

- Ansible version 2.5 or higher

# Role Variables

To customize the role to your liking, check out the [list of variables](vars/main.yml).

# Dependencies

N/A

# Example Playbook

Run `ansible-galaxy install RedHatOfficial.rhel7_cjis` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel7_cjis }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

# License

BSD-3-Clause

# Author Information

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
