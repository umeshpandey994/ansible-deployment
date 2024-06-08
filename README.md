# Deployment

### Install python and ansible to setup deployment in local system
pip install ansible==2.9.1 && python version = 2.7.17 

### RUN ANSIBLE COMMAND AND PASS HOST OPTION USING -l
ansible-playbook --private-key <path of private file> -l <inventory host name> site.yml --tags git-clones -e branch_name=<your branch name>

### Deploy git branch and run django command migrate, collect-static, npm install, npm run build and restart services
ansible-playbook --private-key ./key.pem -l example-stage site.yml --tags "git-clones, run_django_command" -e branch_name=<branch name>                                                        

### Supervisord: Restarting and Reloading 
https://www.onurguzel.com/supervisord-restarting-and-reloading/

### Install pyenv in local system
https://akrabat.com/creating-virtual-environments-with-pyenv/

### Create a new python virtualenv
pyenv install <python version>
pyenv virtualenv <python version> <pyenv name with python version>
pyenv local <pyenv name with python version>

### check python path for any project
pip --version

### Git commit message guideline must read 
https://chris.beams.io/posts/git-commit/
