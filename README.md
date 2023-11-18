# index

# introduction
pokemon games are unique due to their utilization of real-time clock, aka rtc. rtc keeps track of time while you aren't playing pokemon games, essentially it syncs in-game time with real-time. in-game events such as pokemon catchability, access ot the move tutor, kurt's apricorn pokeballs, certain pokemon evolutions, berry growth, lotteries, secret Base battles, etc. depend on rtc. this causes complications depending on what method you're using to play pokemon games on the analogue pocket. bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/rtc effects in each generation of pokemon. generation 2 is much more dependant on rtc than generation 3, but it's important enough in both generations that i wouldn't consider playing without functional rtc.

# quick explanation of the rtc mechanism
it's pretty complicated... but from my understanding, an encoded start time stamp is stored in your save file. when you launch your game, a calculation is made by getting a difference in your original timestamp, and current time. directly modifying the data that controls this time stamp seems nearly impossible as an end user. it would appear that different hardware (oem carts, flash carts, fpga) & software (emulators) calculate things differently, making it difficult to transfer save data between different hardware/software without de-syncing your in-game clock. **because rtc data is stored within a game's save data, analogue could technically push a fix for this in the future.*- by ripping the save data from the cart, modifying the save data, and loading a state with correct rtc data. but i wouldn't your breath.

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
        - **gbc carts*- - save states are partially functional
        - **gba carts*- - save states are fully functional
        - **gba carts*- - time is recalculated when sleep/save states are loaded (always in-sync)
        - **ez-flash junior*- - in-game clock can be reset via modification of cart's internal clock
        - **ez-flash omega de*- - compatible with analogue pocket's sleep feature
        - easy to replace internal batteries
    - cons
        - costs money
        - **everdrive gba mini x5 & gbc carts*- - incompatible with analogue pocket's sleep feature
        - **everdrive gb x7*- - time is ireversably desynced when save states are loaded without mods/exploits
        - **gbc carts*- - time is not recalculated when save states are loaded (desync)
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
    - **!!! important !!!**
        - an unlisted / hard to find [firmware](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) is currently required for the junior to function with an analogue pocket
        - this unlisted firmware will cause your junior to brick / die if you're not using a [fast enough micro sd card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
    - 3x cheaper than the everdrive gb x7, albiet wtih an inferior physical build quality.
    - while time isn't recalculated after loading a save state, the in-game clock can be reset by manipulating the cart's internal clock
        1. set the internal clock 2 years ahead
        2. launch your game
        3. return the junior's menu by pressing the button in the cart (press on front), or by resetting the cartrige via the anlogue pocket's menu.
        4. re-sync the internal clock with real time
        5. launch your game
        6. follow the in-game prompts to re-set your in-game clock
    - incompatible with n64 game pak, and thus pokemon stadium.
- #### [everdrive gb x7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=everdrive+gb+x7&qid=1700286142&sprefix=everdrive+gb+%2Caps%2C138&sr=8-1) (**not recommended**)
    - 3x more expensive than the ez-flash junior, albeit with a superior physical build quality.
    - for whatever reason, the method mentioned above for resetting the in-game time via the ez-flash junior, is not possible via the everdrive gb x7. there is no method of re-syncing in-game time with real time outside of rom hacks / in-game exploits. you could technically use your giant brain to constantly adjust the cart's internal clock, to offset for in-game time. but it's not tenable, as it would have to be accounted for *per game*.
    - incompatible with n64 game pak, and thus pokemon stadium.
- #### [bennvenn mbc3000 v4](https://bennvenn.myshopify.com/products/mbc3000-rtc-gbc-cart-v4?variant=40095079202919) (**recommended for use with the n64 game pak**)
    - requires bennvenn's joey jr v2++, or something comparable, to flash games to the cartridge.
    - more expensive (including a joey jr v2++) than the ez-flash junior, but less expensive than the everdrive gb x7.
    - time is permanently desynced like the everdrive gb x7 when save states are loaded.
    - unlike other carts, there is no sd card, and only one game can be stored on the cart at a time.
    - because only one game is loaded at a time, **this cart is compatible with the n64 game pak / pokemon stadium.
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
### micro sd cards
- ez-flash & everdrive carts utilize micro sd cards
- both cart manufacturers state that <=32gb must be formatted as fat32
- specificallly ez-flash asks that you use a 32KB allocation size
- you can technically use cards greater than 32gb with these carts
    - everdrive gb x7
    - everdrive gba mini
    - ez-flash omega de
    - *note that cards >32gb must be formatted as exfat*
