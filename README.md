# Google Contacts and Calendar Sync adapters for use with MicroG

This is a Magisk module that contains the required files to be able to sync your Google Contacts and Calendar to your device.

For use with MicroG. WARNING: Compatible only with arm64 devices running Android 12!

# Versions

Taken from [MindTheGapps](https://gitlab.com/MindTheGapps).

- Google Calendar Sync (`com.google.android.syncadapters.calendar`): Version 2021.41.2-406147485-release
- Google Contacts Sync (`com.google.android.syncapadaters.contacts`): Version 12-7567768

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

If you download this repo as zip from GitHub it will be as follows (incorrect and Magisk will throw an error):
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

## Step 3
Reboot your device, and you should have the sync adapters.

## Step 4
Go to settings -> apps -> menu -> Show system

Find Google Calendar Sync and Google Contacts sync, for both, grant the permissions they want. Also enable networking permission (Mobile data & Wi-Fi -> Allow network access).

Reboot your device again. After this you should see the option to sync contacts and calendar when you go to settings -> accounts -> the Google account you added using MicroG.