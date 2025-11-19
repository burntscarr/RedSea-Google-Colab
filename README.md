# RedSea for Google Colaboratory (Colab)

## Info
This is based off the version found at [Dniel97's GitHub](https://github.com/Dniel97/redsea)
It is updated to use [my own fork of redsea](https://github.com/burntscarr/redsea)

It is made to work with [Google Colaboratory](https://colab.google.com/) and download Tidal tracks into your [Google Drive](https://drive.google.com/)

You will need access to a Google account to use this project. You can create one by visiting the [GMail Website](https://www.gmail.com/) if you don't already have one.

When you're ready, open the .ipynb file [located in RedSea/RedSea.ipynb]([https://github.com/burntscarr/RedSea/blob/main/RedSea.ipynb](https://github.com/burntscarr/RedSea-Google-Colab/blob/main/RedSea.ipynb) and click the link up top.

## Begin Setup
* Open [the Colab Notebook](https://colab.research.google.com/github/burntscarr/RedSea-Google-Colab/blob/main/RedSea.ipynb) - If you have multiple Google Accounts, choose the one you want to use from the top right (profile picture area).
* Run the steps in order:
1. Import Google Drive - click play, click the link in the output box, choose account if multiple, scroll down, click allow, copy code into input box on colab project.
2. This command is to change the directory into your Google Drive. Normally Colab stores content in /content/ so you want to be connected to you GDrive to be able to get the files you're downloading with RedSea.
3. This is an optional command I added for people who have issues with "could not stat x" - Remove the # before ls to list the files in the directory you're in. This helps to solve typos such as when the MyDrive folder is named "My Drive" with a space.
4. This command is to install the required packages with the apt package manager. - If any node errors occure that's fine. Colab has a few default packages that are meant to stay at a specific version, but they'll still work with RedSea.
5. This command is to clone the [RedSea project from my own fork](https://github.com/burntscarr/redsea) into a folder in the current directory which, from command 2, is your GDrive root.
6. Assuming you were still in the GDrive root, this command will move you into the RedSea folder called redsea.
7. This command uses Python's Package Installer to install a few packages that RedSea also needs to run. Similar to step 4, except these are python packages.
8. Multiple commands here, first we go into the captcha directory, this directory is meant for installing the code for re-captcha that only runs on Desktop terminals, and won't work with Colab. Still, it should be ran anyway. Then we run the code.
9. Multiple commands here, first we go to the config directory, this directory contains your settings. Then we change the filename so it is the right one that RedSea looks for.
10. Finally, we're starting to USE the program. Here, we're adding a session and authorizing it. You'll want to select TV, which is ```t``` then press enter. Next it prompts you to login, do so, and it should prompt Session Saved!
11. And here, we're actually putting the program to use. Just enter the Tidal URL you want to use and you're good to go! Since you've only got one auth session, no need to choose one.
    

## What's next?
I'm still working on a few things, but here's some extra info for you.
* You can find your files in your Google Drive in the redsea folder then the downloads folder. (Drive/redsea/downloads) There should be a folder per link you entered named after the content.
* You can download Tracks, Albums, Playlists, Music Videos and Dolby Atmos all with your TV session!

## Customization
Advanced users can edit options for naming/path/metadata and more found in settings.py
