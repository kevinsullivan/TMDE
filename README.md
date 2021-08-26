# The Mathematics Development Environment (TMDE)
## Why you're here

You're here because you want the coolest mathematical development environment ever, with very little configuring of your own computer required. You must provide VSCode and Docker Desktop running properly on a Windows 10 or MacOS computer, and we then supply you with a Mathematics Development Environment, based on VSCode, the Lean Prover and its library of formalized mathematics, opened to a new, GitHub-backed project, served from a container providing Ubuntu 20.04 LTS, Lean, its dependencies and a few other essentials. The mixed news for Windows users is that we can't guarantee that Docker Deskop runs properly on a Windows 10 *Home* computer, even though it's advertised to. We've found it troubled. We advise to obtain an upgrade key to update to Windows 10 Professional or Education. Now just follow the yellow brick road .,..,.

## .,,.. the Yellow Brick Road
- Update your operating system:
  - If MacOS: Be sure your OS is up-to-date (current version of Big Sur, 11.5.2 as of this writing).
  - If Windows: 
    - First update your Windows OS to the current release (run Windows Update until it stops finding more updates to install). 
    - Windows 10 Home won't do: you must either be running or update to Windows 10 Professional, Enterprises, or Education. 
    - Update keys are readily and immediately available online and might be available for free through your educational institution.
- Install git on your computer (if you know you already have it, skip this step):
  - Windows: Download and run the Git for Windows installer here: <https://git-scm.com/download/win>
  - OSX/MacOs
    - Find and run the Terminal program
    - Enter the following command in the window: *git --version*
    - If git is not installed, you'll be asked whether you want it installed. Answer yes. 
- Have a GitHub account. Create one for yourself if necessary. It's free: https://github.com/
- Install Docker Desktop: https://www.docker.com/products/docker-desktop. It's free. If you already have it, update it to the current version.
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
- You may now work in and exit from VSCode as you wish. VSCode will let you re-open this project when you're ready to work on it again.

You now have, up and running, the coolest mathematical development environment ever. You're done here now!

## Of course, if your're curious
- Yep, that was clickbait, but hey, your new environment delivers many capabilities. They include the following.
  - VSCode will be open and ready for you to start developing your applications with professional-quality infrastructure
  - A containerized/virtual computer delivering a richly configured environment including the Lean Prover and its library of formalized mathematics (mathlib)
    - Ubuntu 20.04 LTS operating system
    - Lean Prover Community, with mathlib
    - Widely used VSCode IDE
    - Root "shell" into Ubuntu container.
    - VSCode operates on a clone of your repo created in your container
  - The entire development environment builds itself when you first follow these procedures
- The clone of your repo is in the directory, /workspaces, in the container. 

## If you find a problem or an opportunity ...
If you think you've found a problem, revisit this GitHub page and report an Issue. Better yet, if you then fix the problem on your own clone of this site, commit and push it to your GitHub repo then send us a *Pull Request*. That will will send us your changes to review and possibly merge them into our main repository, whereupon they will then become available for anyone else to *Pull*, as well.  

## Other notes
- More sophisticated developers might already be running *podman* in lieu of Docker's version of docker. One user reports that the Clone Repo in Container VSCode command doesn't work but that cloning the repo manually and then running the Open Folder command does work. We haven''t confirmed.

## Legal and contact
- Acknowledgement: This work is supported in part by the National Science Foundation under grant (Award Abstract) #1909414.
- Copyright: © 2021 by Kevin Sullivan, Sebastian Elbaum, et al.
- Permission: You must preserve our copyright notice when making use of this material. We request that you let us know of any use of this technology beyond the purely personal: e.g., for teaching, reseasrch, government, or industrial purposes. 
- Primary and Contact Author: Kevin Sullivan. UVa CS Dept. sullivan@virginia.edu. Acknowledgements for contributions that helped me to produce this repository go to Charlie Houghton, Andrew Elsey, et al.  
