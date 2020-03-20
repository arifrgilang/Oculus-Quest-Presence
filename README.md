# Oculus-Quest-Presence

> Discord Rich Presence for the Oculus Quest

---

## How to install

- Dowload the zip file from <a href="https://github.com/madmagic007/Oculus-Quest-Presence/releases/tag/2.0" target="_blank">here</a> and unzip it somwhere.
- install <a href="https://sidequestvr.com/#/download" target="_blank">sidequest</a> on your pc (skip if you already have sidequest installed).
- Download <a href="https://github.com/tverona1/QuestAppLauncher/releases/tag/v0.10.2" target="_blank">Quest app launcher</a>.
- Sideload the quest app launcher apk to your quest (skip if already installed), plenty of tutorials on how to sideload apks exist.
- When your quest is connected to your pc via usb and connected to internet, look in the top left corner of the sidequest window for the wifi ip of your quest and note it down somewere. It should look something like 192.168.1.100.
- From the zip file, sideload the Oculus Quest Discord RPC.ak to your quest.
- Run oqrpc.exe from the zip file.
- Once its installed, run the Oculus Quest Discord RPC.jar and a window should pop up asking for the ip of your oculus quest.
- Make sure your oculus quest is powered on and connected to the internet. Next type the ip you noted earlier in the text area and hit validate. if everything is done right, it should say "found device, but apk is not running on devide" (don't close this window yet).
- Open the quest app launcher on your quest, go to library > unknown sources and look for something called quest app laucnher.
- In quest app launcher, click on the 2D tab and look for oqrpc.apk and run it.
- A window should open saying presence is running with a button "terminate presence" below.
- Go back to your pc and hit the validate button in the window again and it should say something like "apk is running on device, everything ready to go". if that's the case, go back in your quest, hit the terminate presence button and restart the oqrpc apk via quest app laucher.
- A notification should appear on your computer and if discord is running, it should show that you are playing on your oculus quest!
  
---

##  Things to note & issues im aware of

- If your computer/quest lose internet conection for more than one minute, the presence will stop showing. To restore this right click on the oculus quest rpc icon in the system tray on your computer and hit "manual send".
- If your computer is turned on after your quest, it wont show the presence untill you manually start the apk via quest app launcher.
- Both programs "should" automatically start with device boot, but thay may not always the be case. im working on making this more reliable.
- When you turn on your quest, there "should" be no need to manually start the oqrpc apk. It takes a while for discord to display the presence after you turned on your quest and connected it to internet, so just be patient. If it really doesnt show, manually start the apk via quest app launcher.
- The way i get the names of the games you are playing is by reading the package name of the current topmost process. For Pavlov this would be "com.vankrupt.pavlov" i use an api that reads the lang.json file found in this repository to get a better looking name, like "Pavlov Vr" in this case. If a package name isnt listed in the lang file, it will show just the last part of that package name, for pavlov that would be just "pavlov". I will try to add as many names as posible, but ofcourse i dont know every game so if you find one, make sure to report it to me.

---

## Contact me for bug reporting or reporting an unlisted name

- Discord: ⎛⎝⧹Maͫgͣiͩc⧸⎠⎞#6891
- Twitter: @madmagic5
- Reddit: u/madmagic008
