# My instance is not compatible with Java version [number] (Prism Launcher)!

To update your java instance, you need to get a new JDK for the respective Java version. If the error says you need Java version 21, you need to get a JDK version 21. **For this tutorial, we are going to download JDK 21**.

### 1. Downloading JDK
There are many places to download a jdk such as openjdk and adoptium. We are going to use adoptium. Go to this link: https://adoptium.net/temurin/releases/?os=windows&arch=x64&package=jdk

> [!WARNING]
> **Make sure you are downloading the jdk for the right OPERATING SYSTEM, ARCHITECTURE (its usually x64), PACKAGE TYPE (jdk), and VERSION (21 - LTS)**

Once you put the right stuff for the jdk, you can either choose to download with `.msi` or `.zip`. It doesn't really matter I prefer to download the `.msi` file because it gives you a GUI to help you set it up which I highly recommand.

### 2. Opening and setting up the .msi file
Once you finished installing the `.msi` file, open the file and you will greeted with the installation wizard. Just ignore the stuff and press "next" and install. Make sure you give the file administrator permissions to download.

### 3. Changing the JDK version in Prism Launcher (i.e the complicated part)
- Once the JDK is done downloading, open up Prism Launcher
- Right click the instance you want to update Java and press "edit"
- Go to "settings". It's on the left side of the pop up.
- You should now see a screen that says "Java installation" and a long file path. You need to find the JDK's `javaw.exe` file.
- Press the "browse" button that is next to the long file path and it will open your file explorer.
- Go to "local disk" which under "This PC"
- Go to Program Files
- Go to Eclipse Adoptium
- Go to `jdk-21-something-something` 
- Go to "bin"
- Scroll down and find `javaw.exe`. **IT IS NOT `java.exe`**
- Press `javae.exe` **ONCE**. **DO NOT DOUBLE CLICK IT**. Then press the "open" button on your file explorer

And voila, you updated Java. Make sure you check the "Java Installation" checkbox in the instance settings.
**IF YOU NEED FURTHER HELP, feel free to ping me or DM me.**
