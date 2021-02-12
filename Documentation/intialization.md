# Website Setup Documentation
## Overview

1. Installing Jeykll

2. Initializing the Source Repository

3. Building the Website Repository

4. Working with INDICO Space

5. Launching Site with GH-Pages

## Installing Jeykll

### How to get Jekyll

Note: In this tutorial, sudo apt was used rather than other utilities such as cat. This turorial was performed on Ubuntu 18.04 and works for 20.04

Jekyll is a static site generator that is used for the iris-hep website; this is the website which DANCEOrg is modeling after. 

The Jekyll [website](https://jekyllrb.com/) is an excellent resource for the installation process. Most of the commands used are from the site. 

Before installing Jekyll, there is a critacal prerequisite called Ruby. 

Run command: `ruby -v` to see if ruby is already installed

If not installed run here are the instructions. 

Optional: sync your WSL clock with: `sudo hwclock -s`

First, update the `apt-get` utility with: `sudo apt-get update`

Install system dependencies: `sudo apt-get install openssl libssl-dev zlib1g zlib1g-dev`

The following instructions are from the techiediaries [website](https://www.techiediaries.com/install-ruby-2-7-rails-6-ubuntu-20-04/):
  
```
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
rbenv install 2.7.2
rbenv global 2.7.2
```
After cloning and the rbenv installations, close and restart your shell. 

Run command: `ruby -v` and it will return 2.7.2
