# AdvancedSamsungVibrationPattern
This is the Documentation how you can create own vibration patterns in ringtones that react to "Sync with ringtone" on OneUI roms.

#How-to

I made this discovery after extracting the /system/media folder of my S22 Ultra.
After that i thought about if we can't just add our own vibration pattern to a sound.
I loaded the ringtone "ACH_Asteroid.ogg" into Audacity and found out, that the Ringtone is actually seperated into 3 different tracks.
2 of which is just the normal ringtone, aka "ACH_Asteroid 1" and "ACH_Asteroid 2".
"ACH_Asteroid 3" is basically just the vibration pattern. 
This is how the structure looks like:
![Structure](https://github.com/JeyKul/AdvancedSamsungVibrationPattern/blob/main/howdoesitlook.jpg?raw=true)

Here is a example of "ACH_Asteroid 3"
![Audio](https://github.com/JeyKul/AdvancedSamsungVibrationPattern/blob/main/vibrationexample.ogg?raw=true)

With that knowledge, we take a look at the metadata of the .ogg file.

![Structure](https://github.com/JeyKul/AdvancedSamsungVibrationPattern/blob/main/metadata.jpg?raw=true)


as you can see here, we have 
> ANDROID_HAPTIC: 1

> ANDROID_LOOP: true

which I assume are very important for this to work.
