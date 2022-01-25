# Chat to Trello Integration
I made this setup so that I can type suggestions for myself for stuff to fix on stream.  Stuff like "I need to remember to add XYZ to OBS" kinda things.

This setup has some more steps than normal, since it requires both a [Trello](https://trello.com/) and [IFTTT](https://ifttt.com) account.

## Setup for Trello
* Log into Trello and create a board that you want the cards to be dumped into. 
* Make a list in that board to receive incoming cards.

## Set up for IFTTT:
* Go to ifttt.com/create
* Click "If This (add)"
* Search for Webhooks and select it
* Choose "Receive a Web Request"
* Create an "Event Name" Trigger (note this name)
* Click "then that"
* Search for Trello, and Login to Trello through IFTTT and authorize the connection.
* Fill out the relevant info (Board, Listname, Position)
* Title = Title of the card (what you see on the Trello on the main screen).  Use {{Value1}}
* Description = What you see when you click the card and see more details. I use {{Value1}} again with {{value2}} as the user and the {{OccurredAt}} to note the time.
* Click Save / Update, and save your Applet.
* Click [this link](https://ifttt.com/maker_webhooks) and then click "Documentation" on that page.  On the documentation page right at the top it'll say "Your key is:" and have a long string of characters.  Copy that key, you will need that.



## Firebot Setup:

When importing the setup file it will ask you for the Event Name and your Webhook Key from IFTTT.

Put those in the fields and that's it!

## Usage

`!remindme add your reminder here`
