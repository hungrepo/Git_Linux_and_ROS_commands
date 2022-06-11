						Instalations
Google Chrome

wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -

echo 'deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main' | sudo tee /etc/apt/sources.list.d/google-chrome.list

sudo apt-get update 
sudo apt-get install google-chrome-stable
Rotate toolbar
gsettings set com.canonical.Unity.Launcher launcher-position Bottom


Texlive
sudo add-apt-repository ppa:jonathonf/texlive-2017
sudo apt-get update
sudo apt-get install texlive-full

Matlab

sudo sh install
sudo cp libmwservices.so /usr/local/MATLAB/R2016a/bin/glnxa64
cd /usr/local/bin
sudo ./activate_matlab.sh
sudo apt-get install matlab-support (insert the folder /usr/local/MATLAB/R2016a)

sudo wget http://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png -O /usr/share/icons/matlab.png

sudo touch /usr/share/applications/matlab.desktop

sudo gedit /usr/share/applications/matlab.desktop

#!/usr/bin/env xdg-open
[Desktop Entry]
Type=Application
Icon=/usr/share/icons/matlab.png
Name=MATLAB R2014a
Comment=Start MATLAB - The Language of Technical Computing
Exec=matlab -desktop
Categories=Development;

link: https://askubuntu.com/questions/401948/how-to-create-launcher-icon



Linux Command Line
Functions
Command
open a file : 
xdg-open [file]
Search file name: 
ls | grep [file_name]
Remove folder
rm -rf  [file name]
Display all files in a foder
Ls-la

Create a new folder
Mkdir [folder name]
Create a new file
Touch [file name]
Open a text file
Vi [file name with extension]
Move file from this folder to destination folder
Mv [this file] [destination folder]
Copy a file
Cp [file need to copy] [new copied file]
Copy a folder
Cp -r 
Modify the permision of a file
Chmod +x [file name]











