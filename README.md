These are the accompanying files from my PHPNW13 presentation on Vagrant and Ansible.

# Installation

Download and install Virtualbox + Vagrant

* https://www.virtualbox.org/wiki/Downloads
* http://downloads.vagrantup.com/

# Running things

Clone this repo and run `vagrant up` and wait. It'll take a while on the first run whilst it downloads the base image.

```bash
git clone https://github.com/mheap/phpnw-ansible-playbooks.git
cd phpnw-ansible-playbooks
vagrant up
```

Then, you can run either the playbook from the live demo:

```bash
ansible-playbook -i host.ini live-demo/bootstrap.yml
```

Or, you can run the role based playbook I put together

```
ansible-playbook -i host.ini well-formed/site.yml
```

If you have any issues, feel free to open an issue, or ping me on twitter (@mheap)
