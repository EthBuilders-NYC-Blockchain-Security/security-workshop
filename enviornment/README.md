# Environment setup for parrot linux
- The purpose of this documentation is to create a virtualbox and setup a linux environment where people can safely test their environment in linux without issues. 

## Requirements:
1. https://www.virtualbox.org/
- virtual environment 
2. https://www.virtualbox.org/wiki/Downloads
- Download: virtualbox-ext-pack
3. https://www.parrotsec.org/download/
- Parrot linux is meant for security. It's lighter than kali linux and easier to setup. 

## Instructions
1. Download virtual box
2. Go to parrotsec.org/download
3. Click "Get security edition"
4. Download MATE desktop (Don't get torrent)
5. Next go back to virtualbox 
6. Click "New" and a screen will show up
7. Fill out the "Create Virtual Machine":
    - Name: Parrot Security
    - Machine Folder: <default>
    - Type: Linux
    - Version: Other Linux (64.bit)
8. Click how much resources of memory you would want into this virtualbox. Make sure it's enough to even use the machine. 
9. Leave hard disk on default setting: Create virtual hard disk now
10. Click create
11. Confirm file location
12. File size: 20gb
13. Select VDI
14. Make sure the virtualbox is Dynmically allocated
15. Click "Create"
#### NOTE this will create just the machine. Next we will upload the linux image

1. Click settings
2. Go to general
3. Go to the "advanced" tab
4. Click the shared clipboard and drag n drop then put "bidirectional" for both
5. Next go to "system on the left side of the panel
6. Adjust the amount of RAM inside the machine
7. Go to "Processor" tab
8. Click at least up to 2 CPU 
9. Click "Enable PAE/NX
10. Next click on "Display" on the left side of the panel
11. Adjust the amount of resources that will display. Suggestion: 90mb
12. Next click on "Storage" on the left side of the panel
13. Go to "Controller: IDE" (there should be an empty CD icon)
14. Click the empty CD icon
15. Go to where you downloaded the parrot linux ISO
16. Next click on "Network" and make sure Enable Network Adapter is on and it's attached to NAT
17. Next click on "USB" on the left side of the panel
18. -- Note -- If you installed the virtualbox-ext-pack then you can select "USB 3.0 (xHCI) Controller
19. Next Click on "Finsh"

#### NOTE This just uploaded the image, now we have to install the image onto the virtualbox

1. Click on "Parrot Linux"
2. The image should start up and click "Try/install"
3. The default image will appear 
4. Click "Install Parrot" icon
5. Click default language
6. Click next
7. Configure location
8. Click next
9. Leave default settings, click next
10. Select "Erase Disk"
11. Select Swap (with hibernate)
12. -- Note -- If you want to encrypt then add a passphrase
13. Click next
14. Fill out your user
15. Click next
16. Review the summary
17. Click "install"