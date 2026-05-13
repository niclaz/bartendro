# Roadmap

Some improvements we want to make to Bartendro to disentangle it from mayhem's Hippo Oasis and simplify the setup porocess, so it can be used by other people and find a good home.

1. Serve its own wifi access point
   * no need to depend on another wifi network being present, for people to connect to it
   * this does not need to connect to internet, should just be a local network
2. Fix annoying bug where drinks will be poured directly from the drinks menu, without waiting for the confirmation screen
   * this needs to be investigated, last time it started doing that later in the evening
   * successive reboots helped for short amounts of time, but problem returned
   * after some time the bug stopped happening, no idea why
   * perhaps related to some queuing system I saw some old code for?
3. Setup wizard - current setup is complicated and lots of manual work, requires figuring out combinations on paper
   * wizard should allow you to easily select ingredients for each pump
   * then present a list of cocktails that can be served with the available ingredients
   * allow selecting (tickbox) the cocktails to put on the menu, and which section in the UI they go to
4. Stretch goal: cocktail explorer
   * need to find an appropriate free API, where you can search by multiple ingredients
   * on bartendro admin, input your available liquids and fetch a list of cocktails that use them
   * then import cocktail recipes right into the bartendro database
