## Linux already comes with python 2.7 installed, and in this tutorial we will update it to version 3.5.0, it is easy you just need to follow this steps:

# Check python version on Terminal ( Ctrl + Alt + T open terminal)
python -V

#Installing the pyenv
curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash

#Install dependencies before pyenv
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev git

# Add to ~/.bashrc at the end of file
export PATH="~/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

#Test with the command(you may need to restart terminal):
pyenv versions
* 3.5.0 (set by /home/{user}/.pyenv/version)

# Install python on pyenv
pyenv install 2.7.17

# Check if version 3.5.0 is selected with the command
pyenv versions

# Test the python version with:
python -V

pyenv install 2.7.17
# error: python-build: TMPDIR=/tmp cannot hold executables (partition possibly mounted with `noexec`)  solution: sudo mount -o remount,exec /tmp

#Set Python2.7.17 as global pyenv
pyenv global 2.7.17

pyenv virtualenv 2.7.16 example-2.7.16 


# python -dev 
sudo apt-get install python-dev

# create directory
mkdir example

# local env
pyenv local example-2.7.17

# Install Git
sudo apt install git-all

# Create ssh keys in the server
ssh-keygen -b 2048 -t rsa

# added .pub key into gitlab account

# pull code
git pull origin master

# Install python 2
sudo apt install python2

# install pip
curl https://bootstrap.pypa.io/pip/2.7/get-pip.py --output get-pip.py
sudo python2 get-pip.py
pip --version


