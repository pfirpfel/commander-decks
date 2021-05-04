# My commander deck lists
My deck list collection for the Magic: The Gathering [Commander format][edh].

In the **paper** folder, you'll find all my current and past paper commander decks.

The **online** folder consists of all the commander deck lists I play on [Magic: The Gathering Online (MTGO)][mtgo].


# Working with the repo

## Installation
`npm install` (requires NodeJS)

## Checking format of deck lists
`npm test`

## Format single deck list
`npm run format online/list.txt`

## Format all deck lists
`npm run format-all`

## Add or update a deck list from MTGO
In MTGO right-click a deck to export it. Choose the txt format and save it to the correct folder in this project.
To update an existing deck list in this repo, just overwrite it.
Avoid file names with white space or special characters in them.

Then, run the format deck command (either for all or just this particular list) from the instructions above.
The new or changed deck list is now ready to be commited using Git. If the deck list is not properly formatted,
the git pre-commit hook will prevent it from being commited.

Example:
1. Add new list at online/Foobar.txt
2. Format the deck: `npm run format online/Foobar.txt`
3. Add to git repo: `git add online/Foobar.txt`
4. Commit the deck: `git commit -m "Adding new Foobar deck"`

# License
This work is licensed under a [Creative Commons Attribution 4.0 International License][cc-by].

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[edh]: https://magic.wizards.com/en/content/commander-format
[mtgo]: https://magic.wizards.com/en/mtgo
