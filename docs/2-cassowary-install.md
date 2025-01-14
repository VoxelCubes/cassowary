# 2. Installing cassowary on Windows 10 and Linux

## On Windows 10
- Open Settings, click on System, scroll to bottom and click on Remote desktop then click on Enable Remote Desktop and click confirm!
- Open this page and download latest .zip from the [release page](https://github.com/casualsnek/cassowary/releases/)
- Extract the downloaded .zip file
- Double click on setup.bat located on extracted directory
- Logout and login again to windows session
- After you have logged in continue the instructions below

## On Linux
Here we will be using Arch Linux. You can easily find equivalent commands for your Linux distro.

- Go to the [release page](https://github.com/casualsnek/cassowary/releases/) and download latest `.whl`;  
- Open terminal on the location where you downloaded the `.whl` file;  
- Install python3, python-pip, freerdp and dependencies by running following commands on terminal:

```
$ sudo pacman -S python3 python-pip freerdp
$ pip3 install PyQt5
```

- Install the downloaded `.whl` file by running:

```
$ pip install cassowary*
```

- Launch cassowary configuration utility with:

```
$ python3 -m cassowary -a
```

- Head over to Misc tab and click on **"Setup Autostart"** and **"Create"**. This will bring cassowary to your application menu and setup background service autostart;
- Enter the VM name from the VM setup step; in this case `Win10`;
- Click on "Save changes" and then on **"Autodetect"**, this should automatically fill up the VM IP;
- Click "Save changes" again then click **"Autofill host/username"** then enter the password you set during the windows setup. Then click "Save changes" again;
- Now goto **"Guest app"** tab and create shortcut for any application you want.

Now you can find application on your application menu which you can use to launch apps easily
You can explore other commandline usage of cassowary by running:

```
$ python -m cassowary -h
```
