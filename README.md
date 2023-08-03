# GradleMCP
A simple to setup workspace to use mcp with Gradle.

Linux: Yes, tested.

MacOS: Yes, tested.

Windows: Yes, tested.

Supported versions:

1.8.8

# How to setup #

This may seem like a lot but trust me it isn't it takes like a minute to setup (Besides decompile time and such)

Step 1: Make a new folder on your desktop call it anything you want, preferably your client name.

Step 2: Download or git clone this repository in that folder

Step 3: Remove everything except the contents inside of the '1.8.8' folder. So you should end up with your client folder, with 3 files. (build.gradle, BuildProject.sh/bat, CompileClient.sh/bat)

# Windows Users #

Step 4: Run BuildProject.bat

# Linux/Mac users only #

Step 4: Open the folder in terminal and type "chmod +x BuildProject.sh" and hit enter

Step 5: Type in the terminal "./BuildProject.sh" and hit enter.

# Now sit back and wait till the decompile is done #

Step 6: You will be prompted with the question "Would you like to install optifine aswell? [y/n] type in 'y' for yes or 'n' for no.

# Now GradleMCP is completed #

Step 7: Open up IntelliJ IDEA and open the project folder.
Step 8: If asked if you trust the folder select Trust.

# Now we configure intelliJ #

Go to build.gradle:

Now we need to add a run configuration:
Expand "src" -> "main" -> "java" and click on "Start.java"
To the left you should see a small green arrow, just click that.

You will get an error this is how to fix:

Click on the drop down box right by the green hammer (top right corner) and click on "Edit Configurations".

Press "Modify Options" and tick "Add VM Options"

Then in "VM options: ", put "-Djava.library.path=versions/1.8.8/1.8.8-natives/". This is linking the native libraries.

Then you will see "Working directory: " then a textbox with a file path in it, just add a /.minecraft at the end of it.
"/home/hippo/Desktop/GradleMCP" will become "/home/hippo/Desktop/GradleMCP/.minecraft"

Now just click apply then ok.

Now you are done! Just click the green arrow right by the dropdown box then start coding away.




# How to compile #

# Linux Users / Mac Users #

Step 1: Open your client folder with terminal and type "chmod +x CompileClient.sh"

Step 2: Type in the terminal "./CompileClient.sh"

# Windows Users #

Step 1 : Run CompileClient.bat

_________________________________________________________________________________

Step 3: Sit back and wait for the message "Please enter a client name and version (example: Client v1):" then you will enter your client name and (optional) version.

Step 4: You will see a new folder which would be named your client name you just entered, and that is your client compiled! Just put it in your .minecraft and you are done. (And obfuscate the jar if you want)
