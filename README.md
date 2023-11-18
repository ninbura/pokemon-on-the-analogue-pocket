# index

# introduction
pokemon games are unique due to their utilization of real-time clock, aka rtc. rtc keeps track of time while you aren't playing pokemon games, essentially it syncs in-game time with real-time. in-game events such as pokemon catchability, access ot the move tutor, kurt's apricorn pokeballs, certain pokemon evolutions, berry growth, lotteries, secret Base battles, etc. depend on rtc. this causes complications depending on what method you're using to play pokemon games on the analogue pocket. bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/rtc effects in each generation of pokemon. generation 2 is much more dependant on rtc than generation 3, but it's important enough in both generations that i wouldn't consider playing without functional rtc.

# quick explanation of the rtc mechanism
it's pretty complicated... but from my understanding, an encoded start time stamp is stored in your save file. when you launch your game, a calculation is made by getting a difference in your original timestamp, and current time. directly modifying the data that controls this time stamp seems nearly impossible as an end user. it would appear that different hardware (oem carts, flash carts, fpga) & software (emulators) calculate things differently, making it difficult to transfer save data between different hardware/software without de-syncing your in-game clock. **because rtc data is stored within a game's save data, analogue could technically push a fix for this in the future.** by ripping the save data from the cart, modifying the save data, and loading a state with correct rtc data. but i wouldn't your breath.

# play methods & pros/cons
there are three methods of playing pokemon on the analogue pocket. tldr; flash carts are currently superior for playing pokemon games that utilize rtc.
1. #### authentic cartridges
    - pros
        - time is tracked while you aren't playing the game
        - sleep/save states are partially functional
        - display modes are supported
        - no setup required
        - interfaces with official nintendo hardware/software (n64 game pak, pal park, etc.)
        - karts r kool
    - cons
        - extremely expensive
        - time is not re-calculated when sleep/save states are loaded (desync)
        - gen 2 cartridge save data is lost when the cart's internal battery dies
        - gen 3 cartridge time is no longer tracked when the cart's internal battery dies
        - cartridge battery replacement requires soldering
        - additional hardware is required to backup save data
2. #### flash carts
    - pros
        - much cheaper than authentic carts in the grand scheme of things
        - time is tracked while you aren't playing
        - **gbc carts** - save states are partially functional
        - **gba carts** - save states are fully functional
        - **gba carts** - time is recalculated when sleep/save states are loaded (always in-sync)
        - **ez-flash junior** - in-game clock can be reset via modification of cart's internal clock
        - **ez-flash omega de** - compatible with analogue pocket's sleep feature
        - easy to replace internal batteries
    - cons
        - costs money
        - **everdrive gba mini x5 & gbc carts** - incompatible with analogue pocket's sleep feature
        - **everdrive gb x7** - time is ireversably desynced when save states are loaded without mods/exploits
        - **gbc carts** - time is not recalculated when save states are loaded (desync)
        - additional setup required
        - save files are easily accessible for backup
        - rtc relies on internal batteries that eventually die 
3. #### 3rd party cores
    - pros
        - free
        - sleep/save states are partially functional
        - save files are easily accesible for backup
        - save data & rtc functionality is not dependant on the finite life of a non-rechargable battery
        - additional setup required 
    - cons
        - time is only tracked when playing the game
        - time is not re-calculated when sleep/save states are loaded
        - display modes are not supported (but should be by the end of 2023)
        - incapable of interfacing with some nintendo hardware/software (n64 game pak, pal park, etc.)

