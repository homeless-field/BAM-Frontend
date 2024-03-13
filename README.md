# BAM-Frontend
### [Skip to Set-Up Guide](#set-up-guide)
  The Frontend Code for the BAM! App - Created by the Bellevue College Tech Startup Club, beginning in Winter 2024


# Set-Up Guide
Getting everything set up is not a trivial task. It might take a few hours if you aren't already comfortable with GitHub and VS Code. It's not the easiest thing on the planet, but the best things in life never are. :) This guide only covers Windows 10 and VS Code. For help, feel free to ask in the club's [Discord](https://discord.gg/Dw8dHZEDmu), contact an officer from the club, or contact Ashton Gibson in-person, [on GitHub](https://github.com/homeless-field), or on Discord (@pibto).
### The basic steps are:
1. [Set Up GitHub](#1-set-up-github)
2. [Set Up VS Code](#set-up-vs-code)
3. [Set Up Android Studio](#set-up-android-studio)
4. [Set Up GitHub Desktop](#set-up-github-desktop)
5. [Clone the Demo Repository](#clone-the-demo-repository)
6. [Enable the Flutter Extension](#enable-the-flutter-extension)
7. [Run The Code](#run-the-code)

### 1. Set Up GitHub
The club uses GitHub to host the app's code, so the first thing you'll need to set up is an account. Visit [GitHub's sign-up page](https://github.com/signup) and follow the prompts. Congratulations! You've already completed the first step!

### 2. Set Up VS Code
The first program we'll need to install is VS Code. VS Code is where you'll be actually writing your Flutter code. This type of software is called an IDE, if you want to research some alternatives. To install it, visit their [install page](https://code.visualstudio.com/download), then go to your downloads folder and click the .exe file, and follow the prompts. The process is relatively simple, and you can install it wherever you choose. If you need a visual guide, [this video](https://www.youtube.com/watch?v=HxJXKFxhah4) is helpful.

### 3. Set Up Android Studio
Yes, you'll need Android Studio even if you have an iPhone and/or a Mac. You won't actually be using it, but Flutter needs it for some stuff. If you're technical, you can also install _just_ the Android SDK [here](https://developer.android.com/studio/index.html#command-line-tools-only), but this guide can't help set it up. To begin, visit their [install page](https://developer.android.com/studio), open the .exe, and follow the prompts. Leave the Android SDK component enabled. Install Android Studio wherever you want, but make sure to leave the Android SDK installation location as the default. Also choose the standard install option unless you know what you're doing. Once you're at the screen with options to start a new project or open an existing one, you can close the program and never have to open it again. If you have issues installing Android Studio, they have an [official guide](https://developer.android.com/studio/install).

### 4. Set Up GitHub Desktop
Before installing GitHub Desktop, you'll also need to install Git, a command-line tool. Visit their [install page](https://git-scm.com/download/win), and choose the option for your system. Most likely, that's "64-bit Git for Windows Setup".  Git is a _very_ complex program, so here's my advice:
1. Don't change the install location
2. For the default editor, use Visual Studio Code
3. If you don't know what something means, it's probably best to click Next
     
If you aren't sure about something, [this video](https://www.youtube.com/watch?v=RsNsYvYDyTc) is a quick summary, but there's plenty of resources online to help. To test and see if Git installed correctly press the Windows key and type "cmd", open your command prompt, and type "git" then enter. If you get a response other than "Git is not recognized as an internal or external command", it's installed correctly! Otherwise, it's likely that Git didn't install to your path. [This video](https://www.youtube.com/watch?v=lt9oDAvpG4I) from 1:40 to 3:00 can help to fix that.

And now we can _finally_ install GitHub Desktop itself. This is the last install, I swear! To start, visit their [home page](https://desktop.github.com) and click the install button. From there, open the .exe file and follow the prompts to ensure it's installed where you want. When it's done, launch the program and log in with your GitHub account. For more detail, visit their ["Getting Started" page](https://docs.github.com/en/desktop/overview/getting-started-with-github-desktop).

### 5. Clone the Demo Repository
Until the project's GitHub page (called a repository or repo) is more interesting, we'll be using a demo project and creating a local copy (called a clone) of it on your computer. To begin, go to GitHub Desktop and to File > Clone Repository. Then click URL at the top and copy [https://github.com/homeless-field/FlutterDemo](https://github.com/homeless-field/FlutterDemo) into the textbox, and choose where you want to create the project. Then click Clone. Finally, near the center of your screen there should be an option "Open in Visual Studio Code". Click it, and the project should open in VS Code. There should be a lot of errors, because we haven't finished setting it up yet.

### 6. Enable the Flutter Extension
In VS Code, click File in the top left, then go to File > Preferences > Extensions. Search for "Flutter", and install it. Then restart VS Code. It might ask you to also install the Dart extension. Install that as well and restart again. To ensure the extension installed correctly, go to View > Command Palette, and search for "Flutter: Run Flutter Doctor. The last line of the output should say "exit code 0" and the left-hand column should be all checkmarks.

If they aren't, and your issue is with Android Toolchain, [this page](https://developer.android.com/tools) likely has the solution, although it isn't exactly user-friendly. If VS Code or that page tells you to run something, clicking "TERMINAL" above the output will open a command prompt and you can copy it there.

### 7. Run the Code
This is the big moment! We're gonna run the code! To run it the first time, click "TERMINAL" above the output of Flutter Doctor and type "flutter run". It should ask you to choose a device again, then it should compile and run it! Congratulations!

In the future, if you prefer, you can find the file called "main.dart" in the "lib" folder and select it before just pressing F5. If you use Android and want it to run it on a real device, plug in your phone, enable file access and then enable USB Debugging. [This guide](https://developer.android.com/studio/debug/dev-options) can help with that. Either way, in VS Code go back to View > Command Palette and search for "Flutter: Select Device" and choose which of the available options you want to use. If you set your phone up for USB Debugging, it should be listed here. Congratulations! You can open files on the left and edit the code! Feel free to break stuff - You can always clone the repository again.

If it doesn't compile and run, or you get an error, try going  to View > Command Palette and searching for "Flutter: Run Flutter Doctor" again. Ensure that the left-hand column is all checkmarks, and refer back to step 6 or the guide introduction for help.
