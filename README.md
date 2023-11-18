# index

# introduction
pokemon games are unique due to their utilization of real-time clock, aka rtc. rtc keeps track of time while you aren't playing pokemon games, essentially it syncs in-game time with real-time. in-game events such as pokemon catchability, access ot the move tutor, kurt's apricorn pokeballs, certain pokemon evolutions, berry growth, lotteries, secret Base battles, etc. depend on rtc. this causes complications depending on what method you're using to play pokemon games on the analogue pocket. bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/rtc effects in each generation of pokemon. generation 2 is much more dependant on rtc than generation 3, but it's important enough in both generations that i wouldn't consider playing without functional rtc.

# quick explanation of the rtc mechanism
it's pretty complicated... but from my understanding, an encoded start time stamp is stored in your save file. when you launch your game, a calculation is made by getting a difference in your original timestamp, and current time. directly modifying the data that controls this time stamp seems nearly impossible as an end user. it would appear that different hardware (oem carts, flash carts, fpga) & software (emulators) calculate things differently, making it difficult to transfer save data between different hardware/software without de-syncing your in-game clock.

# play methods
there is currently 3 methods of playing pokemon games on the analogue pocket
1. authentic cartridges
2. flash carts
3. 3rd party "cores"
