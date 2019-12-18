## Requirements

[Blender 2.8+](https://www.blender.org/)

---

## Physical Starlight and Atmosphere installation instructions

"Physical Starlight and Atmopshere" is only available for purchase on
[Blendermarket](https://blendermarket.com/products/physical-starlight-and-atmosphere) or [Gumroad](https://gumroad.com/l/PSaA).


**1. Download the "physicalStarlightAtmosphere.zip" file.**

To make sure you have the latest .zip, check it here:
[Blendermarket](https://www.blendermarket.com/account/orders) /
[Gumroad](https://gumroad.com/library)


**2a. If you are installing it for the first time:**

- Open Blender.
- Go to Edit/Preferences. 
- Choose "Add-ons" tab and press "Install..." button. 
- Locate the .zip file and press "Install Add-on".
- You will see the newly installed add-on, enable it by checking the checkbox. 
- Wait till it registers. Voila!

**2b. If you are updating to a newer add-on version (or the method above did not work):**

I recommend removing previous version of the addon. For now this is the only option I can assure that addon will work properly. To do that:

- Go to the Blender addons location:

**Windows 7 / 10**

>`C:\Users\{username}\AppData\Roaming\Blender Foundation\Blender\2.XX\scripts\addons` 

**Mac**     

>From Finder in the Go dropdown holding Command key will expand and show Library where you can access the local data of Blender.

>`/Users/{username}/Library/Application Support/Blender/2.XX/scripts/addons`


**Linux:**        

>`~/.config/blender/2.XX/scripts/addons`


- Remove "physicalStarlightAtmosphere" folder.
- Then do the normal Blender addon installation (2a.)

or

- Copy the contents of the .zip to the **/scripts/addons** directory
- Open Blender and enable the add-on. (Edit/Preferences/Add-ons/ search for "atmosphere" - tick the checkbox)


---


### Installation Troubleshooting


**"Physical Starlight and Atmosphere" is not installing!**      

>- Please remove the old addon folder before installing a new version. **(see 2b.)**

>- Do not try to install it on the Blender install directory itself. example - C:\ProgramFiles\Blender Foundation\Blender\2.80\scripts\addons - **NOT HERE (see 2b.)**

>- On Macs, browser (or Finder?) sometimes automatically unzips .zip files. You need to install the .zip file!

**"Physical Starlight and Atmosphere" won't enable!**

>- Try reopening Blender.
>- Check installation. 
>- "Physical Starlight and Atmosphere" only works with Blender 2.8 and above.