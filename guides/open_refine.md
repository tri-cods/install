# OpenRefine

## What it is

OpenRefine is cross-platform, open-source software that allows users to clean and transform messy data. Originally supported by Google, it is now maintained by a large user community. OpenRefine is by no means the only or best way to work with data; however, it strikes an unusual balance between working in proprietary tools for a broad audience (like Microsoft Excel or GoogleSheets) on the one hand, and on the other, straight programming for data science (R Studio, Python Notebooks).

## Why we use it

It allows users to bring in messy data from wide range of formats easily without requiring preliminary transformation. It allows for granular auditing of any changes. It combines (relatively) easy to use suite of features with the ability to write advanced custom scripts when needed. It also allows users to parse with lots and lots of data. Microsoft Excel, for example, has a maximum of 1,048,576 rows by 16,384 columns.

## Installation

**For this workshop we will be using OpenRefine 3.4.1**

If you already have OpenRefine installed in your computer but have an older version, OpenRefine recommends that you backup your working directory (i.e. the folder in your computer where OpenRefine saves projects). If you need to backup your working directory, [follow these instructions](#backing-up).

### Windows

* [click on **Windows Kit** link under OpenRefine 3.4.1](http://openrefine.org/download.html) then download 
* unzip the downloaded `.zip` file then double-click on `openrefine.exe`. (If you’re having issues with the above, try double-clicking on `refine.bat` instead.)
* OpenRefine will open in your web browser

If you are unable to open the program without crashing, [see the instructions below](#user-content-possible-issues-when-installing-openrefine).


### OSX

* [click on **Mac Kit** link under OpenRefine 3.4.1](http://openrefine.org/download.html) then download
* open the downloaded `.dmg` file.
* drag icon into Applications folder
* double click on the icon
* first time you run the program you should receive a dialogue box asking you if you are sure you would like to open it. Here you should click `Open`. 
* OpenRefine will open in your web browser

### Backing-up

It is possible to backup each project individually by opening the project in OpenRefine, then going to the export dropdown menu and selecting export project. 

You can also back-up your directory by making a copy of it manually. You can get to this directory from the OpenRefine start page by clicking on the Browse workspace directory link at 
the bottom left of the page.

#### FYI

**OSX**

The working directory is usually located in `~/Library/Application Support/OpenRefine`

**Windows**

If using Windows, depending on the version you have, the working directory could be located in one of these directories:

* `C:\Documents and Settings\(user id)\Local Settings\Application Data\OpenRefine`
* `C:\Users\(user id)\AppData\Roaming\OpenRefine`
* `C:\Users\(user id)\AppData\Local\OpenRefine`
* `C:\Users\(user id)\OpenRefine`

### Possible issues when installing OpenRefine

**OpenRefine does not start after clicking the .exe, it only opens and closes a window**

For Windows users who are unable to open the program without crashing, you may need to install the [Windows Kit with embedded Java available from the OpenRefine Download page](https://openrefine.org/download.html). And have at least 1 GB of RAM available for it.



