# Mac-Updater
script to run updates for Macs

In order for either of the MacUpdaters to run correctly, you will need admin priveleges for your computer. 
The MacUpdaterResourceInstaller is used to install other programs utilized in the MacUpdaterDailyTasks.

Those resources are as follows:

  Git: Utilized to install SpeedTestCli. It will check what your current version of Git is, if it is     outdated or not already instaled, it will install or update Git.
  SpeedTestCLI: used to check current internet connection speed. 
  
That's it! Nothing heavy, just a few items used in the DailyTask program.

The MacUpdaterDailyTasks is a code I have been using to simplify keeping my Macbook updated. Instead of running the individual commands or clicking through GUIs, this saved that time by just opening terminal and running this script. The following is a walkthrough of all actions taken by the script:

who: We start with this in order to identify who all is currently logged into the computer. A simple security check to make sure you don't see any unwanted connecitons. If anything doesn't look right, stop with program with contrl c ( ^c ) and investigate or take necessary actions. If you are the only user that is supposed to be logged in, then you should only see your account name twice: once for being logged into the computer and once for being the user in the terminal app. 

SpeedTest: Next we run an internet speedtest. This just takes a few moments, but if you notice your speed if lower than usual, then you may want to run updates at a later time. 

softwareupdate: Here we are checking for any updates related to the operating system (OS). Keeping your OS up to date is usually recommended, especially since they typically include security updates for your computer. 

mas: This is where we will be updating all the applications on the computer. Instead of going to each app and checking for updates, this will do it all for you.

-sudoPanda
