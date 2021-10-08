# Welcome

Here you'll just learn about the barebones of making a *Marshmellow*!

I'll just be going through steps, the rest will be up to you!

1. Decide on your endpoints and their format.

EG `https://carl.gg/api/<action>`

**IMPORTANT**
As stated in the original README discord makes requests to the api, the first is just to get it, however discord may send another request to cache the image.

Though this may sound unrelated this means if you have a link which is something like

`https://carl.gg/api/carl` which shows a random picture of carl every time, it will not work.

Discord will cache the image it gets on the second request and for around a few hours it will stay that way until it's cleared. To get around this you must add a completely everchanging parameter.

I used a simple unix value using the unix block, this means that you must take in a completely useless parameter in your endpoint so that discord won't cache it.

`https://carl.gg/api/carl/123456789`

After a second:

`https://carl.gg/api/carl/123456790`

This is important if you have an endpoint that updates itself, this allows you to display the changes.

2. Set up whatever database you'll be using and add all the functions in

EG when `http://carl.gg/api/carl/123456789` is called, carl will return a random turtle plus add 1 to a global uses value stored in your database...

3. Tagscript

For this part it really doesn't matter, I would recommend using a switch but this part should be something you understand...

Just alter a base url and put a variable containing it in the image field of the embed.