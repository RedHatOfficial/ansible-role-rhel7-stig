## Amazon Linux 2 Ansible Hardening

This Ansible role will harden an Amazon Linux 2 (AL2) system based on the hardening instructions in the Defense Information Systems Agency (DISA)'s Security Technical Implementation Guide (STIG) for Red Hat Enterprise Linux 7, off of which the AL2 OS is based.

## Getting Started

This Ansible role provides a straightforward way to apply security hardening configurations to your Amazon Linux 2 instances. To get started, follow these steps:

1. Clone this repository to your local machine.

```
   git clone https://github.com/mitre/amazon-linux-2-ansible-hardening.git
```

Make sure you have Ansible installed on your local system. If you haven't already installed Ansible, you can do so by following the instructions on the Ansible website.

2. Create an Ansible playbook that includes this role. For example, you can create a playbook like harden-al2.yml:

```
---
- name: Harden Amazon Linux 2
  hosts: your_target_hosts
  roles:
    - amazon-linux-2-ansible-hardening
```

3. Run Ansible playbook to apply the hardening configurations:
```
ansible-playbook harden-al2.yml
```

4. Monitor the playbook's execution for any errors or warnings.

5. After the playbook completes, your Amazon Linux 2 instance should be more secure, following the DISA STIG recommendations.

## Requirements

- [Ansible](https://ansible.com)

## License

This project is licensed under the Apache License 2.0. For more details, please see the [LICENSE](./LICENSE.md) file.

## Author Information

This project is a collaborative effort between multiple contributors from MITRE and the open-source community (VMware).
If you encounter any issues or have suggestions for improvements, please open an issue on the GitHub repository.
