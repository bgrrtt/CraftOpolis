<!-- ![Craft-Ops Logo](https://raw.githubusercontent.com/bgrrtt/craft-ops/master/logo.jpg "DevOps Environment for Craft CMS and AWS") -->
Craft-Ops
=========

**DevOps Environment for [Craft CMS](http://craftcms.com) and [AWS](http://aws.amazon.com).**

Built with [Ansible](http://ansible.com). Made by [MIZZEN](http://madebymizzen.com).

Installation
---
Clone the repo, get into the project's folder, and start up the virtual dev environment.
```
git clone https://github.com/bgrrtt/craft-ops.git your_project_name
```
```
cd your_project_name
```
```
vagrant up
```
### Prerequisites
The host computer, only tested for macOS 10.11+, must have [Vagrant](vagrant_link) and [VirtualBox](virtualbox_link) installed. If you aren't familiar with [brew.sh](brew_link), check out my article on [dotfiles](dotfiles_article_link).

```
brew cask install virtualbox vagrant
```

#### Optional (sorta)
These vagrant plugins come in *very* handy, *so* handy that the rest of the instructions assume you have them installed.
- [vagrant-cachier](https://github.com/fgrehm/vagrant-cachier)
- [vagrant-hostsupdater](https://github.com/cogitatio/vagrant-hostsupdater)
- [vagrant-vbguest](https://github.com/dotless-de/vagrant-vbguest)


### Virtualbox Configuration
In the `Vagrantfile`, change the following variables on line `4` and `5` to fit your development environment needs:
- PROJECT_NAME (project) (dev site will be available at `http://project.dev` by default)
- LOCAL_IP (192.168.0.0 - 192.168.255.255) (dev site will be available at `192.168.0.1` by default)


---


[Visit the wiki for more instructions!](https://github.com/bgrrtt/craft-ops/wiki)
========================

Thanks to [@howardroark](https://github.com/howardroark), [@geerlingguy](https://github.com/geerlingguy), [@khalwat](https://github.com/khalwat), and [@pixelandtonic](https://github.com/pixelandtonic).
