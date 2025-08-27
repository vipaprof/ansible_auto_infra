# Ansible Project

### The purpose:

This Project for me was an Introduction to Ansible.
The need for automation and tools of automation continue to grow.
Learning the basics of Ansible has given me a better understanding of the word Idempotent and I now have become a little bit better at managing systems using ansible.

#### The setup:

* Operating Systems - Ubuntu, Debian, Centos
* Ubuntu - Ansible server, Reverse proxy
* Debian - Two web servers
* Centos - Database server, Samba share

##### How To:

* This is the playlist to get started if you don't know anything  [youtube](https://youtube.com/playlist?list=PLT98CRl2KxKEUHie1m24-wkyHpEsa4Y70&si=P5GuVW3LrOXk3KQx)

* First run bootstrap.yml with your ssh public key(without passphrase) in the `key:` line
* If you didn't understand this. Please watch the series.
* After bootstrap you do not need `--ask-become-pass`
* Uncomment two lines of `ansible.cfg` leave last one as a comment for now
* Run `main.yml`
* Uncomment last line of `ansible.cfg`
* Disconnect and connect with changed ssh port 
* Uncomment every `role`
* Run `main.yml` with `--ask-vault-pass`
* Changing file paths, host_vars and passwords.yml.j2 has been left up to you 
 
##### Shortcomings:

* As you can already see running playbooks multiple times is not good for automation.
* The playbooks and taskbooks can always be better refactored for future ease of use
* Changing ssh ports in playbooks require disconnect


> Overall This project on Ansible was a great learning experience and I will be sure to write better playbooks in coming Future.

`DRY - Dont Repeat Yourself` If you are going to do it something more than once just automate it, you can use Ansible.
