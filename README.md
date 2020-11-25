# Un-sign Microsoft Teams Application to re-enable virtual webcams

Recent Microsoft Teams Builds have broken support for Virtual webcams.  Aparently this is due to security and
interaction with unsigned webcam drivers.

A solution can be found here: https://answers.microsoft.com/en-us/msteams/forum/all/microsoft-teams-mac-os-client-is-not-recognizing/d9e863be-d9a4-4d03-a4b8-1b5c7df58828
Microsoft information here: https://docs.microsoft.com/en-gb/microsoftteams/troubleshoot/teams-on-mac/virtual-camera-doesnt-work-macos

You can vote for a proper fix here: https://microsoftteams.uservoice.com/forums/908686-bug-reports/suggestions/40961347-latest-teams-update-breaks-virtual-cameras-micro

The script in this repo automates the process, and acts as documentation for me.
- After un-signeing the apps you'll need to give the unsigned app permission to access yor keychain, and to access the cameras and microphone (it'll ask).  For me it didn't ask to re-enable screen recording (needed for the screen sharing feature).  I had to close the app, go to System PreferenceSecurity&Privacy->Privary(tab)->Screen Recording, disable and re-enable Miscrosoft Teams and then re-start the teams application.
