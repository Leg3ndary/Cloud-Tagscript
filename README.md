# Cloud-Tagscript

This is a tutorial of how I made the [Shell Tag](https://discord.com/channels/186980582863929345/474346837352906752/847923391758991382)

[Repl Link](https://replit.com/@TenshiBot/leg3ndarytagscript#main.py)

## The Problem

Carl-bot offers a very unique and interesting language called tagscript, however, one of the major downsides of it, is you currently have no way to save data in an efficient, secure way. 

To save data you have in a sense 2 options in Tagscript:

1. Saving users nicknames
    - Doesn't work unless you either ping an alt user or have a user continuously run the command for you
    - Takes up a command block that has to edit a user nickname
    - The data is publicly available
    - Limited to 32 characters
2. Using a role colour and changing its value
    - Limited to the same permissions as no 1
    - Information is in a sense also publicly available
    - Limited to 6 characters that are case insensitive and can only have 0-9 with no emojis
    - Also uses a command block

In essence, you really cannot desirably save data...

So how do we work around this?

Here's a solution I propose:

1. User sends !help
2. Carl now makes an embed with an image from a url like so [Image](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/Picture_icon_BLACK.svg/1200px-Picture_icon_BLACK.svg.png)
3. Before carl sends it discord requests the image url
4. Discord sends the embed Carl requested with the image url

## Pros/Cons

Everything has its pros and cons, I'll explain them here and now.

Pros:

1. Can be called (Maybe) the best way of storing info in Tagscript
2. Can hold much more data then other ways
    - This is limited to 512 mb through my method (If you don't want to spend money...)
3. Not as secure but is still better then others
4. No command blocks needed
5. Very flexible!

Cons:

1. Not 100% secure
2. Requires a lot more work (It took me a week to work through everything with almost no prior knowledge... I'd say it would now take me around a day now, but thats still a lot)
