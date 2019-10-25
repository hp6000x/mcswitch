# What is it?

It's a BASH script that switches out softlinks to folders containing minecraft instances, allowing you to, for example, switch between different modpacks using the official Minecraft Java Edition for Linux launcher.

# Why did you write this when we already have multimc?

I just tried to run the FTB Unstable 1.14.4 modpack and couldn't get it to work in multimc. This seems to be the case with modpacks for minecraft version 1.13 and later. The only way I could get the pack to launch was by using multimc to unpack the downloaded zip and pull in all the mods, then transfer it to an existing minecraft instance, created using the official launcher from http://minecraft.net

# How do I set it up?

(Approximately) Ten relatively easy steps. Information on how to do the things listed is available with a quick Google :-)

0. Install zenity from the repository. If you don't know how to do that, google "How do I install programs in" and the name of your Linux distribution.

1. Download the script, remember where you put it. I use $HOME/bin sometimes.

2. Download the official launcher, run it, launch minecraft and exit

3. Go to https://files.minecraftforge.net/ and run the installer for the forge version you require

4. Download the modpack you want to play: go to https://www.curseforge.com/minecraft/modpacks and find the pack you want, click on it to open its page, click on the "Files" tab, scroll down to "Recent files" and click on the latest version, finally you should see a download link, click it and download the modpack

5. Next, open multimc, create new instance, click on "Import from zip" and navigate to the modpack you downloaded

6. In multimc, choose "Instance Folder" from the right hand side of the main window, then copy everything in the "minecraft" folder to:

	$HOME/.minecraft

7. Run the mcswitch script

8. Choose a name for the instance you created

9. Select it from the list and click OK to launch.

10. If you want to create another, run the script, select "Create New", name it, launch it and exit, then repeat steps 3-9
	
# What do I do next?

Have fun with your new minecraft switcher. Have a look at the code, see how simple it is and what you could do to expand it if you like!
