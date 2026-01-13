# Card Filterer
This is a program that allows you to filter your cards from any card game you enjoy. Instead of having to comb through by hand and find ones matching what you are looking for, throw all the data in here, and the program will take care of it for you!

# Purpose/Value
The main purpose of this is to save you time. Depending on how thoroughly you wish to sort your cards, you could spend a long while sifting through. It is also easy to make errors depending on the cards you are looking at. If you were to have 3 decks of classic playing cards, and are sorting by suit, misreading a card once could lead to placing a diamond in the hearts or vice-versa. This tool aims to eliminate that possibility, and heavily speed up the process simultaneously.

# Capabilities
This can take in data in a number of forms. tsv, csv, xlsx, ods, json, dat, and txt are all supported. You can upload said data through the GUI or as a command-line argument on launch. You can also manually input information, either as a new set of data, or to add onto an existing set if you forgot to add a card, for example. Data input can contain the following attributes:

| Data | Data Type | Use |
| --- | --- | --- |
| Name | String | The name of the card |
| Description | String | The description of the card |
| Image | Varies | An image of the card |
| Color (optional) | String | The color of the card |
| Value (optional) | int | The value of the card |
| Weight (optional) | float | Weight for priority sorting |
| Number (optional) | int | The number of the card |

# Features
Within the GUI, you can create and swap between multiple different decks, for multiple games or multiple decks within the same game. Creating groups allows even further sorting from here.

## sort(criteria) - GUI & command-line
-Input data from the table above in the order you want it to be sorted in. You can also leave out data pieces that are irrelevant (skipping weight as it is optional). It will automatically sort the data in the order of the data. sort(name, value) would go alphabetically, then numerically, for example. 

## filter(criteria) - GUI & command-line
-Input multiple criteria to filter out only based on that criteria. Entering "color" would provide only cards with a color applied.

## filter(criteria, match) - GUI & command-line
-Input a criteria, and matches within that criteria. Entering "title, 'pokemon'" would provide only cards with pokemon in the title.

## remove(name) - GUI
-Input the name of a card to remove it from your library. This is usable in the GUI only, as it auto-provides the name on click, to ensure there is no accidental deletion of a card from a typo, or misremembering the name of a card.

# Technologies
This program uses Python, C and C++ as its languages. It uses several Python libraries, most notably the external library *library*. Within C & C++, it sticks to the standard, built-in ones, and no external ones are used. 

# Usage
This program is usable on Windows, Mac, and Linux. It can be run through the command-line, but the GUI is recommended and has more features. 

# Outreach
This program is intended for those who utilize digital decks of cards for trading games, and often want to check if they own a certain type, how many of a type they own, etc. The idea is to streamline it all into one interface. It isn't for everyone, due to needing to upload all the data initially potentially using much more time then they'd spend just checking themselves. But for someone with hundreds of cards that frequently adds to them or needs to do checks, this program can be a great initial cost that provides numerous benefits.
