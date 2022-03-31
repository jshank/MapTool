1. Install BoT per [directions](https://forums.rptools.net/viewtopic.php?f=46&t=28409&p=274496#p274496)
2. Install Elevation per [directions](https://www.youtube.com/watch?v=kbFEi2FyHIc)
3. Select the `Lib:EventMacros` token and then go to the **Selected** window
4. Add a new macro named `ElevationToX` where X is the elevation you want tokens to move to when they step on a specific location
5. Edit the **Command** to be `[h: elevation.stepAndFollowTokens(X)]` again, where X is the elevation you want the token set to
  * You will need to create one of these macros for each elevation in your map that you want to automatically change to
6. Switch to the map you want the triggers on and add a token to the location that should trigger the event. We'll call this the trigger token. It can be any token, I used a simple 100x100 tranparent square I made in GIMP. 
7. Name the Token EventPad XXXXX where XXXXX can be anything you want. I used `EventPad Switch Elevation 0`
8. Select the token you want to use as a trigger and click on **Set Event Pad** on the BoT Macros (click on Bag of Tricks Macros button to show the toolbar)
9. In **Name of associate macro**, select the `ElevationToX` macro you created earlier
10. Check **Token moved onto pad** and click Ok
11. Click **Initialize Pads** on the BoT Macros window and make sure you see your token name show up in the EventPad list for that map
12. Move a player token onto your trigger token and watch the magic!
    
Note that you should have two trigger tokens adjacent to each other along the "path" so that you can easily transition between elevations. I put a trigger token on the stairs for the ElevationTo0 and one a the top of the stairs (landing) for the ElevationTo15