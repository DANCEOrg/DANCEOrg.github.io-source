# Website Setup Documentation
## Overview

1. Installing Jeykll

2. Initializing the Source Repository

3. Building the Website Repository

4. Working with INDICO Space

5. Launching Site with GH-Pages

## 1. Installing Jeykll

*Note: In this tutorial, sudo apt was used rather than other utilities such as cat. This turorial was performed on Ubuntu 18.04 and 20.04*

Jekyll is a static site generator that is used for the iris-hep website; this is the website which DANCEOrg is modeling after. 

The Jekyll [website](https://jekyllrb.com/) is an excellent resource for the installation process. Most of the commands used are from the site. 

### Pre-Reqs

Before installing Jekyll, there is a critacal prerequisite called Ruby. 

Run command: `ruby -v` to see if ruby is already installed

If not installed here are the separate instructions for LTS 18.04 and 20.04. Both will install Ruby using Rbenv

#### For LTS 18.04:

Optional: sync your WSL clock with: `sudo hwclock -s`

First, update the `apt-get` utility with: `sudo apt-get update`

Install system dependencies: `sudo apt-get install openssl libssl-dev zlib1g zlib1g-dev`

*The following instructions are from the techiediaries [website](https://www.techiediaries.com/install-ruby-2-7-rails-6-ubuntu-20-04/):*
  
```
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
rbenv install 2.7.2
rbenv global 2.7.2
```
After cloning the rbenv installations, close and restart your shell. 

Run command: `ruby -v` and it will return 2.7.2

#### For LTS 20.04:
*Instructions for installation on 20.04 are from the [linuxize](https://linuxize.com/post/how-to-install-ruby-on-ubuntu-20-04/) website*

First, update the `apt-get` utility with: `sudo apt-get update`

Install required libraries and compilers:

```
sudo apt install git curl autoconf bison build-essential \
    libssl-dev libyaml-dev libreadline6-dev zlib1g-dev \
    libncurses5-dev libffi-dev libgdbm6 libgdbm-dev libdb-dev
```

Install the rbenv tool using `curl`:`curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-installer | bash`

To start using rbenv, add `$HOME/.rbenv/bin` to your `PATH` with Bash or Zsh: 

For Bash:

```
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
source ~/.bashrc
```

For Zsh:

```
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc
source ~/.zshrc
```

Run: `rbenv -v` to confirm and it should return: `rbenv 1.1.2-30-gc879cb0` 

Now, install 2.7.1: 

```
rbenv install 2.7.1
rbenv global 2.7.1
```
Run command: `ruby -v` and it will return 2.7.2


#### Bundler Install 
Now bundler can be install with: 

```
gem install bundler
rbenv rehash
```

### How to get Jekyll

Now that `gem install bundler` is installed, it can be used to install jekyll with: `gem install bundler jekyll`

Once complete, confirm with: `jekyll -v` and it should return: `jekyll 4.2.0`

## 2. Initializing the Source Repository


## 3. Building the Website Repository

### Running the Website locally