# relevant flash carts & surrounding nuance
### gbc
- #### [ez-flash junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-Everdrive/dp/B08379XZWY/ref=sr_1_1?crid=27VHV05U1YVS0&keywords=ez-flash+jr&qid=1700286287&sprefix=ez-flash+jr%2Caps%2C124&sr=8-1) (**recommended**)
    - 3x cheaper than the everdrive gb x7, albiet wtih an inferior physical build quality.
    - while time isn't recalculated after loading a save state, the in-game clock can be reset by manipulating the cart's internal clock
        1. set the internal clock 2 years ahead
        2. launch your game
        3. return the junior's menu by pressing the button in the cart (press on front), or by resetting the cartrige via the anlogue pocket's menu.
        4. re-sync the internal clock with real time
        5. launch your game
        6. follow the in-game prompts to re-set your in-game clock
    - incompatible with n64 game pak, and thus pokemon stadium. this is particularly relevant given [the announcment](https://x.com/analogue/status/1713933239327273452?s=20) of the analogue 3d.
- #### [everdrive gb x7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=everdrive+gb+x7&qid=1700286142&sprefix=everdrive+gb+%2Caps%2C138&sr=8-1) (**not recommended**)
    - 3x more expensive than the ez-flash junior, albeit with a superior physical build quality.
    - for whatever reason, the method mentioned above for resetting the in-game time via the ez-flash junior, is not possible via the everdrive gb x7. there is no method of re-syncing in-game time with real time outside of rom hacks / in-game exploits. you could technically use your giant brain to constantly adjust the cart's internal clock, to offset for in-game time. but it's not tenable, as it would have to be accounted for *per game*.
    - incompatible with n64 game pak, and thus pokemon stadium. this is particularly relevant given [the announcment](https://x.com/analogue/status/1713933239327273452?s=20) of the analogue 3d.
- #### [bennvenn mbc3000 v4](https://bennvenn.myshopify.com/products/mbc3000-rtc-gbc-cart-v4?variant=40095079202919) (**recommended for use with the n64 game pak**)
    - requires bennvenn's joey jr v2++, or something comparable, to flash games to the cartridge.
    - more expensive (including a joey jr v2++) than the ez-flash junior, but less expensive than the everdrive gb x7.
    - time is permanently desynced like the everdrive gb x7 when save states are loaded.
    - unlike other carts, there is no sd card, and only one game can be stored on the cart at a time.
    - because only one game is loaded at a time, **this cart is compatible with the n64 game pak / pokemon stadium. this is particularly relevant given [the announcment](https://x.com/analogue/status/1713933239327273452?s=20) of the analogue 3d.
### gba
- gba flash carts cannot be used to play gbc games without utilizing emulation. this defeats the purpose of fpga and games are noticably letterboxed, taking up only a small fraction of the pocket's display.
- #### [ez-flash omega definitive edition](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1) (**highly recommended 👑**)
    - 40% cheaper than the everdrive gba mini x5 with similar build quality and *more features*
    - a physical switch on the outside of the cart allows you to enter [mode b / standalone mode](https://www.ezflash.cn/omegade-en.pdf#page=13)
        - *please note that mode b is not compatible with the latest analogue pocket firmware, but ez-flash is working on a fix.*
        - allows for operation like the bennvenn mbc3000 v4, making the receiving console believe that only one game is flashed to the cart.
        - allows for use of analogue pocket's sleep function
        - can interface with pokemon [pal park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park) to transfer pokemon from gen 3 to gen 4 via a nintendo ds.
- #### [everdrive gba mini x5](https://www.amazon.com/EverDrive-GBA-X5-Mini-Game-Boy/dp/B0052URK0Q/ref=sr_1_1?crid=3S3NA2KAJ3BKM&keywords=everdrive+gba+mini&qid=1700285313&sprefix=everdrive+gba+mini%2Caps%2C122&sr=8-1) (**recommended**)
    - 40% more expensive than the ez-flash omega de with similar build quality and *less features*
    - not compatible with stand alone cart functions, like the analogue pocket's sleep functionality, or pokemon [pal park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park).
### conclusion
the best combination of carts for use with the analogue pocket is the ez-flash junior + the bennvenn mbc300 + the ez-flash omega de. why? because this gives you the most compatibility with the analogue pockets sleep/save state functions, and official nintendo hardware/software (n64 game pak, pal park, etc). the ez-flash junior & bennvenn mbc3000 is kind of a wombo combo, as you can fix time sync via the junior, and interface with the n64 game pak / pokemon stadium via the mbc3000.
    
