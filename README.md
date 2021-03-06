# SmartThings Projects

A repository of my open-source SmartThings projects

## [Google Fit Tile](/smartapps/c99koder/google-fit-tile.src/google-fit-tile.groovy)

A SmartApp that will display your Google Fit steps as a tile.  Requires registering the [Google Fit device handler](/devicetypes/c99koder/google-fit.src) and enabling OAuth2.

Steps to set this up... (based on instructions from mnestor's [GCal-Search SmartApp](https://github.com/mnestor/GCal-Search/))

1. Create a Google Project - https://console.developers.google.com
 - Give it any name
 - Enable the Fitness API - https://console.developers.google.com/apis/library
 - Setup new credentials - https://console.developers.google.com/apis/credentials
 - Enable OAuth with a redirect URI of: ```https://graph.api.smartthings.com/oauth/callback```
 - Copy the Client ID and Client Secret, you will need these later
2. Install the [Google Fit Tile](/smartapps/c99koder/google-fit-tile.src/google-fit-tile.groovy) SmartApp
 - https://graph.api.smartthings.com/ide/app/create
 - Enable OAuth for "Google Fit Tile"
 - Put the ClientID and Client Secret you copied from Step 1 into the Settings for "Google Fit Tile"
 - Publish the App
3. Install and Publish the [Device Type](/devicetypes/c99koder/google-fit.src)
 - https://graph.api.smartthings.com/ide/device/create

Open the ST app on your phone and install the "Google Fit Tile" app.
This will walk you through connecting to Google and setting a steps goal.

![Screenshot](/smartapps/c99koder/google-fit-tile.src/Screenshot_20161107-153736.png)

## [Steps Reminder](/smartapps/c99koder/steps-reminder.src/steps-reminder.groovy)

A SmartApp that will send you a push notification if you haven't reached a specific step count at the specified time

![Screenshot](/smartapps/c99koder/steps-reminder.src/Screenshot_20161106-140629.png)

# License

Copyright 2016 Sam Steele

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
