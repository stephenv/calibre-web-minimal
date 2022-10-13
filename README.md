# About

*Currently work in progress - a stable version is not yet complete*

Calibre-Web-Minimal is fork of Calibre-Web ([version 0.6.19](https://github.com/janeczku/calibre-web/releases/tag/0.6.19)). The user interface and experience has been reimagined for use on iOS devices. It is strongly influenced by Apple Books mobile apps.  \
*This will not be maintained and it is unlikely this project will keep up with any newer released versions of Calibre-Web*

[Calibre-Web](https://github.com/janeczku/calibre-web) is a web app providing a clean interface for browsing, reading and downloading eBooks using a valid [Calibre](https://calibre-ebook.com) database.

![Main screen](https://user-images.githubusercontent.com/1682114/195546719-8e8acc7b-fb36-4fd1-b2b0-7d88c3d4e30b.png)

## Installation

#### Installation via pip
1. To avoid problems with already installed python dependencies, it's recommended to create a virtual environment for Calibre-Web
2. Install Calibre-Web via pip with the command `pip install calibreweb` (Depending on your OS and or distro the command could also be `pip3`). 
3. Optional features can also be installed via pip, please refer to [this page](https://github.com/janeczku/calibre-web/wiki/Dependencies-in-Calibre-Web-Linux-and-Windows) for details 
4. Calibre-Web can be started afterwards by typing `cps` 

#### Steps to complete customization
1. Navigate to "profile" and uncheck "Show Random Books in Detail View"

In the Calibre-Web Wiki there are also examples for: a [manual installation](https://github.com/janeczku/calibre-web/wiki/Manual-installation)

## Quick start

Point your browser to `http://localhost:8083` or `http://localhost:8083/opds` for the OPDS catalog \
Login with default admin login \
Set `Location of Calibre database` to the path of the folder where your Calibre library (metadata.db) lives, push "submit" button \
Optionally a Google Drive can be used to host the calibre library [-> Using Google Drive integration](https://github.com/janeczku/calibre-web/wiki/G-Drive-Setup#using-google-drive-integration) \
Afterwards you can configure your Calibre-Web instance ([Basic Configuration](https://github.com/janeczku/calibre-web/wiki/Configuration#basic-configuration) and [UI Configuration](https://github.com/janeczku/calibre-web/wiki/Configuration#ui-configuration) on admin page)  

#### Default admin login:
*Username:* admin\
*Password:* admin123

## Requirements

python 3.5+


