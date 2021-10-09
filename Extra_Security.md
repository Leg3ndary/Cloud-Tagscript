# Security

**This should be read after reading all of the python or regular folder.**

As you should know already, when sharing a tag a user will get to see everything they want in the content of the tag. This means its basically impossible to impose an 100% secure tag. So what can you do?

The simplest solution I've came up with is just using unix times which are ever changing however always accurate.

Consider this;

Person A and Person B are both playing a game you've made, and Person B is trying to impersonate Person A and steal currency

```py
/give/givingpersonid/recieveingpersonid/amount
```

Lets say this is now the basic url for the command.

2 massive problems arise, 1 discord will ultimately send more then just 1 request meaning commands may be ran twice by accident.

2 its really easy to now just steal currency.

So how do we fix this?

Ultimately I would just advise completely against having this in the first place, but if you steal want to go through, I would add another parameter; the unix time value.

Now what we can do is check if this request was sent with a unix time accurate within 1-2 seconds.

This means now discords second requests should be nullified (They would send a request maybe 5 seconds after and now our program seeing the wrong time will know that this isn't needed and won't answer the request)

This also means users that are trying to bypass the system must keep alternating the url with an accurate unix value.

This won't 100% help however its the best way to fix a few issues in my opinion.