Oneworld RTW Routes Explorer
============================

An easy way of planning your Oneworld RTW trip


<img src="https://github.com/IanWorthington/rtw-explorer/blob/master/assets/main.png?raw=true">
<img src="https://github.com/IanWorthington/rtw-explorer/blob/master/assets/search.png?raw=true">

When purchasing a horse make sure there's a leg at each corner (aka things you should know)
-------------------------------------------------------------------------------------------

This is an early release of the application, but it's still in active development, so expect bugs and niggles!.  Most of the Oneworld 3015 rule set has been implemented but not everything.  In particular the special rules for Australia are not yet included. The route data may be a little stale.  No attempt has been made to identify which non-oneworld carriers operate some of their routes under OW codeshares (but I think LATAM might have some, so their routes are included but with their tier points harvest set to zero.)  Tierpoints are calculated based on BA's earning percentages before bonuses. I've only done testing against DONE3 continent rules so far.

The "Find Max TPs..." dialog will allow you to start a search for the most profitable routings.  The default settings will usually work for a single continent, but you may need to increase the width and branching for more complicated searches.  In theory you can use this to plan a complete RTW itiniary but my machine runs out of memory when attempting to do so, which suprises me not at all.  Also it makes a rather long time.  I'm working on an alternative search algorithm that may help.

The Hub-only pruning and Anti-backtracking options are likely redundant, and will probably be removed in the next version.

Searching tip: find a well connected exit airport from the continent prior to the one you wish to search (eg JFK, BOS, LAX, ...) and step further back into that continent (eg DFW, ORD).  Set this later as your starting point, then search over this continent with only one segment, then the continent you're interested in (eg Asia), with your destination as a well connected entry airport into a new continent (eg MAD, DOH, LHR).  Not all Asian airports are well connected into Europe so take a look at the map first to identify likely suspects.

The major performance bottlenecks have been eliminated but there's still further work to be done there. 

Whilst running a complex search the dialog may show "(Not responding)".  You should though see occasional messages written to the console window opened in the background.  Don't despair.  Unless your search is overly large it will come back to you.

Feel free to record any major issues you find here. 