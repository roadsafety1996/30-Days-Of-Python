

## Setting up Virtual Environments

To start with project, it would be better to have a virtual environment. Virtual environment can help us to create an isolated or separate environment. This will help us to avoid conflicts in dependencies across projects. If you write pip freeze on your terminal you will see all the installed packages on your computer. If we use virtualenv, we will access only packages which are specific for that project. Open your terminal and install virtualenv

```sh
 pip install virtualenv
```

Inside the Python folder create a flask_project folder.

After installing the virtualenv package go to your project folder and create a virtual env by writing:

For Mac/Linux:
```sh
Desktop/Python/flask_project\$ virtualenv venv

```

For Windows:
```sh
C:\Users\User\Documents\Python\flask_project>python -m venv venv
```

I prefer to call the new project venv, but feel free to name it differently. Let us check if the the venv was created by using ls (or dir for windows command prompt) command.

```sh
Desktop/Python/flask_project$ ls
venv/
```

Let us activate the virtual environment by writing the following command at our project folder.

For Mac/Linux:
```sh
:~/Desktop/Python/flask_project$ source venv/bin/activate
```
Activation of the virtual environment in Windows may very on Windows Power shell and git bash. 
