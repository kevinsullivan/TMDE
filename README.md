# Get Your CS2120 Discrete Math Learning Environment Here!

You're here because you want the coolest discrete math learning environment ever, *and* you want it with *minimal* configuring of your own computer. Good news! We have just that for you. You must provide properly running VSCode and Docker Desktop installations on either Windows 10 (footnote below) or MacOS. Then, just follow the yellow brick road .,..,.,..,.,...

## ... the Yellow Brick Road
- Update your operating system:
  - If MacOS: Be sure your OS is completely up-to-date (current version of Big Sur, 11.5.2 as of this writing).
  - If Windows: 
    - Windows 10 Home won't do, but it's probably what you have. You must update to Windows 10 Professional, Enterprises, or Education.
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
  -   Visit your GitHub web page to confirm that you now own a clone of this repository. 
  -   Now you will "fire up" a whole new computer, that we're giving you, within a Docker container; and this computer will in turn have a clone of your new clone.
  -   You will work entirely through VSCode and with direct acccess to the (virtual) computer that provide with your new discrete math learning environment (DMLE). The next step requires the GitHub URL of your new clone.
  -   Select the green Code button, then HTTPS, then copy the URL that is provided. This will be the GitHub URL of your newly forked copy of the respository.
- Launch DMLE
  - Launch a *new* VSCode window. 
  - Use CTRL/CMD-SHIFT-P to bring up the VSCode command palatte. 
  - Search for and select *Clone Repository in Container Volume*
  - Paste in the GitHub URL of your new clone as the argument.
  - If you're asked to choose something, select *unique repository*.
- Now just wait. You environment is being built from the ground up. You can click to see the build process if you want. Wait for your development environment to completely "boot up" before taking any further actions. There is a status bar at the bottom of the screen that reflects build processes status and activities.
- Check to see that everything is working
  - Open the test.lean file (src/test/test_lean_mathlib.lean)
  -Check that the conditions described therein are satisfied.
  - Cases
    - true: celebrate
    - false: tell us!  

## What you have wrought

You now have, up and running, the remarkable discrete math learning environment for CS2120 (Fall 2021) Yay! You're done.

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

## Help Make It Even Better
Let us know what you think. Better yet, make it better and send us a PR. You'll be completely set up to do that by the results of this procedure. 


## Legal and contact
Copyright: © 2021 By the Rector and Visitors of the University of Virginia.
Supervising Author: Kevin Sullivan. UVa CS Dept. sullivan@virginia.edu. 
Acknowledgements: Thank you to multiple students for read, test, and fixing. This work was supported in part by NSF Grant ...


