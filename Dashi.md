# Dashi - a GW2 Companion app.
Dashi is a Guild Wars 2 companion app which consumes data from the official GW2 API's.
Use your API key created from the official GW2 website (in Account Settings) in order to view information about your account. Different permissions are required for different tiles, so be sure to grant the ones you want in order to be able to see that information. If your key does not have the required permissions, tiles that require it will tell you so.
Your Account information is not stored in any servers and is only stored on the client side.

Dashi is still under development so bugs may be present. Please feel free to report any issues you experience within the Issues tab and these will be addressed when time permits.

## Features
The full feature list is still a work-in-progress with many more to be added in the future. You can submit feature requests via the Issues tab.

### Character View
The character view shows information at an individual character level. You can use the drop down to swap between your characters to view the following information:
* Character's Equipment with item chat link
* Character's Inventory with search and item chat link
* Story Progress for that character with drilldown
* Character stats (death, birthday, level, age)

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/6d1f1d1e-0307-43af-b1af-140c708ddc0d)

#### Inventory Search
Type in the search box to search over your characters inventory and narrow down results:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/fe2b59dc-73b7-4b0a-ab2b-279cc81c8b5c)


#### Item details
hover over an item with your mouse to view its details, as well as to see the in game chat link which can be copied with a click:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/bead4fd6-432f-497c-be6b-45dc09c636c5)


#### Story Progress Drilldown

click an expansion / season to drill down into the individual episodes to see which ones your character has completed. Click an episode to see the chapters that make it up, and your progress with those:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/41a9fb39-64bb-48d8-b1c9-aec57dfd984d)


### Account View
The account view shows account level information such as :
* Bank inventory with search and item chat link
* Wallet
* Gold count
* Mount skin unlocks
* Outfit unlocks

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/777a36e6-ac01-44cc-aef3-c35311c08938)


### Map View
Map view gives you an interactive GW2 Map (data provided from the official GW2 map service APIs). This view does not require any API key to work, so you can use Map View without supplying any API Key.
Features available in Map View:
* Custom Markers
* Options to toggle visibility of waypoints, hearts, points of interest, map borders, region boarders.
* Ability to import and export your custom markers in a .json file for sharing with friends or backing up. Custom Markers are stored in client side local storage and not on the server side so if you remove them from your client they will be removed from everywhere. Be sure to back them up if you don't want to lose them after a browser clear cache etc!
* Pan to marker

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/196dfeab-620e-4c60-bb14-9f629c9c8edc)

#### Custom Markers
Once the map data has all loaded in (blurred when loading) you can then set a custom marker by clicking anywhere on the map. You can then view these markers by clicking the marker button on the left hand side:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/288190cd-2c18-4ee5-9aa0-3369feb06b01)

Open a marker to see the description given, and for the option to pan to that marker:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/c5863899-25f8-4dde-9843-f77481cbca73)

Use the location button to pan to that custom marker on the map. Use the note button to edit the details of that custom marker.

To remove a marker, pan to it and then click on the marker. To remove all markers at once, use the Bin all option. This is a destructive action and will delete ALL your custom markers.

Use the Export button to export all your custom markers into a .json file which can then be shared with your friends, or used as a backup in case you lose your markers.
Use the Import button to import an exported .json file such as your friends, to import their markers. This will not remove your markers, but will add the markers into your collection.



### Trading View
The trading view gives information around the trading post:
* Items / gold currently waiting for you to pick up
* Your pending sell transactions which have been listed for sale along with how much for, and when it was listed.

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/1f49aabc-c684-4993-83b3-60b04c98d540)

#### Waiting for pickup
Items waiting for pickup will show in this tile:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/c8627da6-09d6-473a-bfde-c9a0071362e7)

#### Pending Sell Transactions
Your pending sell transactions will show up like so:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/38b45bb4-ab17-4629-b196-024c469350de)


### App features
* Dark theme / light theme toggle. Switch between the two at your pleasure using the toggle in the popout nav bar.
* Option to remember your API key so you don't need to paste everytime. This is only ever stored in your browers local storage until you clear it via browser cache or using the Delete API key option.
* Delete API key - use this to swap to a different API key and remove any remembering of the key you used. Any key previously remembered will be cleared from local storage and session storage.
* Ability to generate a new sub API Key from your key. You can use this to select specific permissions and an expiry date for the key to give to your friends so they can view your stats that you allow. (your custom map notes will not show as these are only ever stored on your browser client's local storage. You will need to export these if you want to share them, for your friend to import).
* Links to various sites such as the official GW2 wiki, the official event timers site and this github issues tab for reporting any bugs or submitting feature requests.

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/67ae1028-2ea1-4b70-b841-a34ac6e60d40)

#### Dark theme / light theme toggle
Use the toggle to swap between light theme and dark theme whenever you want:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/e36789a4-33f0-4d02-8151-50d007af517d)

#### Generating a sub key
Select the permissions you wish to grant the key, and an expiry date to create a sub key. The key will be copied to your clipboard when you click create:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/1deb252c-96f0-4034-acb8-a64c03e2a040)

any subkeys created will no longer work when its parent key (the key you were logged in with when you created one) expires or is deleted. The sub key cannot have more permissions than its parent, only the same or less. Permission options will vary depending on which options were granted to the parent key.


### Viewing on Mobile
#### Dropdown menu in mobile view
the popout menu will change to a dropdown one when viewed on smaller screens such as mobile.
![image](https://github.com/Rebecku/dashi-issues/assets/87721142/32c96408-bb74-4ae9-a715-815bd769308e)

#### Map view in mobile
![image](https://github.com/Rebecku/dashi-issues/assets/87721142/b4330bbb-09e4-4295-8a12-76ad100bdebf)

#### Map custom markers in mobile

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/64231581-e175-4a0b-9768-7007078d7cbc)

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/b7c3b04c-efd2-4fbf-adf2-ad778219b551)


#### Dashboard layout
The dashboard layout will change depending on the screen size. On mobile tiles will be arranged in a single column:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/07d0d098-e6b4-45c8-bba9-a29f967b952d)

#### Item Information
clicking an item will bring up its information in a modal instead of a popover in smaller screens:

![image](https://github.com/Rebecku/dashi-issues/assets/87721142/7e62f8a5-1bb2-4b38-a7b4-e01acced3948)

## Upcoming Features
There are still a lot of features we want to add to Dashi. These features include, but are not limited to:

* Crafting view
* Best Route Map feature
* Main cities / hub areas in map listed for easy navigation
* Multi-Character inventory view, search across ALL characters inventories without having to swap through the different characters
* Dye unlocks
* Event Timer Markers in map view so you can easily copy waypoint chat links and see where the events are happening and when

# Known Issues
* Custom markers import / export on mobile does not work

