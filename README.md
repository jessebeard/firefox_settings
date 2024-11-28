Update: 27-11-24 Firefox 133.0 broke the animation, so I pushed a fix and updated this readme. 

You'll need Firefox and Tree Style Tabs (TST)[1] installed as well as some of the TST extensions. Here I'm showing "TST indent line"[2] and "TST Bookmark subpanel"[3]
The config file is totally optional and is mostly for personal use, it stores keyboard/mouse shortcuts and tab behavior. 

A little demo of how this mods TST.

*  it minimizes and expands over the web page
*  shows "tab lines" to better show tab hiearchy when expanded 
*  it has an pulsing animation for sound.
*  it has an integrated bookmarks menu, nice because TST takes the place of the bookmarks bar.
![TST_demo](https://github.com/jessebeard/firefox_settings/assets/61173820/d4c457d4-c657-439e-be7e-424a84f6f516)


[1] https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/ 

[2] https://addons.mozilla.org/en-US/firefox/addon/tst-indent-line/

[3] https://addons.mozilla.org/en-US/firefox/addon/tst-bookmarks-subpanel/


### Installation:

Apart from installing TST you will need to conifuge it's `treestyletabs.css`, and the Firefox `userChrome.css` file will need manual configuration/installation. 

3 Steps



1. Firefox requires enabling custom style sheets.
*    In Firefox,  type `about:config` in the address bar. This should bring you to a page asking if you wish to accept the risks of changing these advanced settings. After proceeding,  search for "userprof" and change the `toolkit.legacyUserProfileCustomizations.stylesheets` option to `true`. All done there!

2. Neither the filesystem path nor the stylesheet file exist, so we create both. 
* Go into the options of Firefox (currently the path is to click the Hamburger/ 3 vertical bar button) 
* Click on Help.
* In the Help submenu the current option is called "More troubleshooting information", click on it.
* There you should find a line item in the "Applications Basics" table called "Profile Folder".
* Select the "Open Folder button or browse to the path listed
* At this location in your file system you will need to first create a new Folder/directory called `chrome`
* Inside of it you will put the userChrome.css file. so there should exist .../chrome/userChrome.css
* You can also create the file here, just like you created the folder and copy paste the contents. Just an fyi.
The website https://www.userchrome.org/ is a great resource if you are having trouble at this stage. 

3. install the rest of the theme, you'll need to load the contents of `treestyletabs.css` into TreeStyleTabs in it's options menu.
* Go back to the Firefox options menu
* This time open the "Add-ons and themes" page.
* Then browse to the options tab for the TreeStyleTab Add-on.
* Near the bottom, under the "Advanced" heading near the bottom of the options, there will be a rather large "user style sheet" box, at the bottom there is a text box and a button. Either load the "treestyletab.css" file with that button, or just paste the contents into that box. 

If you wish to install the configuration file, the button for that is all the way at the bottom of this page. Under "Development"  there are three buttons in the "All Configs" Box. Select Import and import the `configs-treestyletab@piro.sakura.ne.jp.json` file. 

That's all. Thank you.

