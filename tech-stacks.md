# Setting Up Languages and Frameworks

## JavaScript (Node.js, NVM, and NPM)
Run these commmands from your terminal.

- `sudo apt update`
- `sudo apt install nodejs npm`

Confirm installation with `node --version` and `npm --version`

## Databases (MongoDB and PostgreSQL)

The following instructions are adapted from [Microsoft's WSL Database Guide](https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-database). Bookmark that page to have a quick reference for establishing a quick connection to popular database systems.

## MongoDB

Update your Ubuntu packages: `sudo apt update`

Install MongoDB with this command: `sudo apt-get install mongodb`

Confirm installation and get the version number: `mongod --version`

After finishing the installation, run `which mongod` (yes, `mongod` with a d) to check that it's installed.

There are 3 commands you need to know once MongoDB is installed. Write these down somewhere safe when start using these DBs in class:

- `sudo service mongodb status` for checking the status of your database.`
- `sudo service mongodb start` to start running your database.`
- `sudo service mongodb stop` to stop running your database.`

## PostgreSQL

To install PostgreSQL on WSL (Ubuntu 18.04):

Update your Ubuntu packages: `sudo apt update`

Once the packages have updated, install PostgreSQL (and the -contrib package which has some helpful utilities) with: `sudo apt install postgresql postgresql-contrib`

Confirm installation and get the version number: psql --version

There are 3 commands you need to know once PostgreSQL is installed. Write these down somewhere safe when we start using these DBs in class:

- `sudo service postgresql status` for checking the status of your database.
- `sudo service postgresql start` to start running your database.
- `sudo service postgresql stop` to stop running your database.

The default admin user, postgres, needs a password assigned in order to connect to a database. To set a password:

Enter the command: `sudo passwd postgres`
You will get a prompt to enter your new password.
Close and reopen your terminal.
To run PostgreSQL with psql shell:

Start your postgres service: `sudo service postgresql start`
Connect to the postgres service and open the psql shell: `sudo -u postgres psql`
Once you have successfully entered the psql shell, you will see your command line change to look like this: 
```
postgres=#
```

To exit postgres=# enter: \q or use the shortcut key: Ctrl+D

To see what user accounts have been created on your PostgreSQL installation, use from your WSL terminal: psql -c "\du" ...or just \du if you have the psql shell open. This command will display columns: Account User Name, List of Roles Attributes, and Member of role group(s). To exit back to the command line, enter: q.

## Python3 & Pip3

Python3 should come with Ubuntu 18.04 and later. Please confirm by running command: `python3 --version`

To install pip3 run `sudo apt install python3-pip` and confirm its installation with `pip3 --version`

## Django

Install the python3 Django virtual environment with: `sudo apt install python3-django`

Then run: `pip3 install django`

Confirm installation with `django-admin --version`

https://linuxize.com/post/how-to-install-pip-on-ubuntu-18.04/

* [x] [Command Line](command-line-setup.md)
* [x] [Installing Git](git-installation.md)
* [x] [Tech Stacks](web-technologies.md)
* [ ] [Desktop Applications](desktop-applications.md)