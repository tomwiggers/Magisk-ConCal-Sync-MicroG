# Google Contacts and Calendar Sync adapters for use with MicroG

This is a Magisk module that contains the required files to be able to sync your Google Contacts and Calendar to your device.

For use with MicroG.

# Versions

Taken from OpenGApps package.

- Google Backup Transport (`com.google.android.backuptransport`): Version 9
- Google Calendar Sync (`com.google.android.syncadapters.calendar`): Version 6.0.32-246984162-release
- Google Contacts Sync (`com.google.android.syncapadaters.contacts`): Version 10

# How to
## Step 1
Download this git repo, and zip the folders. You cannot download this repo as zip and flash that zip because then the folder structure is incorrect. The zip contents must look like this:
```
ZIP
---> META-INF
---> system
---> module.prop
---> readme.md
```

If you download this repo as zip from Github it will be as follows (incorrect and Magisk will throw an error):
```
ZIP
---> Magisk-Play-Store-Patched-MicroG-master
     ---> META-INF
     ---> system
     ---> module.prop
     ---> README.md
```

## Step 2
When you have the zip, copy it to your phone, and in Magisk manager go to Modules -> tap on the + symbol and select the zip.

## Reboot and
Reboot your device and you should have the sync adapters, however you're not done yet. The next step is to go to settings -> apps -> memu -> Show system

Find Google Backup Transport, Google Calendar Sync and Google Contacts sync, for all three, grant the permissions it wants.

Reboot your device again. After this you should see the option to sync contacts and calendar when you go to settings -> accounts -> the Google account you added using MicroG.