Project Home: <https://domainmod.org>  
Project Demo: <https://demo.domainmod.org>  
Source Code: <https://domainmod.org/source/>

About
------
DomainMOD is an open source application written in PHP & MySQL used to manage your domains and other internet assets in a central location. DomainMOD also includes a Data Warehouse framework that allows you to import your web server data so that you can view, export, and report on your live data. Currently the Data Warehouse only supports web servers running WHM/cPanel.

Live Demo
----------
Not sure if DomainMOD is what you're looking for? Don't want to take the time to install it only to find out that it's not? We hate when that happens ourselves, which is why we've setup a live demo so you don't waste your time.

So go ahead, take the live demo for a test drive before you install: <https://demo.domainmod.org>

Downloading
-------------
There are currently two options for downloading DomainMOD. Whenever possible we recommend that you use option #2, the git repository download directly from your web server. Not only is it a nice quick install, but it also makes upgrading a breeze.

**NOTE:** Using download option #2 requires that you have git installed on your web server, and that you have access to and know how to use the command line.

**Download Option #1**  
Visit the following URL to download the most up-to-date version of DomainMOD: <https://domainmod.org/download/>

**Download Option #2**  
Use git right from your web server to retrieve the source code. To do so, change to the directory where you want to install DomainMOD and run the following command:

    git clone git://github.com/domainmod/domainmod.git

Installing
---------
If you downloaded the .ZIP file in the previous step, you will now need to upload the archive to your web server and then unpack it into the folder where you wish to install (or unpack it and then upload it, whichever you prefer).

If you used git to retrieve the source code in the previous step, just change to the directory where you ran the git command and your files are already waiting for you in a folder called /domainmod/. Feel free to rename this folder to whatever you want.

**Installation Steps**

1. Create a MySQL database that will be used to store DomainMOD's data.

2. In the '_includes' folder, copy config.SAMPLE.inc.php to config.inc.php and then update config.inc.php to reflect your web server's settings.

3. In a web browser, visit the URL where you just installed DomainMOD, enter the requested information, and then click the Install button. For example, example.com/domainmod/. After a few seconds a message will appear letting you know that the installation was successful.

4. Setup the below cron job on your web server.

Cron Job
---------
DomainMOD includes a Task Scheduler that allows you to run various system jobs at specified times, which helps keep your DomainMOD installation up-to-date and running smoothly, as well as notifies you of important information, such as emailing you to let you know about upcoming Domain & SSL Certificate expirations.

The Task Scheduler is very powerful, and it enables features that you otherwise wouldn't be able to use, but in order for it to function you need to schedule the below cron job to run on your web server. Once the cron job is setup to run the Task Scheduler will be live.

**NOTE:** This file should be executed every 10 minutes.

    Filename: /cron.php

Upgrading
----------
**WARNING:** Before upgrading it's strongly recommended that you make a backup of your DomainMOD installation directory and database. If something goes wrong during the upgrade there may be no way to recover your data, and having a backup of your installation directory and database will allow you to easily restore your previous installation.

**Upgrade Option #1**  
If you installed DomainMOD by downloading the .ZIP file, visit the following URL to download the most up-to-date version: <https://domainmod.org/download/>

Once the download completes, upload and unpack the new archive overtop of where you installed the previous version (or unpack it and then upload it, whichever you prefer).

**Upgrade Option #2**  
If you installed DomainMOD using git right from your web server, just run the following command from within your installation directory to upgrade:

    git pull
    
That's it! Upgrading with git is very easy, which is one of the reasons it's our recommended method for obtaining the DomainMOD source code.

Data Warehouse
-----------------
DomainMOD has a Data Warehouse framework built right into it, which allows you to import the data stored on your web server. Currently the only web servers that are supported are ones that run WHM/cPanel.

If your web server doesn't run WHM/cPanel, or you don't want to import your web server data into DomainMOD, you can ignore this section.

**NOTE:** Importing your web server(s) into the Data Warehouse will not modify any of your other DomainMOD data, nor any of the data on your web server.

**Supported Data**  
The following WHM sections are currently supported, but our end goal is to have every piece of WHM information that can be retrieved via the API stored in the Data Warehouse.

**Accounts**  
Domain, IP Address, Owner, User, Contact Email, Plan, Theme, Shell, Partition, Disk Limit, Disk Usage, Max Addons, Max FTP Accounts, Max Email Lists, Max Parked Domains, Max POP Accounts, Max SQL Accounts, Max Subdomains, Creation Date, Suspend Status, Suspend Reason, Suspend Time, Max Email Per Hour, Failed Email % Before Defer, Min Failed Email # Before Defer

**DNS Zones**  
Zone Filename, Original/Primary Source of Zone Data, Admin Email, Serial #, Refresh, Retry, Expiry, Minimum TTL, Authoritative Name Server

**DNS Records**  
TTL, Class, Type, IP Address, CNAME, Mail Server, Mail Server Priority, TXT Data, Line # of Zone, # of Lines, RAW Data

Support
--------
For the DomainMOD documentation please visit <https://domainmod.org/documentation/>, or access the /documentation/ folder within your DomainMOD installation.

If you have any questions, comments, or bugs to report, please visit <https://domainmod.org/support/>.

Changelog
-----------
Please see the CHANGELOG file that came with DomainMOD, or view the Changelog online at <https://domainmod.org/changelog/>.

License
-------
DomainMOD is an open source domain and internet asset manager.  
Copyright (c) 2010-2016 Greg Chetcuti <greg@chetcuti.com>

DomainMOD is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

DomainMOD is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with DomainMOD. If not, see <http://www.gnu.org/licenses/>.
