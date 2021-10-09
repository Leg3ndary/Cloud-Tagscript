# Welcome

Here you'll learn about how I made the "Shell Tag" which stores words and gives them an index so you can view them later.

I used python though I cannot say I'm exactly an expert, all of this is just what worked for me and is by no means something that will always work.

**IMPORANT**
Please do not DM me or go to Carl bots support server to ask for help. This is not something they or I will help with. You can though create an issue on this github and I will try my best to answer questions when I have time.

## Getting Started
You will obviously need to know a bit of python, I would also recommend going to https://repl.it and creating an account, you can create a project later but if you don't have an IDE open up a project.

First I would recommend setting up your endpoints and what you actually want to do...

```py
API Endpoints... 
BASE URL (Removed, don't really want people messing around too much...)
The above shows wether the api endpoint is alive and working...

Endpoints...
/dev/show
Shows the original image/shell which images are further drawn on

/dev/cache
Shows the built cache

/show/<index:int>/<unix:int>
Shows the image at that index... You can view different images with this, integer input

/add/<word:str>/<unix:int>
Adds another word to the cache and database... Must pass a small filter before being shown 

/error
Literally just says error, what did you expect?
```

This is what I had planned out for mine!

The rest of the files in this folder will contain all the info you need, have fun!