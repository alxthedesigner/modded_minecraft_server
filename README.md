# Setup Modded Minecraft Server with CurseForge Mods
### Minecraft version 1.21.5 on Forge version 55.0.14.
How to create, setup, and connect to your own Minecraft server to use CurseForge mods. To play with mods, everyone on the server must download the Forge client and all the mods that are present on the server. This implementation also uses the NordVPN meshnet so your friends can connect from home.

## **Prerequisites**
Install:
1. ***[The Forge Server and Client Installer](https://maven.minecraftforge.net/net/minecraftforge/forge/1.21.5-55.0.12/forge-1.21.5-55.0.12-installer.jar)*** - Used to connect to the forge server. 
   - Place an empty folder on your desktop. Open the installer and choose server. Place the server in the new folder you just placed on your desktop
   - Open the installer and choose client. The client must be installed wherever launcher_profile.json file is, so find your Minecraft game directory. For PC, follow [these instructions](https://www.wikihow.com/Access-Your-.Minecraft-Folder-on-the-Computer#:~:text=Opening%20Your%20Minecraft%20Folder,Minecraft%20folder%20to%20open%20it.) to find the .minecraft folder. For Mac, this folder is located at ~/Library/Application Support/minecraft.
   - Find the directory with the launcher_profiles.json in it, and install there. If you do not see launcher_profiles.json or keep getting an error looking for the file, open vanilla minecraft to make sure the launcher_profiles.json file generates. Press play and make sure the game loads up to the home screen. Exit vanilla minecraft. Try insructions again.
   - Exit the installer once successful.

2. ***[The Forge App](https://www.curseforge.com/download/app)*** - Used to launch the modded Forge Minecraft. 
   - Open this app and click the “+” to add Minecraft as a game
   - You can either add each mod individally here or drag and drop them into the mods folder, which is also in this guide.

3. ***[Java 21 Installer](https://www.oracle.com/java/technologies/downloads/#jdk21-windows)*** - You need Java 21 to play Minecraft 1.21.5. Java 24 is the latest but too new. Download the installer version and follw the instructions

4. ***[NordVPN Meshnet]()***



## **Setup Minecraft Server**
1. ***Collect all CurseForge Mods on the server*** - Collect all the .jar files of the CurseForge mods you want on your Minecraft server. You then want to drag and drop these files into the Minecraft games directory.
   - Find your Minecraft game directory. For PC, follow these instructions to find the .minecraft folder: https://www.wikihow.com/Access-Your-.Minecraft-Folder-on-the-Computer#:~:text=Opening%20Your%20Minecraft%20Folder,Minecraft%20folder%20to%20open%20it. (For Mac, this folder is located at ~/Library/Application Support/minecraft.)
   - If the mods directory is present, drag all the (unzipped) jar files into the mods folder under .minecraft. If there is no mods folder, create one, then complete this step.

3. After dragging the mods over, return to the Forge app and press play. Click the new Minecraft instance with the Forge name - it's the modded instance of the game.
Load up the home screen again and now you should see all the mods if you press the mods button

4. **If you have a world downloaded from a different server**, move the <world> folder from that instance into this directory. It *must* be named <world>.
  If Java version out of date:
  - Install new Java 21 and enter location into CurseForge settings. Go to Settings > Game Specific > Minecraft > Java Versions. Next to Java 21, paste the Location of your Java 21 JDK.
  Windows Location: C:\Program Files\Java\jdk-21 (if not, add .jdk at the end)
  Mac Location: ~/Library/Java/JavaVirtualMachines/jdk-21.jdk



## **Connect to Minecraft Server**
The friends connecting to your server can also follow these instructions to connect to it.

1. ***[Install the Forge Server and Client Installer](https://maven.minecraftforge.net/net/minecraftforge/forge/1.21.5-55.0.12/forge-1.21.5-55.0.12-installer.jar)*** - Used to connect to the forge server. 
   - Open the installer and choose client. The client must be installed wherever launcher_profile.json file is, so find your Minecraft game directory. For PC, follow [these instructions](https://www.wikihow.com/Access-Your-.Minecraft-Folder-on-the-Computer#:~:text=Opening%20Your%20Minecraft%20Folder,Minecraft%20folder%20to%20open%20it.) to find the .minecraft folder. For Mac, this folder is located at ~/Library/Application Support/minecraft.
   - Find the directory with the launcer_profiles.json in it, and install there.
   - Exit the installer once successful.

2. ***Get same mods present on server (Add Mods)***. To play on a modded server, everyone must download all the mods that are on the server, then add them to the game files. The server owner should have a list of mods you need to download as a client of the server
   - Download all the mods for our server here. If zipped, unzip the zip file with all the mods you downloaded. They should all be .jar files.
   - In the .minecraft folder, find the mods folder. If there is no mods folder, create one, then drag the .jar files into it.  If you created the world in the CurseForge app, the mods folder will be in Instances > the instance you made in Forge

3. ***Connect to VPN with NordVPN Meshnet.*** To connect to the server, you must use a VPN (virtual private network) to connect to the Meshnet that the server host is using
   - Check your email for an invitation from the server host to be a NordVPN external device.
   - You will be asked to download the free app, then to make a free account. They will ask you to choose a plan but DO NOT, just exit out into the app.
   - Once you connect, you should see the server/vpn host's network url that ends with .nord. That is the url you use to connect to the server within the ga,e 

5. ***Connect to the Server in Minecraft***
   - Open Minecraft. Bottom left corner should say Forge and the number of mods available.
   - If using Curse Forge press Play, and on the next screen select the modded Minecraft instance. Press play again.
   - Select multiplayer and click Add a Server. Name it whatever. Paste the .nord server address from the VPN and Join Server.
   - Profit!

