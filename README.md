# freeCodeCamp San Francisco WSL2/Linux Guide

## Table of Contents
- How to use this guide/FAQ 
- Installing WSL2 on your Windows Computer
- What will be installed on my computer?
- Setting up your WSL2 environment for freeCodeCamp's Curriculum

## How to use this guide
Based on discussion within our chapter's membership, we agreed that there needed to be a resource for setting up one's own computer for web development outside of the in-browser workspaces that freeCodeCamp provides early in the curriculum. Setting up a working dev environment is important for success later in the full-stack certifications. While many members in our chapter use Macbooks at meet-ups and other chapter events, I wanted to create a resource that proves the viability of using other, more affordable computer systems.

Windows Subsystem Linux 2, or WSL2 for short, creates an instance of a Linux operating system running on a Windows computer. The advantages of performing tasks inside this embedded system are explained in detail later in this guide. Setting up a Dev Environment with WSL2 allows Windows computer users to seamless work with other campers using Mac or Linux. 

**While this guide is designed for WSL2 on Windows computers, most, if not all, of these instructions can be followed for setting up an Ubuntu Linux dev environment.**

## What will be installed on my computer?
- Windows Subsystem Linux 2
- Ubuntu Terminal
- Zsh (with Oh-My-Zsh configuration)
- VSCode (+ some optional helpful extensions)
- Git
- Node.js
- NPM 
- Python3
- Django
- Heroku CLI
- MongoDB
- PostgreSQL
- Slack (Desktop App recommended for chapter news!)

^These tools will allow you to follow the freeCodeCamp curriculum and fully participate in most of our chapter's activities including hackathons, open-source projects, and to even launch your own! There are other programming languages and frameworks you may be interested in such as Ruby, Rails, and PHP. We may add those in the future! 

Please read the FAQ section before continuing to look over the installation instructions.

**DISCLAIMER: This information is provided as-is. You are personally responsible for the effects installing WSL on your computer may have. *This document is a chapter open-source project and subject to continued updates.**

## FAQ
- *Why should I install WSL2 on my computer?*
   - We recommend installing WSL2 to provide a (mostly) seamless experience working with the freeCodeCamp curriculum and other learning resources that were designed with UNIX-based operating systems like Linux or Mac OS. These operating systems have a different structure than Windows, and many tools used in the FCC curriculum are best managed with a UNIX OS.

- *What recommended specs/kind of Windows computer do you recommend for learning web development at freeCodeCamp SF?*
   - Here are some recommended specs for any computer:
      - Processor: Intel i5, Intel i7 or equivalent and above (like AMD Ryzen 5 or 7)
      - RAM: at least 8GB (16GB or more recommended for remote work)
      - Storage: 128GB or more available storage
      - compatible with Windows 10 version 1903 or later. (see installation instructions to check compatibility)
   - Most premium business laptop lines from major brands like Dell or Thinkpad will meet these requirements. You can also ask around if you're curious about other Campers' set-ups! :)

- *There are Windows versions of (Git, PostgreSQL, etc.). Why do I need to use the Linux versions of tools?*
   - The version of Linux we install to our computers is treated as a separate operating system, so some tools might not be able to detect what's going on inside our WSL installation. Plus, we will mostly be using our Linux terminal to manage these tools.

- *Why are we installing Django instead of Flask (or other web development frameworks like Ruby on Rails, Meteor.js, etc.)?*
   - We include installation instructions for Django because it is a popular web development framework using Python. It is also an opinionated framework, so it is a good counterpoint to unopinionated frameworks used in our resources like Express.js. You are welcome to install other tech stacks you are interested in learning.

- *Can I use a chromebook at freeCodeCamp SF?*
   - You can definitely get through the very early parts of the front-end and full-stack certifications on freeCodeCamp.org using a chromebook. In fact, some of the early front-end projects will be coded entirely on online workspaces like codepen.io. However, the curriculum will quickly become difficult if you are not able to move away from freeCodeCamp's in-browser workspaces and start working with the back-end or using front-end libraries like React or Vue.
   - We recommend getting a Linux, Mac OS, WSL computer as soon as possible to establish a working dev environment for yourself. You will need a fully-featured operating system to practice controlling your computer with the command line and using professional development tools and systems like Git or a code editor. There are guides to setting up a dev environment on chromebooks, but we haven't found many of them to be friendly to beginners. For this reason, we recommend following this installation guide.

## Ready to get started?
- Click through the links below installation instructions!
* [ ] [Command Line](command-line-setup.md)
* [ ] [Installing Git](git-configuration.md)
* [ ] [Databases and Frameworks](dbs-languages-frameworks.md)
* [ ] [Desktop Applications](desktop-applications.md)
