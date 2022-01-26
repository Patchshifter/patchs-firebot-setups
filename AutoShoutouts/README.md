# Auto Shoutouts

A setup to automatically shout users out that are part of a specified group.

## Contents
* Effect Queue (Shoutouts) - a queue so shoutouts don't overwrite eachother.
* Event Set (AutoShouts) - The event that triggers the Auto Shoutout
* Preset Effects List (Shoutout) - The actual shout out.  Shows a chat message and shoutout graphic.
* Viewer Role (Auto Shout) - The group that contains the user names of people who will be automatically shouted out.

## Customizing
To edit the **users that get shout outs** go to Viewer Roles and edit the "Auto Shout" group and add / remove users to this group.

To edit what the shoutout says, go to Preset Effect Lists -> Shoutout, and edit the effects there.

The **Chat** effect has the message that displays in chat.  You can customize this, but use the following variables:
* `$presetListArg[user]`  - This is the users name (e.g. `Patchshifter`)
* `$game[$presetListArg[user]]` - This is the game the user was playing (e.g. `Super Mario World`)

You can use these variables to create custom messages.  For example, if I had an auto shout out this message:

`Check out the lovely @$presetListArg[user]  over at https://twitch.tv/$presetListArg[user], they were last playing $game[$presetListArg[user]]!`

For me would return:

`Check out the lovely @Patchshifter  over at https://twitch.tv/patchshifter, they were last playing Super Mario World!`
