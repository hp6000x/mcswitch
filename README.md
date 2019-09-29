# What is it?

It's a BASH script that switches out softlinks to folders containing minecraft instances, allowing you to, for example, switch between different modpacks using the official Minecraft Java Edition for Linux launcher.

# How do I set it up?

Ten relatively easy steps. Information on how to do the things listed is available with a quick Google :-)

	1. Download the script, remember where you put it. I use $HOME/bin sometimes.
	2. Download the official launcher, run it, launch minecraft and exit
	3. Go to https://files.minecraftforge.net/ and run the installer for the forge version you require
	4. Download the modpack you want to play, by fair means or foul (Either from curseforge, using the twitch launcher on a windows pc or in a VM and copying it, or via multimc)
	5. If you downloaded a .zip file, you'll need to use multimc to get the actual modpack, as you probably have an overrides file, which isn't the complete pack.
	6. Copy the modpack from either the multimc instance folder, or from the folder you got from a Windows PC into
		$HOME/.minecraft
	7. Run the mcswitch script
	8. Choose a name for the instance you created
	9. Select it from the list and click OK to launch.
	10. If you want to create another, run the script, select "Create_Instance", name it and exit the script, then repeat steps 1-9
	
# What do I do next?

Have fun with your new minecraft switcher. Have a look at the code, see how simple it is and what you could do to expand it if you like!
