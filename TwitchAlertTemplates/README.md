# Twitch Alert Templates

A set of basic alerts for following, raids, subs, bits, and hosts.

## Special Note

This setup does **not** include any media (images, sounds, music, videos, etc).  Firebot setups do not support exporting media.  However, these templates are more than enough to get you started.

## Contents
* An Event Set called Twitch Events which includes alerts for:
    - New Follower
    - New Subscription
    - New Gift Sub (User)
    - New Gift Sub (Random)
    - Raid Alert
    - Cheer (Bits)
* An Effect Queue

## Customizing

To customize each alert go to Events -> Twitch Alerts -> Locate the alert you want to customize, hit the 3 dots, and Click edit.

This will show you all the effects that are attached to the event.  I provided you with 3 to start:
* Chat - Includes a message such as "Thank you for the subscription, $user!"
* Celebration - This puts confetti on the overlay in Firebot.
* Show Text - This will show text in the overlay about the alert ("$user just subscribed!")

Feel free to edit / remove those as you please, they are just a suggestion :)


If you wanted to add anything else, you would do it here.  For example, if you wanted to add a GIF to an alert, use the steps below to add an effect:

1. Click "+ Add New Effect"
2. Select "Show Image/GIF" in the Effect List
3. On the next panel click "choose file" and find the GIF on your PC.
4. Choose where to display the image on the overlay.
5. Choose your Animations (optional)
6. Add the dimensions of the gif.  They can be bigger or smaller than the actual size of the media. 
7. Set the Duration.  These alerts have been preset with an 8 second duration.  You can change this if you want.
8. Click "Add"
9. Save the Event

The same concept can be applied to other effects, too, such as MP3s, videos, etc.

## Duration Notes
If you are using something like a video or sound file in your alert you have to set duration for *every* effect that is in the overlay (Celebration, Show Text, Show Image/GIF, etc).  This is done by editing each effect and setting the duration there.

You also need to set the "Effects Duration" for the Effects Queue.  This is done by editing your event, and looking at the top of the Effects List (the effects list is the box that has the Chat/Celebration/Show Text, etc).  At the to there is an "Effects Duration" field--Click and and set your duration here, too.

