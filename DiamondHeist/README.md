# Diamond Heist

Diamond Heist is a mini-game I created for my channel that pits chat vs the mods/VIPs for a chance to get a Diamond (VIP badge)!

When the effect is run it basically checks if the user is a mod/vip, or if they are the current holder of the diamond, or if the diamond is in the vault, and makes decisions accordingly.

Firebot will automatically handle the actions of making / unmaking VIPs for the game.

## What it Adds
* Commands: `!diamond` will respond with what user has the diamond, if any.
* Preset Effect Lists: `Diamond Heist` is the main "meat" of the set up, this is what handles all the work.
* Viewer Roles: `Diamond Exceptions` is a viewer role to use for users who are exempt from getting their VIP taken away, aka your "real" VIPs.  Put all your VIPs in this group, otherwise if they redeem it, their actual VIP badge will be taken away.

## Usage

This was intended to be a channel reward, but in theory you can have it in a command too, but the idea is the same.

Create a channel reward in Firebot and add an Effect to "Run Effect List" and choose the Diamond Heist Preset Effect List

## Caveats

There are some quirks with this to keep in mind:
* You have to de-VIP who has the Diamond (if any) when you end stream, otherwise that person will be a VIP and the game kind of messes up
* If you want to avoid the above you can go to Settings -> Advanced -> Persist Custom Variables -> On.  If this is set Firebot will save the person between stream sessions. 

## Customizing

If you want to customize any of the responses you can go into the Preset Effect Lists tab and edit the Diamond Heist list.

Edit the "Conditional Effects" effect in the Diamond Heist and we can start drilling down into what we can change.  All of the text responses are in "Run Random Effects" in the effects here.

For example, if you wanted to change what it says when a mod takes the diamond back, you would follow these steps:

Diamond Heist Preset Effect List > Edit Conditional Effects > If (Moderator / Real VIP Exclusion) -> Edit Conditional Effects -> Otherwise -> Edit Run Random Effect -> Chat effects

All of those chat effects can be changed / removed or added to.

There are a bunch of places to edit them, so dig around those conditional effects and check them out!
