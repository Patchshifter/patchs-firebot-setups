#Simple Death Counter

## Adds the following:
**Commands**
* `!death` - increments the death counter and current death counter by 1
* `!deaths` - Displays the current totals for each.

## Counters
* `Deaths` - Total Deaths across *all* sessions
* `currentDeath` - Death count for *current* session

## Events

* `Reset Death Counter` - This is automatically run when Firebot starts up and will clear the 'currentDeath' counter so it's ready to go for each stream.

## Preset Effect List
* `Death Counter` - This handles all increment/decrementing of the counters

## Customizing

* Go to Firebot -> Counters -> currentDeath and click "Edit."  Edit the chat effect there to customize the text that is displayed when you update the counter (e.g. using `!death+`
* Go to Firebot -> Commands -> `!deaths` and edit this chat effect to customize what is said when you run the `!deaths` command.

## Usage

Use the command `!death+` and it will do its thing.

Use `!deaths` if you want to only display the counters.
