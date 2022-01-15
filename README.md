# GDQPing-Python36
A Discord bot written in python to ping member of server when a GDQ speedrun is about to start. You can also see upcoming runs, or search the schedule for key words.

***Many commands are setup to DM the caller in order to reduce channel spam. Its recommended to make a special channel for the bot.

How to setup(The guild owner must run this command):
 +admin init (*Used once* Initiate a guild into bot's guild directory.)

[+help]
 
    GDQping bot - receive notifications when a GDQ run is about to start.
    Quick Tutorial:
    1. Use '+schedule all' to get all run ids
    2. Construct your sub command, example:
       +sub 1 3 5 or +sub 1,2,3,4
       OR +sub all to subscribe to all runs
    3. Use the sub command in the bot channel
    5. Get a ping about 10 minutes before a run
    6. Profit!

    Commands:
        +sub [number]- Subcribe to a GDQ run
        +unsub [number]- Unsubscribe to a GDQ run
        +upcoming - Get the upcoming games
        +schedule "query here"- Query GDQ Schedule
        +admin - Only admins (obv) can use these
    
    
[+help sub]

    Usage:
    +sub 1 (Subscribe to single run)

    +sub "1,2,3,4,5" (Subscribe to multiple runs, quotations recommended)

    +sub all (Every run will notify you)

    +sub list (Get a list of your subscriptions sent DM to you)

    Subscribe to runs by using it's ID. The ID can be found on the schedule next to the game name. The 'all' command does not overwrite your single subscriptions, however it takes priority over your single subscriptions.


[+help unsub]

    Usage:
    +unsub 1 (Unsubscribe to single run)

    +unsub "1,2,3,4,5" (Unsubscribe to multiple runs, quotations recommended)

    +unsub all (Every run won't notify you)

    +unsub purge (Purge all subscriptions, including 'all' subscription)

Unsubscribe to runs by using it's ID. The ID can be found on the schedule next to the game name. The 'all' subscription is a seperate preference from your single subcriptions, you will keep your single subscriptions if you unsub from 'all'.


[+help schedule]

    Usage:
    +upcoming (Show 5 next runs on the schedule)

    +schedule "search string" (Quickly search for a run)

    +schedule all (Get all IDs via DM, works only once an hour)

    +schedule ['name', 'runner', 'host'] "search string" (Search for a run using it's name, runner, or host)

View the latest schedule for AQGDQ 2021. The schedule is sync'd to the AGDQ schedule every five minutes to reduce inconsistencies.
