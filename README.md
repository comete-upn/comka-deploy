# Comka - Deploy Karuta local test environment

Deploy Karuta test environment using Vagrant and Ansible. Karuta is installed on Tomcat 7 and MariaDB. To ease the testing process [Frontail](https://github.com/mthenw/frontail) is installed to view Tomcat and Karuta logs in the browser.

# Requirements

- Vagrant 2.0 or greater
- Ansible 2.5 or greater

# Installation

Copy *config.sample.yml* to *config.yml* and edit it to suit your needs. Review *Vagrantfile* if you want to change port forwarding for Karuta and Frontail and start Vagrant environment :

```bash
vagrant up
```

Tested on :

 - Ubuntu 18.04
 - Vagrant 2.0.2
 - Virtualbox 5.2.32
 - Ansible 2.5.1

# Usage

Start the environment :

```bash
vagrant up
```

Visit: 

 - http://localhost:8080/karuta
 - http://localhost:9001

Default root login for Karuta is *root* with password *mati*.

# Credits

 - Université Paris Nanterre - Comete

# License

GNU General Public License v3.0 or later