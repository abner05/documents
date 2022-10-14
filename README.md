# documents
# links 
https://nubenetes.com/cheatsheets/#jenkins-cheat-sheet
# Mac 
http://commandlinemac.blogspot.com/2008/12/macports-up-and-running.html
#AWS 
https://tutorialsdojo.com/aws-cheat-sheets-compute-services/
# Devops Tools 
https://hostadvice.com/blog/devops-toolbox-jenkins-ansible-chef-puppet-vagrant-saltstack/

# https://github.com/sk3pp3r/cheat-sheet-pdf/blob/master/pdf/cheatsheet-python-grok.pdf
window update  script 
How to install 20H2 manually:

You need to copy the installer down 

\\sccm.fiservcorp.net\public\

The folder is 20H2_Precache

Copy this onto the users c:\temp folder.


It will take a bit as its over 5 GB.



Once you have downloaded the 20H2 precache you will open up cmd line as admn account and do the following:

1. Navigate to c:\temp\20h2_precache

2. Run this command to make sure there are no blockers, if it runs through without popping up with anything and just closes

then you can move to the next step, if it shows any blockers,  you will need to remediate them IE: non-compatible software/not enough space/ect..

SETUP.EXE /ImageIndex 3 /auto Upgrade /noreboot /DynamicUpdate Disable /compat IgnoreWarning /compat ScanOnly

3. To install it: from the same directory c:\temp\20h2_precache in cmd run this to kick off the install.

SETUP.EXE /ImageIndex 3 /auto Upgrade /DynamicUpdate Disable /compat IgnoreWarning

One of the users screens will turn blue and have a % on it, advise them to save any open work before it gets to 80% as it will do a reboot cycle at 100% automatically. 

The reboot cycle can take up to 20-30 min depending on the machine, tell them to wait for their login to come back up before logging back in.

4. Post update:

Verify the machine updated: either hop back on the machine or have the user do this and send you a snip.

click start, type run, in the runbox type winver and hit enter. It should pop up with a blip showing the version.


Doug Schwebke and Erik Larson are the escalation contacts if manual upgrade does not complete.
