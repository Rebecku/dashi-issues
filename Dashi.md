# What is it?
This is currently in beta so you may experience some bugs - please feel free to report these in the Issues tab in GitHub. (link within the app in the drop down menu)
It is a GW2 dashboard app which consumes the GW2 APIs in order to display things such as:
* your characters and inventories
* your bank items
* your story progress

# Features available now
 ## Dark mode
 You can change the theme of the app to use dark mode if you so prefer. This is accessed by clicking the settings menu drop down and using the toggle switch:
 
![image](https://github.com/Rebecku/dashi-issues/assets/87721142/3cedfd7b-c6e4-4622-b711-883227e31425)

you can switch back to light theme by using the toggle again. Your preference will be stored in localstorage so the preference will persist the next time you load the app.

## Remember API Key
You can tell the app to remember your API Key so you do not need to input it every time by clicking on the settings drop down and checking the "Remember key" option:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/7c862bf5-93ec-47f1-9aed-f597fd59de2b)

This will store your API Key in localstorage. You can click "Remove" to have the app forget your key if you no longer want the app to store it:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/ea060e8c-742b-487e-8e15-c64a68573529)

Be sure to remember to untick the "Remember key" preference if you reset the key, since your preference for remembering it will still be set to true, so untick it to set to false before entering your API key again:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/e49060b8-00bd-4fb4-bafc-9b19fd45dad6)

## Character View
The character view is a dashboard view within the context of a specific character.

Showing:
   - inventory
   - some basic stats
   - equipment
   - story progress

### Inventory
You can search through your characters inventory using the supplied search bar:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/53183365-d20b-4580-bad2-0fc134b14ad4)

The inventory count will update with the search results.

You can hover over an item to see its details and chat link:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/13ebabae-53ad-4906-a842-edae2d47df7a)

The details will display its name and rarity. The background colour reflects the rarity of the item.

Click the chatlink to copy it to clip board so you can paste it in-game:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/ace4b176-6c24-4fd0-9629-4548238e011b)

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/2c42d554-45ba-4cec-9e3d-a5b6637a2b60)


### Equipment
Similar to the Inventory, you can hover over your items to see the details. No search is given in this view since there are only a few items.

### Story Progress

You can view your overall story progress for each story type:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/5abcc90a-1d50-4730-8973-6457654aa12c)

**please note** The "My Story" will not reflect accurately due to there being different paths depending on the answers you gave during char creation, and also depending upon your characters race. These have not been accounted for yet. Also note that if you replay story episodes for achievements etc, sometimes the GW2 API can report incorrectly, and therefore may show as not completed, but really is.

You can click on one of the story bars to see all of the chapters that make up that story, and the completion of each of those chapters:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/51db473c-5f46-430d-8df0-55717c506aa8)

Each chapter can also be drilled into in a similar way:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/e29d7ca2-3dd6-42e0-8a6b-c16688775d14)


## Account View 
Account view is a dashboard view of the overall GW2 account.
Showing:
   - bank
   - wallet

### Bank
Similar to the inventory, the Bank can be searched through using the supplied search bar.
You can also copy the chat link, and see the details when hovering over the item.

### Wallet
The wallet shows all of your various currencies. Hover over an item to see how much of that currency you have:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/a11228b2-8923-4f67-8f46-9511d290b0f6)

**Note** Coin comes back from the API in coppers - some changes will come in soon to convert these into gold, silver and copper appropriately, but currently it will display as copper. For example: 778532 would be 77 gold, 85 silver and 32 copper.



## Map view
The map view does not require an API key to view.
Features:
   - a GW2 interactive map made using leaflet and the GW2 tile service.
   - can place custom markers on map and rename for remembering some cool locations in Tyria
   - can pan to those marker points by clicking the "show me" button when  you drill into the marker item in the right hand side section
   - can import and export custom marker json files.
     
### Custom Markers

You can click anywhere on the map to set a custom marker. You can set a custom name and description by clicking the pencil button on that marker:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/361999ea-ac27-4776-8750-70dd52e4e414)

Markers are stored in localstorage so they will persist between page refreshes.
You can click the "show" buttom to have the map pan to that markers location:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/2af06afd-e48d-4312-8d88-f2418bd4bf3c)

Use the export button to have your markers download to a .json file which you can then share with your friends, where they can then use the import button to import your markers into their instance.
Use the Remove all button to completely wipe all of your custom markers. This is a destructive action and cannot be redone. Backup your markers by exporting them to a json file before clicking, if you want to be able to restore your custom markers.

### Interactive Map
The interactive map is created using the [leaflet.js](https://leafletjs.com/) library and the imagry and data is pulled from the GW2 APIs.
By default waypoints, vistas, points of interest, hero points and hearts will show on the map (plus any custom markers you have).

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/cbf38bc1-2d53-42b4-ac3e-178870ea4182)


You can turn these off / on whenever you want using the menu within the interactive map: 

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/71f2575b-a5df-46f8-8227-777b539ee9b1)

 
# Future Features in the works
* Trading post view
* Display all your dye unlocks
* Mobile optimisation since this is not currently usable and only really works well on larger screens currently.
* ... more