- it is my recommendation that you use 32gb cards for everything to make things simple, realistically you'll never fill 32gb with gb/gbc/gba roms.
- as mentioned above the ez-flash junior specifically requires a fast micro sd card to function, the others will benefit from a fast micro sd card as well.
- i recommend [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro sd card
### flash cart conclusion
the best combination of carts for use with the analogue pocket is the ez-flash junior, the bennvenn mbc300, and the ez-flash omega de. why? because this gives you the most compatibility with the analogue pockets sleep/save state functions, and official nintendo hardware/software (n64 game pak, pal park, etc). the ez-flash junior & bennvenn mbc3000 is kind of a wombo combo, as you can fix time sync via the junior, and interface with the n64 game pak / pokemon stadium via the mbc3000. simply transfer your save files between the 2 carts. functionality with the n64 game pak is particularly relevant given [the announcment](https://x.com/analogue/status/1713933239327273452?s=20) of the analogue 3d.
    
# optimal play method per game
- games with no rtc
    - Red -> GBC Core / bennvenn mbc3000 (stadium 1&2)
    - Blue -> GBC Core / bennvenn mbc3000 (stadium 1&2)
    - Green -> GBC Core / bennvenn mbc3000 (stadium 1&2)
    - Yellow -> GBC Core / bennvenn mbc3000 (stadium 1&2)
    - Fire Red -> GBA Core / bennvenn mbc3000 (stadium 1&2)
    - Leaf Green -> GBA Core / bennvenn mbc3000 (stadium 1&2)
- games with rtc
    - Silver -> EZ-Flash Jr. / bennvenn mbc3000 (stadium 1&2)
    - Gold -> EZ-Flash Jr. / bennvenn mbc3000 (stadium 1&2)
    - Crystal -> EZ-Flash Jr. / bennvenn mbc3000 (stadium 1&2)
    - Ruby -> EZ-Flash Omega DE
    - Sapphire -> EZ-Flash Omega DE
    - Emerald -> EZ-Flash Omega DE
- why interface with pokemon stadium?
    - much easier pokemon box orginzation
    - much faster / bulk transfer of pokemon between games
    - [shiny hunting eggs in gen 2](https://www.youtube.com/watch?v=Nywbm5ZZZvQ&t)

# interfacing with pokemon home
- gen 1&2
   - backup your save file
   - [load your save file onto the virtual console version of said game via a modded 2/3ds running checkpoint](https://www.youtube.com/watch?v=pe9mw25mHGA)
   - from there follow [this guide](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go)
- Gen 3
   - method 1 (authentic carts & ez-flash omega de only)
      - ff you're using the ez-flash omega de the game must be running in mode b
      - [use a nintendo ds + pal park to trade pokemon from gen 3 to gen 4.](https://bulbapedia.bulbagarden.net/wiki/Pal_Park)
      - from there follow [this guide](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go).
   - method 2
      - backup your gen 3 save file
      - [use desume to emulate Pal Park transfer](https://www.youtube.com/watch?v=o0RkljY3UMw) using your save file
      - [load your save file onto an authentic Gen 4 cart using a modded 3DS running checkpoint](https://projectpokemon.org/home/tutorials/save-editing/managing-3ds-saves/using-checkpoint-r25/)
      - from there follow [this guide](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go)

# Product Links
- [ez-flash junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-Everdrive/dp/B08379XZWY/ref=sr_1_2?crid=2827XS0JEDDSF&keywords=ez+flash+jr&qid=1677688333&sprefix=ez+flash+j%2Caps%2C200&sr=8-2&ufe=app_do%3Aamzn1.fos.08f69ac3-fd3d-4b88-bca2-8997e41410bb)
- [ez-flash omega de](https://www.amazon.com/EZ-Flash-Definitive-EZFlash-Geddes/dp/B09SFQK82G/ref=sr_1_2?crid=1W8G08L2V0N23&keywords=ez+flash+omega+definitive+edition&qid=1677688892&sprefix=ez+flash+omega%2Caps%2C279&sr=8-2&ufe=app_do%3Aamzn1.fos.08f69ac3-fd3d-4b88-bca2-8997e41410bb)
- [micro sd card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
- [ez-flash junior battery replacement](https://www.amazon.com/dp/B014WXZO0G?psc=1&smid=A19DY5EK03NION&ref_=chk_typ_imgToDp) (cr1220)
- [ez-flash omega de battery replacement](https://www.amazon.com/dp/B001ERBLME?psc=1&smid=AI62U825BKVWC&ref_=chk_typ_imgToDp) (cr1025)

# relevant guides
- [pocket sync](https://github.com/neil-morrison44/pocket-sync/blob/main/README.md)
- [ez-flash junior](https://www.youtube.com/watch?v=rqeFD8SRbVA) (please use [this firmware](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) & [this sd card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
- [ez-flash omega de](https://www.youtube.com/watch?v=CBPoAjBfV0M&t=651s)
- [ez-Flash omega de mode b / standalone mode](https://youtu.be/MSWgdfbpgPI?t=129)
- [replace batteries in flash carts](https://gbatemp.net/threads/ez-flash-omega-de-replacing-the-battery.612300/)
- [backup saves on authentic carts](https://www.reddit.com/r/Gameboy/comments/4w8xjf/guide_how_to_backup_your_game_save_files/)
- [mod 3ds family systems & load checkpoint for save management](https://www.youtube.com/watch?v=ttHCJ1oFpDc)
