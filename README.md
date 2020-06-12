This was about 25% written by keithcurtis, adapted from code written by the Aaron.

This script pulls the contents from a token's GM Notes field. If the token represents a character, you can optionally pull in the Bio or GM notes from the character. The user can decide whether to whisper the notes to the GM or broadcast them to all players. Finally, there is the option to add a footer to notes whispered to the GM. This footer creates a chat button to give the option of sending the notes on to the players.

This script as written is optimized for the D&D 5th Edition by Roll20 sheet, but can be adapted easily suing the Configuration section below.


**Commands:**

**!gmnote** whispers the note to the GM

**!pcnote** sends the note to all players


**Paramaters**

*--token* Pulls notes from the selected token's gm notes field. This is optional. If it is missing, the script assumes --token

*--charnote* Pulls notes from the gm notes field of the character assigned to a token.

*--bio* Pulls notes from the bio field of the character assigned to a token.

*--avatar* Pulls the image from the avatar field of the character assigned to a token.

*--image* Pulls first image from the bio field of the character assigned to a token, if any exists. Otherwise returns notice that no artwork is available

*--help* Displays help.

*--config* Returns a configuration dialog box that allows you to set which sheet's roll template to use, and to toggle the "Send to Players" footer.


**Configuration**

When first installed, Supernotes is configured for the default roll template. It will display a config dialog box at startup that will allow you to choose a roll template based on your character sheet of choice, as well as the option  to toggle whether you want the "Send to Players" footer button to appear.

template = name of roll template, default is 'npcaction'

const title = name of title or name field used by roll template, default is 'rname'

const theText = name of text field used by roll template, default is 'description'

const sendToPlayers = whether to use the "send to players" footer button, default is true


You will need to edit the code of the script to create a custom configuration. The pre-installed sheets are:

Default Template, D&D 5th Edition by Roll20, 5e Shaped, Pathfinder by Roll20 ,Pathfinder Community ,Pathfinder 2e by Roll20 ,Starfinder
