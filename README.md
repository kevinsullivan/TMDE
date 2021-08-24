# Get Your Mathematical Development Environment Here!

You're here because you want the coolest mathematical development environment ever, *and* you want it with "near-zero" configuring of your own computer (really). Well, that is just what we have for you. You provide properly running VSCode and Docker Desktop installations on a Windows 10 (footnote below) or MacOS computer, and we give you The (coolest) Mathematical Development Environment (ever). To get it, just follow the yellow brick road .,..,.,..,.,...

## .,,.. the Yellow Brick Road
- Update your operating system:
  - If MacOS: Be sure your OS is up-to-date (current version of Big Sur, 11.5.2 as of this writing).
  - If Windows: 
    - Windows 10 Home won't do, but it's probably what you have. Run the System Information App to find out.
    - You must either be running or update to Windows 10 Professional, Enterprises, or Education
      - Outside UVa:  Update keys are readily available online
      - UVa students: Get or update to Windows 10 Education through ITS, as follows:
        1. Get OS Windows Update license key from ITS: https://virginia.service-now.com/its/.  
        2. Click Software in the left-hand navigation. Select the *latest* Windows 10 Education version. Get an update key.
        3. After obtaining the OS key, copy and paste it in to the Windows Activation page (same screen as Windows Update).
        4. Reboot your machine. You can check the Windows *System Information* app to confirm that your OS is updated.
- Have a GitHub account. Create one for yourself if necessary. It's free: https://github.com/
- Install Docker Desktop: https://www.docker.com/products/docker-desktop. It's free.
- Install VSCode: https://code.visualstudio.com/download. It's free.
- Launch Docker Desktop and watch for it to complete its start-up procedures. While it starts up, continue to the remaining instructions that follow here. 
- Use GitHub to fork this repository now. How? Here:
  - Be logged in to your GitHub account.
  - Visit *this* repository on GitHub (which is probably where you're reading this) while logged in to your GitHub account.
  - "Fork" this repo using the *Fork* button in the upper right corner. This will create a clone of this repository (a copy that remembers where it came from) under your GitHub account. 
  -   Visit your GitHub web page to confirm that you now own a clone of this repository. Click to view the repository.
  -   Select the green Code button, then HTTPS, then copy the URL that is provided. This will be the GitHub URL of your newly forked copy of the respository.
- Start up your new environment
  - Start a *new* VSCode window. 
  - Use CTRL/CMD-SHIFT-P to bring up the VSCode command palatte. 
  - Search for and select *Clone Repository in Container Volume*
  - Paste in the GitHub URL of your new clone as the argument.
  - If you're asked to choose something, select *unique repository*.
- Now wait while your environment is built. You can click in the lower right to see the build process if you want. Wait for the building activity to end and for your environment to "boot up" before taking any further actions. There is a status bar at the bottom of the screen that reflects build processes status and activities.
- Check to see that everything is working
  - Open the test.lean file (src/test/test_lean_mathlib.lean)
  -Check that the conditions described therein are satisfied.
-You may now work in and exit from VSCode as you wish. VSCode will let you re-open this project when you're ready to work on it again.

## What you have wrought

You now have, up and running, the coolest discrete math learning environment ever. Yay! You're done.

## Of course, if your're curious
- Yep, that was clickbait, but hey
- Your new development environment delivers the following capabilities among others
- VSCode, open and ready for you to start, and to continue, developing the logic of your application, in a professionally competent manner
- A containerized/virtual computer delivering a richly configured discrete math learning environment
  - Ubuntu 20.04 LTS operating system
  - Lean Prover Community, with mathlib
  - Widely used VSCode IDE
  - Root "shell" into Ubuntu container.
  - VSCode operates on a clone of your repo automatically created in your container
- The entire development environment builds from the ground up when you first follow thees procedures
- You can change and rebuild your own environment anytime, or incorporate improvements that we deliver from upstream 
- The ability to pull "upstream" updates to integrate changes to the main repository into your clones. 
- The ability to issue "pull requests," asking that your changes be incorporated into our upstream respository 
- The clone of your repo is in the directory, /workspaces, in the container. 

## If you find a problem or an opportunity ...
If you think you've found a problem, revisit this GitHub page and report an Issue. Better yet, if you then fix the problem on your own clone of this site, commit and push it to your GitHub repo then send us a Pull Request, which will send us your changes to review and possible merge them into our main repository, whereupon they will become available to everyone else, as well.  


## Legal and contact
Copyright: © 2021 By the Rector and Visitors of the University of Virginia.
Supervising Author: Kevin Sullivan. UVa CS Dept. sullivan@virginia.edu. 
Acknowledgements: Thank you to multiple students for read, test, and fixing. This work was supported in part by NSF Grant ...


