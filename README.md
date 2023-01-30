# MinimalModpackV1
Minimal Minecraft Modpack V1 for personal use.  
Last Updated 1/29/2023

# Installation  

Using ATlauncher:  
Click to "Vanilla Packs"  
Choose Minecraft Version 1.16.5  
Write in a name to remember under "Instance Name"  
For "Loader?" Select "Forge"  
For "Loader Version" use "36.2.34 (Recommended)" 
  
After Installing the instance, you must install the mods.  
Navigate to Instances. Under the newly installed instance select "open folder"  
Put all of the mods from the archive into the mods folder.  
Start the instance back in ATLauncher by pressing "Play" under the instance.  
  
# Fixing Stutters:  
I noticed that I was experiencing stutters while running minecraft.  
These stutters were not caused server-side, so it was likely having to do with garbage collection.  
To fix (at least as far as I've tested) navigate to settings in ATLauncher  
Navigate to Java/Minecraft.  
Use the following user settings:
![java minecraft](https://user-images.githubusercontent.com/71467563/215592084-5d88f020-4f3c-4e36-9c15-b9e1fc51d0e3.png)  
The Java Parameters are:  
-XX:+UseG1GC -Dsun.rmi.dgc.server.gcInterval=2147483646 -XX:+UnlockExperimentalVMOptions -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
