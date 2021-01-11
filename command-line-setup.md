# Installfest for Windows, Step 1: Unix Terminal on Windows

1. Follow [Microsoft's instructions](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide) to get Linux installed on your system.

2. Download Ubuntu (no version after it) to install Ubuntu 20.04 LTS, which is one of the latest versions as of writing and will come with software (like Python3) pre-installed.

3. Install Windows Terminal from the Windows App Store.

NOTE: You may wish to install VSCode first before continuing. 

Once VSCode is downloaded, you can set up opening it up from WSL by typing the command `code .`

We recommend this terminal in class instead of the Ubuntu terminal because its easier to zoom in using by pressing `ctrl` and `plus`. 

I will probably ask you to zoom in your terminal when we screen share. :) 

Open up Windows Terminal and click on the the downward facing arrow next to the new tab (+) button. Click on the settings button.

look for a field called `defaultProfile: ...`

scroll down until you find a field called `"profiles": ...` and look for `"list":...` nested inside

copy the `guid: "{...}"` of `name: ubuntu` and paste it into `defaultProfile:...`

Inside the `guid: {UBUNTU GUID}`, add a new property beneath `name: ubuntu`.

`"startingDirectory": "//wsl$/Ubuntu/home/ YOUR USERNAME HERE `

4. Type `pwd` at the command line. If it gives a path similar to `/home/yourname`, then you're in great shape! If it says that is not a recognized command, try running `bash` or `zsh` first and then `pwd`. If you get errors, please call over an instructor.

If you do not have bash or Zsh installed, I recommend installing Zsh with the following command:

`sudo apt-get update && sudo apt-get -y install zsh`

Make Zsh your default terminal by running:

`chsh -s /bin/zsh`

Install a Zsh theme like `oh-my-zsh` to have a beautiful, easy to use Zsh terminal!

5. Run `apt-get update` to ensure your Linux installation is up to date.

6. Run
```
sudo apt-get -f install
```
to ensure all default packages are installed.

Excellent-you now have Linux installed on your computer, which will let you use the nearly same commands as everyone else for the remainder of the course.

For example, when someone with a Mac says "command" or "apple" key, press control instead. Other keyboard commands may be different, and we've highlighted a few for you to memorize.

7. Git

[Your next step will be installing git!](git-installation.md)

After git: your developer tools!
1. Set up your **Development Environment**:
    * [x] The BASH Command Line
    * [ ] [Installing Git](git-installation.md)
    * [ ] [Developer Tools](developer-tools.md)
2. Set up your **Web Technologies**:
    * [ ] [Web Technologies](web-technologies.md)