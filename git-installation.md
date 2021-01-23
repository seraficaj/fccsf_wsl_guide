## Installing Git

run `sudo apt-get install git`

#### Configuring a Global git ignore

> Note: This is **IMPORTANT**

Everyone should have a global **git ignore** file so that you don’t have to worry about making the appropriate entries in a project’s git ignore.

First, create the file:  `touch ~/.gitignore_global`

Next, configure git to use this file:  `git config --global core.excludesfile ~/.gitignore_global`

Finally, lets put some good stuff in there by editing the newly created `.gitignore_global` file using VS Code:

1. `code ~/.gitignore_global` to open the file in VS Code

2. Copy/paste the following:

	```sh
	# This is a list of rules for ignoring files in every Git repositories on your computer.
	# See https://help.github.com/articles/ignoring-files
	
	# Compiled source #
	###################
	*.class
	*.com
	*.dll
	*.exe
	*.o
	*.so
	
	# Packages #
	############
	# it's better to unpack these files and commit the raw source
	# git has its own built in compression methods
	*.7z
	*.dmg
	*.gz
	*.iso
	*.jar
	*.rar
	*.tar
	*.zip
	
	# Logs and databases #
	######################
	*.log
	
	# OS generated files #
	######################
	._*
	.DS_Store
	.DS_Store?
	.Spotlight-V100
	.Trashes
	ehthumbs.db
	Thumbs.db
	
	# Testing #
	###########
	.rspec
	capybara-*.html
	coverage
	pickle-email-*.html
	rerun.txt
	spec/reports
	spec/tmp
	test/tmp
	test/version_tmp
	
	# node #
	########
	node_modules
	
	# Rails #
	#########
	**.orig
	*.rbc
	*.sassc
	.project
	.rvmrc
	.sass-cache
	/.bundle
	/db/*.sqlite3
	/log/*
	/public/system/*
	/tmp/*
	/vendor/bundle
	
	
	# Ruby #
	########
	*.gem
	*.rbc
	.bundle
	.config
	.yardoc
	_yardoc
	doc/
	InstalledFiles
	lib/bundler/man
	pkg
	rdoc
	tmp
	
	# for a library or gem, you might want to ignore these files since the code is
	# intended to run in multiple environments; otherwise, check them in:
	# Gemfile.lock
	# .ruby-version
	# .ruby-gemset
	
	# CTags #
	#########
	tags
	
	# Env #
	#######
	.env
	
	# Python #
	#######
	*.pyc
	__pycache__/
	```

3. Save the file.

#### Avoiding Having to Create A Git Message Every Time a Git Merge Takes Place

By default, git asks for a commit message any time a merge takes place, for example, you'll be running this command quite a bit:  `git pull upstream master`.

To avoid this from happening, we can add a single line to our terminal configuration - this is the line we're going to need to add anywhere inside of the file identified below:

```
export GIT_MERGE_AUTOEDIT=no
```

**If NOT using ZSH:**

Use VS Code to edit the `~/.bash_profile` file:

```
code ~/.bash_profile
```

**For ZSH users:**

Use VS Code to edit the `~/.zshrc` file:

```
code ~/.zshrc
```

**Regardless of which file you edited, be sure to save it.  You will also need to quit (`command + Q`) terminal and relaunch it for this setting to take effect.**

Next up: Setting Up Languages and Frameworks!
* [X] [Command Line](command-line-setup.md)
* [X] [Installing Git](git-installation.md)
* [ ] [Databases and Frameworks](dbs-frameworks.md)
* [ ] [Desktop Applications](desktop-applications.md)
