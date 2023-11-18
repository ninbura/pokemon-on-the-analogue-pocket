# index

# introduction
pokemon games are unique due to their utilization of real-time clock, aka rtc. rtc keeps track of time while you aren't playing pokemon games, essentially it syncs in-game time with real-time. in-game events such as pokemon catchability, access ot the move tutor, kurt's apricorn pokeballs, certain pokemon evolutions, berry growth, lotteries, secret Base battles, etc. depend on rtc. this causes complications depending on what method you're using to play pokemon games on the analogue pocket. bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/rtc effects in each generation of pokemon. generation 2 is much more dependant on rtc than generation 3, but it's important enough in both generations that i wouldn't consider playing without functional rtc.

# quick explanation of the rtc mechanism
it's pretty complicated... but from my understanding, an encoded start time stamp is stored in your save file. when you launch your game, a calculation is made by getting a difference in your original timestamp, and current time. directly modifying the data that controls this time stamp seems nearly impossible as an end user. it would appear that different hardware (oem carts, flash carts, fpga) & software (emulators) calculate things differently, making it difficult to transfer save data between different hardware/software without de-syncing your in-game clock.

# play methods & their pros/cons
there is currently 3 methods of playing pokemon games on the analogue pocket
  1. authentic cartridges
    - pros
      - time is tracked while you aren't playing the game
      - sleep/save states are partially functional
      - display modes are supported
      - no setup required
      - interfaces with official nintendo hardware/software (n64 game pak, pal park, etc.)
      - karts r kool
    - cons
        - extremely expensive
        - time is not re-calculated when sleep/save states are loaded
        - gen 2 cartridge save data is lost when the cart's internal battery dies
        - gen 3 cartridge time is no longer tracked when the cart's internal battery dies
        - cartridge battery replacement requires soldering
        - additional hardware is required to backup save data
  2. flash carts
    - pros
      - much cheaper than authentic carts in the grand scheme of things
      - time is tracked while you aren't playing
      - **gbc carts** - save states are partially functional
      - **gba carts** - save states are fully functional
      - **EZ-Flash Omega DE** - compatible with analogue pockets sleep feature
      - **gba carts** - time is recalculated when sleep/save states are loaded
      - easy to replace internal batteries
    - cons
      - costs money
      - **everdrive gba mini & gbc carts** - incompatible with analogue pocket's sleep feature
      - **gbc carts** - time is not recalculated when sleep/save states are loaded
      - additional setup required
      - save files are easily accessible for backup
      - rtc relies on internal batteries that eventually die 
  3. 3rd party cores
    - pros
      - free
      - sleep/save states are partially functional
      - save files are easily accesible for backup
      - save data & rtc functionality is not dependant on finite life of a non-rechargable battery
      - additional setup required 
    - cons
      - time is only tracked when playing the game
      - time is not re-calculated when sleep/save states are loaded
      - display modes are not supported (but should be by the end of 2023)
