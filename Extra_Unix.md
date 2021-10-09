# Unix

I've already mentioned this but here is a more in depth explanation for this concept!

After making a similar tag to my shell tag you may notice something.

Lets say you want to show a random picture, lets also assume that this part works perfectly.

Our url would be something like

`/show/random`

Now, everytime this is called it will show a different image and again, let us assume this works perfectly.

You will now notice a massive flaw, when running this command you will always recieve the same image, if you keep running this every minute for a day, a week, a year you will still get the same image...

Why?

Discord wants to be fast and so it caches images occasionally. This means that if our url returns a random picture everytime, discord will not care, they will just use their cached old unupdated image and send that.

So how do we avoid this?

Put simply, we'll make the url change everytime all we have to is add a {unix} value as an extra unused parameter.

`/show/random/unixnumber`
`/show/random/321876378131`

This will let discord cache all they want, but in the end we'll always have a unique value. You could make it even better by adding more unused parameters that choose a random number making the url unique everytime however this is the solution I came up with.