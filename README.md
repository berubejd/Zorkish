# Zorkish!

This is a tiny exercise in JavaScript that allows the user to explore "rooms" in a "world".  It's using prompts and alerts so not the most pleasant of experiences.

The world can be expanded simply by continuing to build out the locations array.  The first of which I've included below:

``` Javascript
            var locations = [
                {
                    "title":"West of House",
                    "description":"You are standing in an open field west of a white house, with a boarded front door. There is a small mailbox here.",
                    "options":[
                        {
                            "option":"Open Mailbox",
                            "response":"You pull a leaflet out of the mailbox that reads:\n\nWelcome to Zorkish!  This is just a couple of fake rooms from Zork.  Other than this, most of the text is from the original game.",
                            "exit":null
                        },
                        {
                            "option":"Go East",
                            "response":"The door is locked, and there is evidently no key.",
                            "exit":null
                        },
                        {
                            "option":"Go West",
                            "response":null,
                            "exit":1
                        }
                    ]
                },
            ];
```

It is also possible to include both a response, which is presented to the user as an alert, and an exit which then changes the location in the array that will next be presented to the user.
