# Bandito 
Bandito is monitoring system that utilises Nagios to monitor the TOR network in its entirety.   

## Getting Started

You need to be somewhat conversant with Ansible, Tor, Nagios and Linux.

Have a vanilla CentOS7/RHEL7 system at your disposal.

[You will also need a TOR Relay configured and have it be connectable via STEM.](https://stem.torproject.org/tutorials/the_little_relay_that_could.html)

### Prerequisites

Have a vanilla CentOS7/RHEL7 system ready, preferably a minimal install, and with Ansible installed.

Install ansible as per the following:

```
yum install ansible -y
```

### Installing

1. Clone this repo

2. There are variable definitions required prior to install:

See the following file

```
vars/main.yml
```

3. To build the system, run the following:

```
ansible-playbook site_bandito.yml
```

4. Upon building, using the http_access credentials you defined in vars/main.yml, navigate a web browswer to:

```
http[s]://<server_name>>/bandito
```

## Deployment

Upon building, using the http_access credentials you defined in vars/main.yml, open a web browswer to 

```
http[s]://<server_name>>/bandito
```

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors
* **Nocturnal** - *Initial work* - [nocturnal-or](https://github.com/nocturnal-or)

**Nocturnal** is available for consultation, and resides in Canberra, Australia. Please contact via github. 

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* The TOR Project. Please consider making a donation: https://donate.torproject.org/
