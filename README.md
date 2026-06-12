# Template Repository for Kodi

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/add-ons/repository.template/icon.png)

Created to illustrate a GitHub repository with a simple folder structure linked to a Kodi repository.

Having spent hours creating a repository using templates and other information online, here is a quick and simple template that can be used without running Python scripts.

It assumes little or no knowledge of GitHub and that a GitHub account has been created and logged into.

Simply edit a few files and publish them on GitHub.<br/>Details of the files and their function are provided below.

This method has been successfully used to create both the Magpie Repository and the Template Repository.

Distribution of the Template Repository is permitted.


# Kodi repositories
Kodi repositories contain a number of links to an external repository similar to this one on GitHub. They are usually installed from a source using the 'Install from zip file' method, after the source is added to Kodi by the user.

The external repository contains other add-ons which can then be installed using the 'Install from repository' method.

Checks for updates and their installation are automatic if 'Install updates automatically' is selected in 'System Settings' and 'Auto-update' is selected in 'Add-on information' for each add-on.

For further details see:<br/>https://kodi.wiki/view/Add-on_manager


# Files and folders
Useful for GitHub beginners:<br/>https://docs.github.com/en/repositories/working-with-files

General:<br/>
• .gitignore (optional) - configuration file that specifies intentionally untracked files to ignore by GitHub

• .screenshots (not required) - folder contains images used by this text

• README.md (not required) - contains this text


GitHub Pages:<br/>
Only two files are required to publish a repository zip on GitHub Pages.

• repository zip - published on GitHub Pages<br/>e.g. repository.template-1.0.0.zip

• index.html - contains the name of the repository zip published on GitHub Pages

Access the repository zip by adding the GitHub Pages address as a source in Kodi or view in a browser.<br/>e.g. https://Code-E-Magpie.github.io/repository.template/


Kodi repository:<br/>
Only two files are required to manage the add-ons available (addons.xml) and updates (addons.xml.md5).

• addons.xml - contains the addon.xml file of the repository and each add-on e.g. repository.template and plugin.program.code-e-magpie<br/>

The first two lines and the last one are specific to the addons.xml file. Starting with the repository and leaving a blank line between each, (excluding the first line) paste each addon.xml in the file.

• addons.xml.md5 - created by copying content of addons.xml into the 'String(s)' section of md5 generator https://www.miraclesalad.com/webtools/md5.php and then copying the 'MD5 Hash(es)' into addons.xml.md5

For technical details see:<br/>https://kodi.wiki/view/Add-on_repositories


add-ons folder:<br/>
The add-ons folder contains a separate folder for the repository and each add-on.

Each folder is named using the add-on id e.g. repository.template, plugin.program.code-e-magpie etc.

The folders contain a zip file, an addon.xml file (repository only) and the other assets defined in the addon.xml e.g. icon.png, fanart.jpg etc. 

If an addon.xml specifies assets in a sub folder then the folder structure must be copied in the GitHub repository e.g.

plugin.program.code-e-magpie addon.xml:<br/>resources/media/icon.png 

GitHub repository from top level:<br/>add-ons/plugin.program.code-e-magpie/resources/media/icon.png


# 0. Method choice
To start from scratch use the method below.

Alternatively select 'Use this template' above to create a copy of this GitHub repository and edit or replace the files online. Some of the information in the method below may help.


# 1. Create GitHub repository
Naming the GitHub repository the same as the Kodi repository id has some advantages when using this method.
Kodi repository ids are named repository.xxxxxx

• Log into GitHub

• Click '+' in the top right hand corner and select 'New repository'

• Create a new repository by entering a name in the 'Repository name *' box

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template0.png)

• Once the name has been checked and 'is available' appears, press the 'Create repository' button at the bottom

The other information can be added later if required.


# 2. Create repository zip
• Create the addon.xml, icon.png and fanart.jpg files for the repository

• Click 'uploading an existing file' and follow the prompts

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template1.png)

• Select the addon.xml, icon.png and fanart.jpg files and click 'Commit changes'

• Click 'Create a new release' to create the repository zip and download it


# 3. Create GitHub Pages
Once a file has been uploaded to the GitHub repository, it is then possible to create the publishing 'GitHub Pages'.

• Click 'Settings' at the top and select 'Pages'

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template2.png)

The 'Github Pages' section loads

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template3.png)

• Click 'None' and select 'Main', then to the right of it select 'Root' and then click 'Save'

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template4.png)

• Click 'Code' in the top left hand corner (to exit Github Pages) and then click 'Settings' at the top and select 'Pages' (to reload Github Pages)

This is necessary for the site to go live and the 'Visit site' option to appear.

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template5.png)

• Click 'Visit site' to view the Github Page created<br/>e.g. https://code-e-magpie.github.io/repository.template/

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template6.png)

The Github Page exists but requires content (repository zip) and a configuration file (index.html) for publishing.


# 4. Add GitHub Page files
• Create the index.html file

• Click 'Code' in the top left hand corner 

• Click '+' (between 'Go to file' and 'Code'), select 'Upload files' and follow the prompts

• Select the repository zip and index.html to upload and click 'Commit changes'

Either go to 'Settings' > 'Pages' > 'Visit site' to view the published GitHub Page or enter the address created previously in a web browser<br/>e.g. https://code-e-magpie.github.io/repository.template/

![icon](https://github.com/Code-E-Magpie/repository.template/blob/main/.screenshots/template7.png)

Please note:<br/>Visibility may not be instant due to GitHub processes / server traffic. Clearing cache / refreshing web browser may help.


# 5. Add Kodi repository files
• Create the addons.xml and xml.md5 files for the Kodi repository only

• Click '+' (between 'Go to file' and 'Code'), select 'Upload files' and follow the prompts

• Select the addons.xml and xml.md5 to upload and click 'Commit changes'

• Move addon.xml, icon.png and fanart.jpg files from the top level to add-ons/repository.xxxxxx

• Add another copy of the repository zip to add-ons/repository.xxxxxx


# 6. Install Kodi repository
• Add the Kodi source to view the repository zip in Kodi<br/>e.g. https://Code-E-Magpie.github.io/repository.template/

• Use the "Install from zip file" method to install the repository zip

This will make the repository add-on visible to the repository in Kodi.

Add-on files can now be added:
<br/>• using the method in section '5. Add Kodi repository files'
<br/>• with reference to 'add-ons folder' in 'Files and folders'
<br/>• with reference to the 'Making changes' section below
<br/>• with reference to the original Template Repository


# Making changes
Add a new add-on
<br/>Top level: amend addons.xml and addons.xml.md5
<br/>Add-on folder: add add-on zip and assets defined in addon.xml (icon.png, fanart.jpg etc.)


Change to an add-on (new version)
<br/>Top level: amend addons.xml and addons.xml.md5
<br/>Add-on folder: add new add-on zip (retain old add-on zips) and change assets if required


Change to repository add-on (new version)
<br/>Top level: add new repository zip (delete old one ?), change index.html, amend addons.xml and addons.xml.md5
<br/>Add-on folder: add new repository zip (retain old repository zips) and change addon.xml (change assets if required)


# IMPORTANT
Distribution of Code-E-Magpie addons are NOT permitted.
Code-E-Magpie addons are exclusively distributed via the Magpie Repository and / or Code-E-Magpie on GitHub.

The code and files of these add-ons are free for use, subject to crediting Code-E-Magpie.
