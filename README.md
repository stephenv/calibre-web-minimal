# About

*Currently work in progress - a stable version is not yet complete*

Calibre-Web-Minimal is a fork of Calibre-Web ([version 0.6.24](https://github.com/janeczku/calibre-web/releases/tag/0.6.24)). The user interface and experience has been reimagined for use on iOS devices and is strongly influenced by 'Apple Books'.

[Calibre-Web](https://github.com/janeczku/calibre-web) is a web app providing a clean interface for browsing, reading and downloading eBooks using a valid [Calibre](https://calibre-ebook.com) database.

*This fork is my customization of Calibre-Web for my personal use and likely (1) will not be maintained and (2) not keep up with any newer released versions of Calibre-Web. Use at your own risk.*

![Main screen](https://user-images.githubusercontent.com/1682114/195546719-8e8acc7b-fb36-4fd1-b2b0-7d88c3d4e30b.png)

## What's New in This Version

- **Updated to latest Calibre-Web** - Includes all recent features and security updates
- **iOS/Apple Books UI** - Custom styling optimized for iOS devices
- **Dropdown sorting** - Clean dropdown menu instead of button grid
- **Mobile-responsive design** - Optimized for touch interfaces
- **Flask-Login compatibility** - Updated for latest Flask-Login API
- **Enhanced security** - Latest dependency updates and security patches

## Installation

#### Manual installation from source

This fork must be manually installed ("from source") following the procedure below. For Windows pip and venv come with the basic installation. On Windows, the python binary can be found after installing the virtual environment under .\venv\script\python3.exe

1. Make sure you have installed pip and also venv for your python version. If missing, install it by the package manager of your distribution (e.g., apt for debian like distributions)

    - `sudo apt install python3-pip python3-venv`

2. Go to the folder where you want to install Calibre-Web-Minimal, e.g., `/opt/calibre-web-minimal `

3. Create virtual environment for calibre web in folder venv 
    - `python3 -m venv venv`

4. Install dependencies by running `./venv/bin/python3 -m pip install -r requirements.txt`

5. Download and extract Calibre-Web-Minimal into the current folder (in this example /opt/calibre-web-minimal)

6. Execute the command: `./venv/bin/python3 cps.py` (or `nohup ./venv/bin/python3 cps.py` - recommended if you want to exit the terminal window)

Issues with Ubuntu:
Please note that running the above install command can fail on some versions of Ubuntu, saying `"can't combine user with prefix"`. This is a [known bug](https://github.com/pypa/pip/issues/3826) and can be remedied by using the command `./venv/bin/python3 -m pip install --system -r requirements.txt` instead.

Remark: All config files (settings database, log files) are stored in Calibre-Web root page (in this example /opt/calibre-web-minimal). Additional config files, such as the config files for gdrive and gmail have to be placed there too.

#### Steps to complete customization
1. Navigate to "profile" and uncheck "Show Random Books in Detail View"

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

python 3.7+ (updated from 3.5+ to match latest Calibre-Web requirements)
