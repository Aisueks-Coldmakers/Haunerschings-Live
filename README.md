# Haunerschings-Live
a tool wich allows the user to create an Live build of an existing linux installation (WIP)

it will use an customized version from the Distroshare ubuntu Imager to runn on other systems. 
for the system installation we will use the Solus-installer (curently working on it).
it is Planed to also allow an cli instalation BUT curently there is no installer for cli mayby it will the void-installer for the first
the configuration from Haunerschings-Live will run over one or more config files mayby i will create an UI for it 

it is planed to create some own cli tools and other staff for the live system and the building


The building will run in 3 steps.
    1. copy the running linux to "/Hsysbuild/build/livecopy"
    2. migrating special live config files (live user desktop, autologin, ...) from "/Hsysbuild/build/livecopy" also delete files and folder if needed
    3. running scripts in chroot (creating live user, manage SystemD/manage Sysvinit) and building image with "grub-mkrescue"
    
your iso shoud be ready to boot
