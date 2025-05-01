# Microsoft Launcher App Configuration Policy Information

This is my Microsoft Launcher layout for Fully Managed Company Owned Devices

# JSON Configuration Information

## Microsoft Launcher Custom Template

I took the template that you can download from intune when you make a "App Configuration Policy" for "Microsoft Launcher" and structured it to fill "Set Allow-Listed Applications" and "Home Screen App Order" easier

## Microsoft Launcher JSON Structure

These JSON files are structured to

* Set the devices Wallpaper
    + User change disabled
* Enables the M365 Feed
    + User change disabled
* Set the "Home Screen Grid Size" to 5x5
* Define the "Set Allow-Listed Applications"
* Define the "Home Screen App Order"
* Disable the dock
    + User change disabled
* Set’s the search bar at the top of the screen
    + User change disabled
* Home screen web browser
    + Microsoft Launcher Google Chrome sets Google Chrome as the home screen browser
    + Microsoft Launcher Microsoft Edge sets Microsoft Edge as the home screen browser

## Adding the JSON to Intune

To create the Microsoft Launcher App Configuration Policy
1. Navagate to Apps - Android - Configuration
2. Create a "Managed Device" policy
    ##### Basic
        1. Name
            * Enter the Desiered Name
        2. Platform
            * Android Enterprise
        3. Profile Type
            * Select
                + All Profile Types
                + Fully Managed, Dedicated, and Corporate-Owned Work Profile Only
                + Personally-Owned Work Profile Only
        4. Targeted App
            * Microsoft Launcher
    ##### Settings
        1. Configuration Settings
            * Enter JSON data
                + Enter the JSON Data from JSON Configurations or JSON Template
    ##### Assignment
        1. Add desiered Users, Devices, or Groups
    ##### Review + create
        * Review then click create

# Demo Images

## Android Home Screen Application Layout With Microsoft Edge

#### This shows how the Android Phone sets the home screen based on the Microsoft Launcher Configuration - Microsoft Edge file

![Android Home Screen Application Layout](https://ldgithubstorageaccount.blob.core.windows.net/githubimages/Microsoft%20Launcher%20App%20Configuration%20Policy%20Information/Home%20Screen%20Edge%20270%20x%20600.png)

## Android Home Screen Application Layout With Google Chrome

#### This shows how the Android Phone sets the home screen based on the Microsoft Launcher Configuration - Google Chrome file

![Android Home Screen Application Layout](https://ldgithubstorageaccount.blob.core.windows.net/githubimages/Microsoft%20Launcher%20App%20Configuration%20Policy%20Information/Home%20Screen%20Chrome%20270%20x%20600.png)

## MS365 Feed

#### This shows how the Android Phone sets the MS365 Feed when you swipe right

![MS365 Feed](https://ldgithubstorageaccount.blob.core.windows.net/githubimages/Microsoft%20Launcher%20App%20Configuration%20Policy%20Information/M365%20Feed%20270%20x%20600.png)

# App Configuration Policy Links

## Link to the Microsoft Edge App Configuration Policy Referenced

* [Microsoft Edge App Configuration Policy ](https://github.com/Lyric-Duda/Intune-Android-Microsoft-Edge-App-Configuration-Policy)

## Link to the Google Chrome App Configuration Policy Referenced

* [Google Chrome App Configuration Policy ](https://github.com/Lyric-Duda/Intune-Android-Google-Chrome-App-Configuration-Policy)

# Referenced Links

* [Configure Microsoft Launcher](https://learn.microsoft.com/en-us/mem/intune/apps/configure-microsoft-launcher)
* [Standardise Android layouts using Microsoft Launcher](https://letsconfigmgr.com/mem-standardise-android-layouts-using-microsoft-launcher)