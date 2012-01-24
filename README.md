# ST4bby (A **S**tandalone **T4** POCO Generator)

ST4bby is a T4 template (actually 2 right now) that will generate POCO's (Plain Old CLR Objects) from your database tables and columns.  It doesn't rely on any particular ORM, but can be used in conjunction with them, including but not limited to

1. Entity Framework
2. Dapper
3. Massive
4. Anything else that uses POCO's relating directly to your database schema.

## How do I use it?

Here is all you need to do:

1. Drop the 2 T4 templates into your Visual Studio Project (Coming soon to NuGet).
2. Open up the "ST4bby.Config.ttinclude.tt" template.
3. Set your own values for the nameSpaceName, serverName, and databaseName (If you're using SQL Server authentication, make sure you set the username and password, OR the connection string name from your web/app.config).
4. Save the template and it should prompt you to run!  Just hit OK and watch the magic happen!

After that, you can continue to run the T4 template as you update the database, or you can delete the templates and keep the POCO's.

## Limitations:

1. Generates POCO's for all tables in the database (no automatic filtering).  Ideally a schema, prefix, or regex filter would be nice.
2. The only Data Annotation attribute that is currently added is the Key attribute.  Ideally we will support all related validation attributes.


# HA HAAAAAAAAA!!!

    ..............................................................................................................................
    ............................  ....:.:... .....................................................................................
    ....................... ::::ccccccccccccccc. ................. .. .:ccccccc:..................................................
    ......................:::.cccccc:.    .:cccccc ............ ::..ccccccccccccccc ..............................................
    ................... :::::cccc             .cccc:......... :::.ccccc:       :ccccc ............................................
    ...................:::.cccc.     :oc        :cccc ...... ::::cccc             cccc ...........................................
    ................. :::::ccc     @@@@@@@8c     :ccccccccccccccccc.      .O@@@c   .ccc ..........................................
    .................::::.ccc:   .@@@@@@@@@@@@o   ................     c@@@@@@@@@   :cc:..........................................
    .................::::.ccc.   8@@@@@@   @@@@                      c@@@@@@@   @O  .ccc .........................................
    .................::::.ccc:   C@@@@@@88@@@@8                      :@@@@@@@@@@@C  :cc: .........................................
    ................. :::::ccc    O@@@@@@@@@@8                        o@@@@@@@@@O   ccc ..........................................
    ...................::::cccc.    C@@@@@@O.   cccccccccccccccccccc.   c8@@@@o   .ccc............................................
    ................... ::::ccccc.            :cccc:cccccccccccccc:ccc:         :cccc ............................................
    .................... .::::ccccccc:....:cccccc:.:ccccccccccccc::.:cccccccccccccc ..............................................
    ....................... .:::cccccccccccccc:.::::cccccccccccccc   .  .:cccc:. .................................................
    ..................................... .:::::::.cccccccccccccc.................................................................
    ...................................... ::::::::.cccccccccccccc ...............................................................
    ...................................... :::::::: cccccccccccccc .......................................................oO888c..
    .............................. .....   :::::::: cccccccccccccc ...................................................:C88O8888c..
    .......................... .::::::::::.::::::::.cccccccccccccc...........................................:: ...:C888888888C...
    .........................:::::::::::.. ::::::::::cccccccccccccc .........................................: .:oO88CO888888O....
    ...................... :::::::::.:cccc:::::::::::.cccccccccccccc ........................................:o888OO88888888O:....
    ......................::::::::.ccccccc:::::::::::::cccccccccccccc......................................oO88CO8888888888O:.....
    ................... ::::::::.ccccc......:::::::::::cooooc....:cc ...................................:O88OO888888888888O.......
    ..... ..:::::::::::::::::::.ccccc.... . ::::::OC88C888888.   .....................................o88OC88888888888888c........
    .... :::.:::::::::::::::::.cccccc.... . ::::coOCOOCOOOOOC... ..................................cO8OCO88888888888888C..........
    .... ::::::.::::::::::::::ccccccc:....  ::::::Oo88C88COOc...................................:O88CO888888888888888o............
    .... ::::::::.........:::ccccccccccccccc::::::::::ccccccccc:.............................:C88CO888888888888888Oc..............
    .... .ccccc:.::ccccccccccccccccccccccccc.::::::::.ccccccccc.........  . :ccc::c...     cO8OCO888888O8888888Oc.................
    ... ccccccccc.ccccccccccccccccccccccccccc.::::::.ccccccccc ... :ccccccccc:.cc.:.:.:::C8888C8888888888888Oc: ..................
    .. ccc.........:ccccc:::.:.:::cccccccccccccc....:.:....   ...ccccccccccccccc..::::.::o8888888O888O8OCc.. . ...................
    .  cc:....... ...... ..:ccccccccccccccccccccc:ccccc:cc.. . cccccccccccccccccc ::::: .:o888888OCo:....... : ...................
    .. ccc ..... ................. .  ......:::::.:::: . .... cccccccccccccccccccc.:::::..:::: ............. : ...................
    ... cccc:... ............... ......... .......... .......ccccccccccccccccccccc.:::::::::::: ............ . ...................
    ...::.:cccc:......................... .......... ........cccccccccccccc.:c:..c::::.:.. . .  .........    :    ................
    .. ::::::::::cccccc. ................ .......... .........cccccccccccc.cccccc.... . . .  ........... ...::::: ................
    .. :::::::::cccccc:cccccccc:.................... .........cccccccccccc::ccc.ccccc................  ..............  ...........
    .. ::::::::.cccccc.ccccccccccccccccccccc::....      ...... .ccccc.ccccc:.c.ccccccc:cc........ ........................  ......
    ..:::::::::.cccccc:cccccccccccccccccccccc.ccc........... .::..ccc:cccccc...:cccc::c...... ................................ ...
    ..::::::::::ccccccccccccccccccccccccc::.:ccc:...........   ....   :ccc::cccc:c:  ...... ......................................
    . :::::::::ccccccc::::......:::ccccccccccccc ........... .   . ..   .c:cccc.cc:...... ........................................