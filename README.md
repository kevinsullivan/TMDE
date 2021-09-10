# The Mathematics Development Environment (TMDE)
## Why you're here

You're here because you want the coolest mathematical development environment ever, with very little configuring of your own computer required. You must provide VSCode and Docker Desktop running properly on a Windows 10+ or MacOS computer. We then provide you with a Mathematics Development Environment. Among its features are the following: 
- the Lean Prover
- its library of formalized mathematics (mathlib)
- a Docker container providing a complete, ready-for-Lean-development platform based on Ubuntu 20.04 LTS
- a containerized clone of (your fork of) this repo as starting point for development within that container
- your own GitHub repo (your fork of this project), to which you can push changes from your containerized clone
- a nicely configured VSCode IDE, already opened for immediate development on that containerized clone 
- VSCode terminal/shells into the containerized Ubuntu platform with full administrative (sudo) privileges
- You can extend and rebuild the environment by adding elements to a Dockerfile we provide
- Start-up after the first one are quick; the first time requires pre-built image downloading

To get it, just follow the yellow brick road ...

## The Yellow Brick Road
- Update your operating system:
  - If MacOS: Be sure your OS is up-to-date (current version of Big Sur, 11.5.2 as of this writing).
  - If Windows: 
    - First update your Windows OS to the current release (run Windows Update until it stops finding more updates to install). 
    - Windows 10 Home won't do: you must either be running, or update to, Windows 10 Professional, Enterprises, or Education. 
    - Update keys are readily and immediately available online and might be available for free through your educational institution.
- Install git on your computer (if you know you already have it, skip this step):
  - Windows: Download and run the Git for Windows installer here: <https://git-scm.com/download/win>
  - OSX/MacOs
    - Find and run the Terminal program
    - Enter the following command in the window: *git --version*
    - If git is not installed, you'll be asked whether you want it installed. Answer yes. 
- Have a GitHub account. Create one for yourself if necessary. It's free: https://github.com/
- Install Docker Desktop: https://www.docker.com/products/docker-desktop. It's free. If you have it, *be sure* to update it to a current version.
- Install VSCode: https://code.visualstudio.com/download. It's free. NB: Docker Desktop *must* be running when you start VSCode as part of these instructions, as you will be using Docker container related commands from within VSCode.
- Launch Docker Desktop and watch for it to complete its start-up procedures. While it starts up, continue to the remaining instructions that follow here. 
- Use GitHub to fork this repository now. How? Here:
  - Be logged in to your GitHub account.
  - Visit *this* repository on GitHub (which is probably where you're reading this) while logged in to your GitHub account.
  - "Fork" this repo using the *Fork* button in the upper right corner. This will create a clone of this repository (a copy that remembers where it came from) under your GitHub account. We recommend that you should change the name of your GitHub repo (hit the pencil icon next to its name on GitHub to start editing it) to reflect the nature of your project. Doing this will avoid conflicts should you try to do this procedure again.
  -   Visit your GitHub web page to confirm that you now own a clone of this repository. Click to view the repository.
  -   Select the green Code button, then HTTPS, then copy the URL that is provided. This will be the GitHub URL of your newly forked copy of the respository.
- Start up your new environment
  - Start a *new* VSCode window.
  - Install the _Remote Containers_ extension.
    - Click on the Extensions icon (four boxes, one out of place) on the left panel of VSCode
    - Search for, select, and install the _Remote Containers_ extension
    - A new green icon >< should appear in the lower left corner of your VSCode window 
  - Use CTRL/CMD-SHIFT-P to bring up the VSCode command palatte. 
  - Search for and select *Clone Repository in Container Volume*
  - Paste in the GitHub URL of your new clone as the argument.
  - If you're asked to choose something, select *unique repository*.
- Now wait while your environment is built. You can click in the lower right to see the build process if you want. Wait for the building activity to end and for your environment to "boot up" before taking any further actions. There is a status bar at the bottom of the screen that reflects build processes status and activities.
- Check to see that everything is working
  - Open the test.lean file (src/test/test_lean_mathlib.lean)
  - Check that the conditions described therein are satisfied.
- Open a terminal and configure git in your Ubuntu container 
  - git config --global user.name "<your name here>"
  - git config --global user.email <you@someemail.com>
  
- You may now work in and exit from VSCode as you wish. VSCode will let you re-open this project when you're ready to work on it again.

You now have, up and running, the coolest mathematical development environment ever. You're done here now!

## If you find a problem or see an opportunity ...
If you think you've found a problem, revisit this GitHub page and report an Issue. Better yet, if you then fix the problem on your own clone of this site, commit and push it to your GitHub repo then send us a *Pull Request*. That will will send us your changes to review and possibly merge them into our main repository, whereupon they will then become available for anyone else to *Pull*, as well.  

## Other notes
- The solution we've described won't quite work "out of the box" on Linux machines because Linux doesn't support Docker Desktop.
- Linux users will likely use *podman* in lieu of Docker's version of docker. The VSCode "Clone Repo in Container" command doesn't appear to work when using podman, but we've been told that cloning your fork of our repo into the container manually and then running the VSCode Open Folder command does work. We haven't confirmed.

## Legal and contact
- Acknowledgement: This work is supported in part by the National Science Foundation under grant (Award Abstract) #1909414.
- Copyright: © 2021 by Kevin Sullivan, Sebastian Elbaum, et al.
- Permission: You must preserve our copyright notice when making use of this material. We request that you let us know of any use of this technology beyond the purely personal: e.g., for teaching, reseasrch, government, or industrial purposes. 
- Primary and Contact Author: Kevin Sullivan. UVa CS Dept. sullivan@virginia.edu. Acknowledgements for contributions that helped me to produce this repository go to Charlie Houghton, Andrew Elsey, et al.  
