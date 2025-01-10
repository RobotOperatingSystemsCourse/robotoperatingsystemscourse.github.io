---
title: Setup
layout: page
nav_order: 6
---

# Setup

All of the programming assignments in this course have been developed for Linux. We will officially support two methods of development: CAEN Linux Remote Login Server (Red Hat Enterprise Linux 8.10 Ootpa) and the MBot (Debian GNU/Linux 12 Bookworm).

## CAEN Linux Remote Login Service

The instructions for using the CAEN Linux Remote Login Service via SSH can be found [here](https://teamdynamix.umich.edu/TDClient/76/Portal/KB/ArticleDet?ID=5002).

In this course, we advise you to set up the VS Code Remote extension to be used with the CAEN Linux Remote Login Service so that you can develop with an IDE in a Linux environment at your convenience. 

1. To set up this workflow, first [install Visual Studio Code](https://code.visualstudio.com) if you have not already, and then install the [Remote Explorer](https://marketplace.visualstudio.com/items?itemName=ms-vscode.remote-explorer) and [Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh) VS Code extensions.
<img src="../assets/images/setup/vscode_setup_1.png" alt="Remote Explorer" width="25%" />
<img src="../assets/images/setup/vscode_setup_2.png" alt="Remote - SSH" width="25%" />

2. Navigate to the Remote Explorer extension tab on the left side of the VS Code browser. Click the settings wheel to open the SSH config file.
<img src="../assets/images/setup/vscode_setup_3.png" alt="Open SSH config file" width="50%" />
<img src="../assets/images/setup/vscode_setup_4.png" alt="SSH config file" width="50%" />

3. Copy the following into the file. Replace `[UNIQNAME]` with your uniqname.
```plaintext
Host oncampus-course.engin.umich.edu
  HostName oncampus-course.engin.umich.edu
  User [UNIQNAME]
```

4. Open the Command Pallette by pressing ctrl/cmd + shift + p. Search "Remote" and open the Remote-SSH: Settings.<br>
<img src="../assets/images/setup/vscode_setup_5.png" alt="Command Palette" width="50%" />

5. Scroll down towards the bottom of the settings and ensure that the **Show Login Terminal** is toggled **on** and the **Use Local Server** option is toggled **off**.<br>
<img src="../assets/images/setup/vscode_setup_6.png" alt="Show Login Terminal" width="75%" />
<img src="../assets/images/setup/vscode_setup_7.png" alt="Use Local Server" width="75%" />

6. Close out of the Command Palette and navigate back to the Remote Explorer window. You can choose to open the remote window in the current VS Code window (arrow icon) or a new window (folder icon). Select one. <br>
<img src="../assets/images/setup/vscode_setup_8.png" alt="VS Code Remote Select" width="50%" />

7. You should see a prompt for your password and two factor authentication. Enter your password and choose an option to authenticate with your device.<br>
<img src="../assets/images/setup/vscode_setup_9.png" alt="DUO" width="50%" />

8. If successful, VS Code should now connect to the CAEN Linux Remote Login Server. You can choose to open a folder and navigate through the directory. When selecting a folder, VS Code may prompt you again for your password and 2FA. Follow steps 7 and 8 if this occurs.

## MBot Setup

You can use VS Code Remote to develop on the MBots as well.

1. Click on the + button in the Remote Explorer window.<br>
<img src="../assets/images/setup/vscode_setup_3.png" alt="Click on +" width="50%" />

2. Find the IP address of the MBot. It should display on the OLED after turning the battery on. Enter `ssh mbot@[IP ADDRESS]` and the password once prompted.

3. You can now open a folder, clone your repository, and develop your assignments with the VS Code IDE on the MBot.