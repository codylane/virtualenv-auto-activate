# virtualenv-auto-activate
A nice little utility that auto activates a virtualenv environment when you cd into a directory

# Recognition and Credit
Example was modifed from the following link:
https://www.burgundywall.com/

All credit should be given to the following person for coming up with this example:
`Kurt Neufeld`

# Installation
Clone the repository
```
git clone https://github.com/codylane/virtualenv-auto-activate.git $HOME/
```

Add this to the end of your ~/.bashrc
```
source $HOME/virtualenv-auto-activate/auto_activate_virtualenv
```

# Add .venv to your project directory.  Here is an example
The example assumes you have a virtual environment created name `python-libvirt`
```
cd ~/prj/my-python/project
echo "python-libvirt" > .venv
```
Next you will need to cd back one directory and then cd into your main project directory.  This will automatically activate the virtualenv environment.  
```
cd ..
cd project
```

You should see something like this, which means the virtualenv is activated.  Now, when you cd to a different directory, outside of the project root, the virtualenv will automatically be deactivated.  
```
(python-libvirt)
$ 
```

