# Bandito 
Bandito is monitoring system that utilises Nagios to monitor the TOR network in its entirety.   

## Getting Started

You need to be conversant with Ansible, Tor (running a relay), Nagios and CentOS7 Linux.

### Prerequisites

* Have a vanilla CentOS7 system at your disposal (with ansible installed), e.g.

```
yum install ansible -y
```

* [You will also need a TOR Relay configured and have it be connectable via STEM.](https://stem.torproject.org/tutorials/the_little_relay_that_could.html)

### Installing

1. Clone this repo

```
git clone https://github.com/nocturnal-or/Bandito.git
```

2. Setup the appropriate variable definitions prior to building:

See the following (well documented) file:

```
vars/main.yml
```

3. To build the system, run the following:

```
ansible-playbook site_bandito.yml
```

## Deployment

Upon installing, using the http_access credentials you defined in vars/main.yml, open a web browswer to 

```
http[s]://<server_name>>/bandito
```

It's probably not a good idea to run this on the open internet without additional security controls in place. 

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors
* **Nocturnal** - *Initial work* - [nocturnal-or](https://github.com/nocturnal-or)

**Nocturnal** is available for consultation, and resides in Canberra, Australia. Please make contact via Github (GPG public key available on profile). 

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* The TOR Project. Please consider making a donation: https://donate.torproject.org/
