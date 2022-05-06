## How to get tree style tabs and hide your regular tab bar on Firefox

1.  In a new tab in the url bar, type "about:config"
    - Click "Accept the Risk and Continue"
    - Type in the "Search preference name" bar "toolkit.legacyUserProfileCustomizations.stylesheets"
2.  In the URL bar type "about:support"

    - Scroll to "Project Folder" or "Project Directory" (You can also look it up by using "ctrl + f") and click the "Open Folder" button
    - In the folder that opened copy the "chrome" folder from this repo in there and restart Firefox or create a "chrome" folder if there isn't one already

      - In "chrome" folder make a "userChrome.css" file.
      - In "userChrome" file type:

        ```
        /* hides the native tabs */
        #TabsToolbar { visibility: collapse; }
        /* leaves space for the window buttons */
        #nav-bar { margin-top: -8px; margin-right: 74px; margin-bottom: -4px; }
        ```
