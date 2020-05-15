# MarveliOS

MarveiliOS is an App that uses Marel Official API to get marvel characters and show the detail of a specific character. 
For personal purposes only, not with comercial use.

Data provided by Marvel. © 2014 Marvel

## Architecture

I have used a MVP-Coordinator architecture, because I think that this kind of architecture is one of the best solutions for separate responsibilities between layers, for testing and for clear coding.

In this architecture View layer only knows what to show, nothing else, that comes from MVP, and also, with Coordinator we minimise the responsibilities of the Presenter because Coordinator is the responsible of the app's navigation. 

## Observations

I have added a SplashScreen because the MarvelAPI doesn't accept real pagination requests, so you should do several request changing the parameter "offset", increasing it at a maximum of 100 in every request, so you only get 100 characters from request, and this is a time handicap for the App, so I used SplashScreen with a ProgressBar to show the loading progress to user.
## Rights
Marvel. © 2014 Marvel