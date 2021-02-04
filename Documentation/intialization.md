# Website Setup Documentation
## Overview

1. Installing Jeykll

2. Initializing the Source Repository

3. Building the Website Repository

4. Working with INDICO Space

5. Launching Site with GH-Pages

## Installing Jeykll

### How to get Jekyll

Note: In this tutorial, sudo apt was used rather than other utilities such as cat

Jekyll is a static site generator that is used for the iris-hep website; the website which DANCEOrg is modeling after. 

The Jekyll [website](https://jekyllrb.com/) is an excellent resource for the installation process. Most of the commands used are from the site. 

Before installing Jekyll, there is a critacal prerequisite called Ruby. 

Run command: `ruby -v` to see if ruby is already installed

If not installed run here are the instructions. 

Optional: sync your WSL clock with `sudo hwclock -s`

First, update the `apt-get` utility with: `sudo apt-get update`



