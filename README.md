# Marshmellow-Tagscript

**Warning** this is a complicated (semi) idea in tagscript and without a very good understanding of all of the communites basic methods and tips I highly recommend you don't continue.

This tutorial of sorts is just meant to clarify how I made the [Shell Tag](https://discord.com/channels/186980582863929345/474346837352906752/847923391758991382)

## Now what is Marshmellow?

Marshmellow is really just similar word for cloud, maybe this is what it'll be called in the future, maybe not.

Carl-bot offers a very unique and interesting language called tagscript, however one of the major downsides of it, is you currently have no way to save data in an efficient, secure way (Tagscript is still fun and interesting though). 

To save data you have in a sense 2 options in tagscript:

1. Saving users nicknames
    - Doesn't work unless you either ping an alt user or have a user continuously run the command for you
    - Takes up a command block that has to edit a users nickname
    - The data is basically publicly available
    - Limited to 32 characters
2. Using a role color and changing its value
    - Limited to the same permissions as no 1
    - Information is in a sense also publicly available
    - Limited to 6 characters that are case insensitive and can only have 0-9 with no emojis
    - Also uses a command block

In essence, you really cannot save data in a desirable way...

So how do we work around this?

A user by the name of **Squidtoon99#3637** first made a tag quite a while back, in which he made a bot capable of doing much more by using api endpoints through a third party service known as https://repl.it.

[The tag link.](https://discord.com/channels/186980582863929345/474346837352906752/763139745068875776)

This intrigued me, how was someone able to make such complicated functions, at that time I really didn't understand any python though so I didn't think much of it and left it.

Note at this point this tag wasn't able to save data, it was just able to do a lot more complicated actions.

## 6 Months Later

Fast forward a few months and I stumbled accross it again, this time understanding a lot more python I decided to take a look and here comes an amazing idea.

Simply put, when discord sends an image in an embed it makes a request (It requests twice actually but that isn't important right now), this request then displays the actual image for you. Meaning if you were to make discord send a request for an image you can return an image while also doing something iternally.

Think of it like this

1. User sends !help
2. Carl now makes an embed with an image from a url like so [Image](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/Picture_icon_BLACK.svg/1200px-Picture_icon_BLACK.svg.png)
3. Before carl sends it discord requests the image url
4. Discord sends the embed Carl requested with the image url

This basic idea was so simple, yet so smart and so after a bit of practice with flask I tried to make Carls first way of saving data in a more efficient, maybe secure way.

## Before I get into it

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
2. Requires a lot more work (It took me a week to work through everything with almost no prior knowledge... I'd say it now take me around a day now but thats still a lot)

## Final Notes

I will be talking as if you understand many tagscript concepts, if you're not sure if you will understand try to understand the following.

```
Create a role color command that assigns a role based on a keyword using a switch, blankify the role command so that it won't execute if the keyword isn't found in the switch.
```

If you understand that you're fine, if not try to learn a bit more tagscript before moving on.

This is entirely possible without python, I just used that because its simple and the first language I learned.

## Finally

If you want to learn about how I made everything with python head on over to the README in the python folder

If you want to learn just about how you can integrate api endpoints with tagscript head on over to the regular folder

I hope you have as much fun as I did using this new concept!

Good luck and have fun!

- _Leg3ndary