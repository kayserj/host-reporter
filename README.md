# Host Reporter

The Host Reporter is a collective of ansible tasks that will ping, tcp scan, detect operating systems, discover path mtu, and run traceroutes with geolocation, against a network or host.

## Summary
This tool utilizes nmap, and will execute nmap scan commands based on the questions asked.  Some of the functions of host-reporter are:

Run against a network host or subnet
Ping sweeps
TCP port scans
Detect host operating systems, report system uptime, and network distance
Path MTU discovery
Traceroute with geolocation discovery
Generate HTML reports from results
Display results in terminal window

Run dependency checks against the local machine to ensure all the proper packages are installed, and install them if not.  


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.


### Prerequisites

Must have ansible installed and configured using python3.
Mac users must have ansible installed using python3, and homebrew installed.

How to install Homebrew https://brew.sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"


### How to install

Copy the host-reporter folder to your machine.


### Execution

From within the host-reporter folder, issue the following command. Most of the tasks require sudo privileges. 

```
ansible-playbook host-reporter.yml --ask-become-pass
```


### Details

Running the playbook will create a single .html file in your user’s home directory.  After the play completes, check your home directory for the file. The users home directory is referenced with `~/`


* [Ansible](https://www.ansible.com/)

* [Nmap](https://nmap.org)

### Authors

* **James Kayser** - *Initial work* - [kayserj](https://github.com/kayserj)

### License

@ 2020 James Kayser All Rights Reserved


