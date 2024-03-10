# definitive guide to playing pokemon on the analogue pocket
- [introduction](#introduction)
- [optimal play method per game as of 2024/03/09](#optimal-play-method-per-game-as-of-20240309)
- [play methods & pros/cons](#play-methods--proscons)
    1. [authenic cartridges](#authentic-cartridges)
    2. [flash carts](#flash-carts)
    3. [cores](#cores)
- [relevant flash carts & surrounding nuance](#relevant-flash-carts--surrounding-nuance)
    - [Game Boy Color](#Game-Boy-Color)
        - [EZ-Flash Junior (not recommended)](#EZ-Flash-Junior-not-recommended)
        - [Everdrive GB X7 (not recommended)](#Everdrive-GB-X7-not-recommended)
        - [BennVenn mbc3000 v4 (recommended for use with the N64 Game Pak)](#BennVenn-MBC3000-v4-recommended-for-use-with-the-N64-Game-Pak)
    - [Game Boy Advanced](#Game-Boy-Advanced)
        - [EZ-Flash Omega Definitive Edition (highly recommended 👑)](#EZ-Flash-Omega-Definitive-Edition-highly-recommended) 
        - [Everdrive GBA Mini X5 (recommended)](#Everdrive-GBA-Mini-X5-recommended)
    - [micro SD cards](#micro-sd-cards)
- [alternative methods of re-syncing in-game time](#alternative-methods-of-re-syncing-in-game-time)
    - [preface](#preface)
    - [methods](#methods)
- [interfacing with Pokémon Home](#interfacing-with-Pokemon-Home)
- [product links](#product-links)
- [cores / software / firmware](#cores--software--firmware)
- [relevant guides](#relevant-guides)
- [frequently asked questions](#frequently-asked-questions)
    - [Why don't you recommend the everdrive GB X7 for use with the Analogue Pocket?](#Why-dont-you-recommend-the-Everdrive-GB-X7-for-use-with-the-Analogue-Pocket)
    - [Why do i want to interface my gen 1/2 games with the N64 transfer pack / Pokemon Stadium 1&2](#Why-do-i-want-to-interface-my-gen-12-games-with-the-N64-transfer-pack--Pokemon-Stadium-12)
    - [Why can't most flash carts interface with specialized Nintendo hardware/software (Game Pak, Pal Park, etc)?](#Why-cant-most-flash-carts-interface-with-specialized-Nintendo-hardwaresoftware-Game-Pak-Pal-Park-etc)
    - [Why can't most flash carts utilize the Analogue Pocket's sleep functionality?](#Why-cant-most-flash-carts-utilize-the-Analogue-Pockets-sleep-functionality)

# introduction
Pokémon games are unique due to their utilization of real-time clock, aka RTC. RTC keeps track of time while you aren't playing Pokémon games, essentially it syncs in-game time with real-time. in-game events such as Pokémon catchability, access ot the Move Tutor, Kurt's Apricorn Pokéballs, certain Pokémon evolutions, berry growth, lotteries, Secret Base battles, etc. depend on RTC. This causes complications depending on what method you're using to play Pokémon games on the Analogue Pocket. Bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/RTC effects in each generation of Pokémon. Generation 2 is much more dependant on RTC than generation 3, but it's important enough in both generations that I wouldn't consider playing without functional RTC.

# optimal play method per game as of 2024/03/09
- Red -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (stadium 1&2)
- Blue -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (Stadium 1&2)
- Green -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts  (Stadium 1&2)
- Yellow -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts  (Stadium 1&2)
- Silver -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (stadium 1&2)
- Gold -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (stadium 1&2)
- Crystal -> GBC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (stadium 1&2)
- Ruby -> EZ-Flash Omega DE
- Sapphire -> EZ-Flash Omega DE
- Emerald -> EZ-Flash Omega DE
- Fire Red -> GBA core
- Leaf Green -> GBA core

# play methods & pros/cons
There are three methods of playing pokemon on the Analogue pocket.
1. #### authentic cartridges
    - pros
        - time is tracked while you aren't playing the game
        - sleep/save states are partially functional
        - no setup required
        - interfaces with official Nintendo hardware/software (N64 Game Pak, Pal Park, etc.)
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
        - GBC carts
            - save states are partially functional
            - **ez-flash junior** - in-game clock can be reset via modification of cart's internal clock
            - **BennVenn MBC3000 & Inside Gadgets RTC carts** - compatible with N64 Gam Pak for use with Pokémon Colleseum
        - GBA carts
            - save states are fully functional
            - time is recalculated when sleep/save states are loaded (always in-sync)
            - **ez-flash omega de** - compatible with analogue pocket's sleep feature
        - both
            - much cheaper than authentic carts in the grand scheme of things
            - time is tracked while you aren't playing
            - easy to replace internal batteries
            - save files are easily accessible for backup
    - cons
        - GBC carts
            - incompatible with analogue pocket's sleep feature
            - time is not recalculated when save states are loaded (desync)
            - **everdrive gb x7** - time is ireversably desynced when save states are loaded without mods/exploits
        - GBA carts
            - **everdrive gba mini** - incompatible with analogue pocket's sleep feature
        - both
            - costs money
            - additional setup required
            - rtc relies on internal batteries that eventually die 
3. #### cores
    - pros
        - GBC RTC Core
            - time is tracked while you aren't playing the game
        - GBA Core
            - sleep/save states are partially functional
        - both
            - free
            - save files are easily accesible for backup
            - save data & RTC functionality is not dependant on the finite life of a non-rechargable battery
            - additional setup required 
    - cons
        - GBC RTC Core
            - sleep/save states are unavailable
        - GBA Core
            - time is only tracked when playing the game
            - time is not re-calculated when sleep/save states are loaded on cores that utilize said functionality
        - both
            - incapable of interfacing with some Nintendo hardware/software (N64 Game pak, pal park, etc.)

# relevant flash carts & surrounding nuance
### summary
There's little reason to use the EZ-Flash Jr. or Everdrive GB X7 after the release of [budude2's RTC compatible GBC Core](https://github.com/budude2/openfpga-GBC). The best combination of carts for use with the Analogue Pocket is the [BennVenn MBC3000 v4](https://bennvenn.myshopify.com/products/mbc3000-rtc-gbc-cart-v4?variant=40095079202919), and the [EZ-Flash Omega DE](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1). Why? Because this gives you the most compatibility with the Analogue Pocket's sleep/save state functions, and official Nintendo hardware/software (N64 Game Pak, Pal Park, etc). Functionality with the N64 Game Pak is particularly relevant given [the announcment](https://x.com/analogue/status/1713933239327273452?s=20) of the analogue 3d.
### Game Boy Color
- #### [EZ-Flash Junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-Everdrive/dp/B08379XZWY/ref=sr_1_1?crid=27VHV05U1YVS0&keywords=ez-flash+jr&qid=1700286287&sprefix=ez-flash+jr%2Caps%2C124&sr=8-1) (**recommended**)
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
    - incompatible with N64 Game Pak, and thus Pokémon Stadium.
- #### [Everdrive GB X7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=everdrive+gb+x7&qid=1700286142&sprefix=everdrive+gb+%2Caps%2C138&sr=8-1) (**not recommended**)
    - 3x more expensive than the ez-flash junior, albeit with a superior physical build quality.
    - for whatever reason, the method mentioned above for resetting the in-game time via the ez-flash junior, is not possible via the everdrive gb x7. there is no method of re-syncing in-game time with real time outside of rom hacks / in-game exploits. you could technically use your giant brain to constantly adjust the cart's internal clock, to offset for in-game time. but it's not tenable, as it would have to be accounted for *per game*.
    - incompatible with n64 game pak, and thus pokemon stadium.
- #### [BennVenn MBC3000 v4](https://bennvenn.myshopify.com/products/mbc3000-rtc-gbc-cart-v4?variant=40095079202919) (**recommended for use with the n64 game pak**)
    - requires bennvenn's joey jr v2++, or something comparable, to flash games to the cartridge.
    - more expensive (including a joey jr v2++) than the ez-flash junior, but less expensive than the everdrive gb x7.
    - time is permanently desynced like the everdrive gb x7 when save states are loaded.
    - unlike other carts, there is no sd card, and only one game can be stored on the cart at a time.
    - because only one game is loaded at a time, **this cart is compatible with the n64 game pak / pokemon stadium.
### Game Boy Advanced
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
- *note that*
    - everdrive requires that cards >32gb remain formatted as fat32. on microsoft windows, this requires a [special tool](http://ridgecrop.co.uk/index.htm?guiformat.htm).
    - the omega de requires that cards >32gb must be formatted as exfat
- it is my recommendation that you use 32gb cards for everything to make things simple, realistically you'll never fill 32gb with gb/gbc/gba roms.
- as mentioned above the ez-flash junior specifically requires a fast micro sd card to function, the others will benefit from a fast micro sd card as well.
- i recommend [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro sd card
 
# alternative methods of re-syncing in-game time
### preface
i personally wouldn't recommend using these methods as they're pretty hands on, or require rom hacks. it is much more intuitive, and feels closer to the intended experience to use flash carts (when it comes to rtc).
### methods
- gen 2
    - [in-game exploit](https://www.youtube.com/watch?v=Vupz6vwylGM&t)
    - rom hacks
- gen 3
    - **authentic carts** - desolder the internal battery, solder in a new one.
    - rom hacks

# interfacing with pokemon home
- gen 1&2
   - backup your save file
   - [load your save file onto the virtual console version of said game via a modded 2/3ds running checkpoint](https://www.youtube.com/watch?v=pe9mw25mHGA)
   - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go) guide
- gen 3
   - method 1 (authentic carts & ez-flash omega de only)
      - if you're using the ez-flash omega de the game must be running in mode b
      - [use a nintendo ds + pal park to trade pokemon from gen 3 to gen 4](https://bulbapedia.bulbagarden.net/wiki/Pal_Park)
      - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go) guide
   - method 2
      - backup your gen 3 save file
      - [use desume to emulate Pal Park transfer](https://www.youtube.com/watch?v=o0RkljY3UMw) using your save file
      - [load your save file onto an authentic Gen 4 cart using a modded 3DS running checkpoint](https://projectpokemon.org/home/tutorials/save-editing/managing-3ds-saves/using-checkpoint-r25/)
      - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go) guide

# product links
- [ez-flash junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-Everdrive/dp/B08379XZWY/ref=sr_1_2?crid=2827XS0JEDDSF&keywords=ez+flash+jr&qid=1677688333&sprefix=ez+flash+j%2Caps%2C200&sr=8-2&ufe=app_do%3Aamzn1.fos.08f69ac3-fd3d-4b88-bca2-8997e41410bb)
- [everdrive gb x7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=everdrive+gb+x7&qid=1700286142&sprefix=everdrive+gb+%2Caps%2C138&sr=8-1)
- [bennvenn mbc3000 v4](https://bennvenn.myshopify.com/products/mbc3000-rtc-gbc-cart-v4?variant=40095079202919)
- [bennvenn joey jr v2++](https://bennvenn.myshopify.com/products/usb-gb-c-cart-dumper-the-joey-jr)
- [benvenn mbc3000 v4 + joey jr v2++ bundle](https://bennvenn.myshopify.com/products/mbc3k-joey-bundle?variant=40037766135911) ($10 discount when bundled)
- [ez-flash omega definitive edition](https://www.amazon.com/EZ-Definitive-gba-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1)
- [everdrive gba mini x5](https://www.amazon.com/EverDrive-GBA-X5-Mini-Game-Boy/dp/B0052URK0Q/ref=sr_1_1?crid=3S3NA2KAJ3BKM&keywords=everdrive+gba+mini&qid=1700285313&sprefix=everdrive+gba+mini%2Caps%2C122&sr=8-1)
- [micro sd card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
- [ez-flash junior, everdrive gb x7, bennvenn mbc3000 v4, & everdrive gba mini battery replacement](https://www.amazon.com/dp/B014WXZO0G?psc=1&smid=A19DY5EK03NION&ref_=chk_typ_imgToDp) (cr1220)
- [ez-flash omega de battery replacement](https://www.amazon.com/dp/B001ERBLME?psc=1&smid=AI62U825BKVWC&ref_=chk_typ_imgToDp) (cr1025)

# cores / software / firmware
- cores/software
    - [pocket sync](https://github.com/neil-morrison44/pocket-sync/releases) (gui core installer | [guide](https://github.com/neil-morrison44/pocket-sync))
    - [fat32 formatter](http://ridgecrop.co.uk/index.htm?guiformat.htm) (required for >32GB micro sd cards used with everdrive carts)
- firmware
    - [ez-flash junior](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) (**use this specific firmware** with [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) specific micro sd card | [guide](https://www.youtube.com/watch?v=inus-2l5oeg))
    - [everdrive gb x7](https://krikzz.com/pub/support/everdrive-gb/x-series/OS/) ([guide](https://ddavegames.neocities.org/guides/everdrivegbx7/))
    - [bennvenn joey jr.](https://bennvenn.myshopify.com/products/usb-gb-c-cart-dumper-the-joey-jr) ([guide](https://bennvenn.myshopify.com/pages/the-joey-junior-gb-gbc-gba-cart-dumper-and-flasher))
    - [ez-flash omega de](https://www.ezflash.cn/download/) ([guide](https://www.ezflash.cn/omegade-en.pdf#page=10))
    - [everdrive gba mini](https://krikzz.com/pub/support/everdrive-gba/OS/) ([guide](https://ddavegames.neocities.org/guides/everdrivegbx7/))

# relevant guides
- [pocket sync](https://github.com/neil-morrison44/pocket-sync/blob/main/README.md)
- [ez-flash junior](https://www.youtube.com/watch?v=rqeFD8SRbVA) (please use [this](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) firmware & [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+sd+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro sd card)
- [everdrive gb x7](https://www.youtube.com/watch?v=p9IYgMTvl2c)
- bennvenn mbc3000 v4 (basically just a normal cart | see joey jr guide below for usage)
- [bennvenn joey jr v2++](https://bennvenn.myshopify.com/pages/the-joey-junior-gb-gbc-gba-cart-dumper-and-flasher)
- [ez-flash omega de manual](https://www.ezflash.cn/omegade-en.pdf)
- [ez-flash omega de](https://www.youtube.com/watch?v=CBPoAjBfV0M&t)
- [ez-Flash omega de mode b / standalone mode](https://youtu.be/MSWgdfbpgPI?t=129)
- [everdrive gba mini](https://www.youtube.com/watch?v=epLif4ju4F0)
- [replace batteries in flash carts](https://gbatemp.net/threads/ez-flash-omega-de-replacing-the-battery.612300/)
- [backup saves on authentic carts](https://www.reddit.com/r/Gameboy/comments/4w8xjf/guide_how_to_backup_your_game_save_files/)
- [mod 2/3ds systems & load checkpoint for save management](https://www.youtube.com/watch?v=ttHCJ1oFpDc)

# frequently asked questions
### why don't you recommend the everdrive gb x7 for use with the analogue pocket?
in-game time desyncs when a save state is loaded while using the everdrive gb x7, with little recourse to remedy the issue. it is also vastly more expensive than the ez-flash junior, while being less functional in relation to the pocket, as previously mentioned.

### why do i want to interface my gen 1&2 games with the n64 transfer pack / pokemon stadium 1&2
pokemon stadium 1&2 provide these unique benefits
- much easier pokemon box orginzation
- much faster / bulk transfer of pokemon between games
- [shiny hunting eggs in gen 2](https://www.youtube.com/watch?v=Nywbm5ZZZvQ&t)
    
### why can't most flash carts interface with specialized nintendo hardware/software (game pak, pal park, etc)?
because most flash carts launch to a menu in-which you first have to select a rom to interact with it. the bennvenn only ever has one game flashed at time. likewise, the omega de has the option (mode b) to run a single game standalone. this allows these carts to interface with specialized nintendo hardware/software, as they are viewed as single authentic game by the receiving hardware.

### why can't most flash carts utilize the analogue pocket's sleep functionality?
similarly to my previous answer, only carts that offer a standalone game mode can utilize the analogue pocket's sleep functionality. this is because this sleep functionality is really a save state *for a specific game* in disguise. when you sleep your analogue pocket a save state is stored, when you wake your analogue pocket it attempts to load that save state. if you're using a flash cart that loads to a menu before it can load a specific game, it's impossible to load a state for a specific game before it is manually selected.
