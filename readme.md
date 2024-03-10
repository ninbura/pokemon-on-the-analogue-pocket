# definitive guide to playing Pokémon on the analogue pocket
- [introduction](#introduction)
- [optimal play method per game as of 2024/03/09](#optimal-play-method-per-game-as-of-20240309)
- [play methods & pros/cons](#play-methods--proscons)
    1. [cores](#cores)
    2. [flash carts](#flash-carts)
    3. [authenic cartridges](#authentic-cartridges)
- [relevant Cores & surrounding nuance](#relevant-cores--surrounding-nuance)
- [relevant flash carts & surrounding nuance](#relevant-flash-carts--surrounding-nuance)
    - [Game Boy Color](#Game-Boy-Color)
        - [EZ-Flash Junior (not recommended)](#EZ-Flash-Junior-recommended)
        - [EverDrive GB X7 (not recommended)](#EverDrive-GB-X7-not-recommended)
        - [BennVenn MBC3000 (recommended for use with the N64 Game Pak)](#BennVenn-MBC3000-recommended-for-use-with-the-N64-Game-Pak)
        - [insideGadgets GBC RTC cart (**recommended for use with the N64 Game Pak**)](#insideGadgets-GBC-RTC-cart-recommended-for-use-with-the-N64-Game-Pak)
        - [insideGadgets GBC RTC LinkNLoad cart (**recommended for use with the N64 Game Pak**)](#insideGadgets-GBC-RTC-LinkNLoad-cart-recommended-for-use-with-the-N64-Game-Pak)
    - [Game Boy Advanced](#Game-Boy-Advanced)
        - [EZ-Flash Omega Definitive Edition (highly recommended 👑)](#EZ-Flash-Omega-Definitive-Edition-highly-recommended-) 
        - [EverDrive GBA Mini X5 (recommended)](#EverDrive-GBA-Mini-X5-recommended)
    - [micro SD cards](#micro-SD-cards)
- [manually reset RTC data](#manually-reset-RTC-data)
- [convert save data to 2/3DS Virtual Console save data and back](convert-save-data-to-23DS-Virtual-Console-save-data-and-back)
- [interfacing with Pokémon Home](#interfacing-with-Pokémon-Home)
- [product links](#product-links)
- [cores / software / firmware](#cores--software--firmware)
- [relevant guides](#relevant-guides)
- [frequently asked questions](#frequently-asked-questions)
    - [Why don't you recommend the EverDrive GB X7 for use with the Analogue Pocket?](#Why-dont-you-recommend-the-EverDrive-GB-X7-for-use-with-the-Analogue-Pocket)
    - [Why do I want to interface my gen 1/2 games with the N64 transfer pack / Pokémon Stadium 1&2](#Why-do-i-want-to-interface-my-gen-12-games-with-the-N64-transfer-pack--Pokemon-Stadium-12)
    - [Why can't most flash carts interface with specialized Nintendo hardware/software (Game Pak, Pal Park, etc)?](#Why-cant-most-flash-carts-interface-with-specialized-Nintendo-hardwaresoftware-Game-Pak-Pal-Park-etc)
    - [Why can't most flash carts utilize the Analogue Pocket's sleep functionality?](#Why-cant-most-flash-carts-utilize-the-Analogue-Pockets-sleep-functionality)

# introduction
Some Pokémon games are unique due to their utilization of real-time clock, aka RTC. RTC keeps track of time while you aren't playing Pokémon games, essentially it syncs in-game time with real-time. in-game events such as Pokémon catchability, access ot the Move Tutor, Kurt's Apricorn Pokéballs, certain Pokémon evolutions, berry growth, lotteries, Secret Base battles, etc. depend on RTC. This causes complications depending on what method you're using to play Pokémon games on the Analogue Pocket. Bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/RTC effects in each generation of Pokémon. Generation 2 is much more dependant on RTC than generation 3, but it's important enough in both generations that I wouldn't consider playing without functional RTC.

# optimal play method per game as of 2024/03/09
- Red -> GBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (Stadium 1&2)
- Blue -> GBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (Stadium 1&2)
- Green -> GGBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts  (Stadium 1&2)
- Yellow -> GBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts  (Stadium 1&2)
- Silver -> GBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (Stadium 1&2)
- Gold -> GBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (Stadium 1&2)
- Crystal -> GBC RTC core / BennVenn MBC3000 or insideGadgets GBC RTC carts (Stadium 1&2)
- Ruby -> EZ-Flash Omega DE
- Sapphire -> EZ-Flash Omega DE
- Emerald -> EZ-Flash Omega DE
- Fire Red -> GBA core (no RTC)
- Leaf Green -> GBA core (no RTC)

# play methods & pros/cons
There are three methods of playing pokemon on the Analogue pocket.
1. #### cores
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
            - incapable of interfacing with some Nintendo hardware/software (N64 Game Pak, Pal Park, etc.)
2. #### flash carts
    - pros
        - GBC carts
            - save states are partially functional
            - **EZ-Flash Junior** - in-game clock can be reset via modification of cart's internal clock
            - **BennVenn MBC3000 & insideGadgets RTC carts** - compatible with N64 Gam Pak for use with Pokémon Colleseum
        - GBA carts
            - save states are fully functional
            - time is recalculated when sleep/save states are loaded (always in-sync)
            - **EZ-Flash Omega DE** - compatible with analogue pocket's sleep feature
        - both
            - much cheaper than authentic carts in the grand scheme of things
            - time is tracked while you aren't playing
            - easy to replace internal batteries
            - save files are easily accessible for backup
    - cons
        - GBC carts
            - incompatible with analogue pocket's sleep feature
            - time is not recalculated when save states are loaded (desync)
            - **EverDrive GB X7 | BennVenn MBC3000 | insideGadgets carts** - time is desynced when save states are loaded & can't be resynced without external software, rom hacks, or exploits.
        - GBA carts
            - **EverDrive GBA Mini** - incompatible with analogue pocket's sleep feature
        - both
            - costs money
            - additional setup required
            - rtc relies on internal batteries that eventually die 
3. #### authentic cartridges
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
     
# relevant cores & surrounding nuance
- there are currently 2 GBC cores & 1 GBA core available for the Analogue Pocket
- Only 1 of 3 cores currently supports RTC, and it's a GBC core.
- There are no GBA cores that support RTC, so you'll want to use a GBA flash cart. Several are mentioned below.
- I recommend installing all cores using [Pocket Sync](https://github.com/neil-morrison44/pocket-sync), but make sure you select the proper GBC core, the one that supports RTC (budude2's core).
- direct links
    - [GBC by spiritualized1997](https://github.com/spiritualized1997/openFPGA-GB-GBC) (RTC not implemented ❌)
    - [GBC by budude2](https://github.com/budude2/openfpga-GBC) (RTC implemented ✅)
        - Note that this core does not crurrently have a sleep/save state implementation, and once implemented could cause RTC desync.
        - I will update the guide when sleep/save state implemenation drops, hopefully it's implemented to account for RTC desync 🤞
    - [GBA by spiritualized1997](https://github.com/spiritualized1997/openFPGA-GBA) (RTC not implemented ❌)

# relevant flash carts & surrounding nuance
### summary
**There's little reason to use the EZ-Flash Jr. or EverDrive GB X7 after the release of [budude2's RTC compatible GBC Core](https://github.com/budude2/openfpga-GBC).** The best combination of carts for use with the Analogue Pocket is the [BennVenn MBC3000](https://BennVenn.myshopify.com/products/MBC3000-rtc-GBc-cart-v5) or insideGadgets GBC carts w/ RTC (see below), and the [EZ-Flash Omega DE](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1). Why? Because this gives you the most compatibility with the Analogue Pocket's sleep/save state functions, and official Nintendo hardware/software (N64 Game Pak, Pal Park, etc). Functionality with the N64 Game Pak is particularly relevant given [the announcment](https://x.com/analogue/status/1713933239327273452?s=20) of the analogue 3d.
### Game Boy Color
- #### [EZ-Flash Junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-EverDrive/dp/B08379XZWY/ref=sr_1_1?crid=27VHV05U1YVS0&keywords=ez-flash+jr&qid=1700286287&sprefix=ez-flash+jr%2Caps%2C124&sr=8-1)
    - **!!! important !!!**
        - an unlisted / hard to find [firmware](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) is currently required for the junior to function with an analogue pocket
        - this unlisted firmware will cause your junior to brick / die if you're not using a [fast enough micro SD card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
    - 3x cheaper than the EverDrive GB X7, albiet wtih an inferior physical build quality.
    - while time isn't recalculated after loading a save state, the in-game clock can be reset by manipulating the cart's internal clock
        1. set the internal clock 2 years ahead
        2. launch your game
        3. return the junior's menu by pressing the button in the cart (press on front), or by resetting the cartrige via the anlogue pocket's menu.
        4. re-sync the internal clock with real time
        5. launch your game
        6. follow the in-game prompts to re-set your in-game clock
    - incompatible with N64 Game Pak, and thus Pokémon Stadium.
- #### [EverDrive GB X7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=EverDrive+GB+X7&qid=1700286142&sprefix=EverDrive+GB+%2Caps%2C138&sr=8-1)
    - 3x more expensive than the EZ-Flash Junior, albeit with a superior physical build quality.
    - For whatever reason, the method mentioned above for resetting the in-game time via the EZ-Flash Junior, is not possible via the EverDrive GB X7. there is no method of re-syncing in-game time with real time outside of external software, rom hacks, or in-game exploits. you could technically use your giant brain to constantly adjust the cart's internal clock, to offset for in-game time. but it's not tenable, as it would have to be accounted for *per game*.
    - incompatible with N64 Game Pak, and thus Pokémon Stadium.
- #### [BennVenn MBC3000](https://BennVenn.myshopify.com/products/MBC3000-rtc-GBc-cart-v5) (**for use with the N64 Game Pak**)
    - Requires [BennVenn's Joey Jr](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr), or something comparable, to flash games to the cartridge.
    - significantly less expensive that insideGadgets offerings
    - time is desynced when save states are loaded without use of external applications or in-game exploits
    - Unlike other carts, there is no SD card, and only one game can be stored on the cart at a time.
    - As only one game is loaded at a time, *this cart **is compatible** with the N64 Game Pak / Pokémon Stadium*.
- #### [insideGadgets GBC RTC cart](https://shop.insidegadgets.com/product/gameboy-2mb-32kb-fram-mbc3-with-rtc-flash-cart/) (**for use with the N64 Game Pak**)
    - Requires [BennVenn's Joey Jr](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr), or something comparable, to flash games to the cartridge.
    - significantly more expensive that BennVenn's MBC3000
    - time is desynced when save states are loaded without use of external applications or in-game exploits
    - Unlike other carts, there is no SD card, and only one game can be stored on the cart at a time.
    - As only one game is loaded at a time, *this cart **is compatible** with the N64 Game Pak / Pokémon Stadium*.
- #### [insideGadgets GBC RTC LinkNLoad cart](https://shop.insidegadgets.com/product/gameboy-mbc3-rtc-linknload-usb-flash-cart-works-with-pokemon-games-hacks-like-cc/) (**for use with the N64 Game Pak**)
    - **Does not** require an additional cart flashing tool, you can flash games directly via the USB-C port on the card.
    - Significantly more expensive that BennVenn's MBC3000 & insideGadgets non "LinkNLoad" cart, but possibly more convenient as an additonal flasher is not required.
    - time is desynced when save states are loaded without use of external applications or in-game exploits
    - Unlike other carts, there is no SD card, and only one game can be stored on the cart at a time.
    - As only one game is loaded at a time, *this cart **is compatible** with the N64 Game Pak / Pokémon Stadium*.
### Game Boy Advanced
- GBA flash carts cannot be used to play GBC games without utilizing emulation. This defeats the purpose of fpga and games are noticably letterboxed, taking up only a small fraction of the pocket's display.
- #### [EZ-Flash Omega Definitive Edition](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1) (**highly recommended 👑**)
    - 40% cheaper than the EverDrive GBA Mini x5 with similar build quality and *more features*
    - a physical switch on the outside of the cart allows you to enter [Mode B / standalone mode](https://www.ezflash.cn/omegade-en.pdf#page=13)
        - *please note that Mode B is not compatible with the latest analogue pocket firmware, but ez-flash is working on a fix.*
        - compatible with Analogue Pocket's sleep function in "standalone mode"
        - Allows for flashing a game to memory and running it in "standalone" mode. This functionality allows for interfacing with Pokémon [Pal Park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park) to transfer Pokémon from gen 3 to gen 4 via a Nintendo DS.
- #### [EZ-Flash Omega](https://www.amazon.com/EZ-Flash-MicroSDHC-Version-Latest/dp/B01GZMNRP6/ref=sr_1_2?crid=6NN7MN3GBTZT&dib=eyJ2IjoiMSJ9.SmTKXapduSgeZ_JdvicuRg4thNulTgxNWppXvD3cVmruPRG7yPAjotgKgyc1wKtwigxpazDeuFgHgnOV_zpsq1mn0Th_iDztT9kPZp5RSn1s009V88zbHYb2gZu2KCi1AXAahSIB0-D1KX4pFzYBNVapK8S44b1lRS1ymXw7bVqD1TB05gF5hRpm_DUvT8SIlbhwbS5v5MCekxO5ftuNDT7xiU0v1pjWvHZYN8TdPRg.dN_DrbgQmKs7ELYJycj41FE9W46kpq8ZMmUnn0-giik&dib_tag=se&keywords=EZ-Flash+Omega&qid=1710045811&sprefix=ez-flash+omeg%2Caps%2C157&sr=8-2)
    - much cheaper than the Omega DE & GBA Mini
    - Not compatible with stand alone cart functions, like the Analogue Pocket's sleep functionality, or Pokémon [Pal Park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park).
    - Battery is soldered in, making it much more difficult to replace.
- #### [EverDrive GBA Mini x5](https://krikzz.com/our-products/cartridges/everdrive-gba-mini.html)
    - 40% more expensive than the EZ-Flash Omega DE with similar build quality and *less features*
    - Not compatible with stand alone cart functions, like the Analogue Pocket's sleep functionality, or Pokémon [Pal Park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park).
### micro SD cards
- EZ-Flash & EverDrive carts utilize micro SD cards
- both cart manufacturers state that <=32GB must be formatted as fat32
- specificallly EZ-Flash asks that you use a 32KB allocation size
- you can technically use cards greater than 32GB with these carts
    - EverDrive GB X7
    - EverDrive GBA Mini
    - EZ-Flash Omega DE
- *note that*
    - EverDrive requires that cards >32GB remain formatted as fat32. on microsoft windows, this requires a [special tool](http://ridgecrop.co.uk/index.htm?guiformat.htm).
    - the Omega DErequires that cards >32GB must be formatted as exfat
- it is my recommendation that you use 32GB cards for everything to make things simple, realistically you'll never fill 32GB with GB/GBc/GBA roms.
- as mentioned above the EZ-Flash Junior specifically requires a fast micro SD card to function, the others will benefit from a fast micro SD card as well.
- I recommend [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro SD card
 
# manually reset RTC data
- [PKHeX](https://projectpokemon.org/home/files/file/1-pkhex/) (gen 1&2)
    1. backup save data
    2. run PKHeX
    3. load backed up save file
    4. select the "SAV" tab
    5. select "Clock (RTC)"
    6. click "Yes"
    7. reload your save data into your cart/core
    8. reset time when prompted to in-game
- gen 2
    - [in-game exploit](https://www.youtube.com/watch?v=Vupz6vwylGM&t)
    - EZ-Flash Junior
        1. set the internal clock 2 years ahead
        2. launch your game
        3. return the junior's menu by pressing the button in the cart (press on front), or by resetting the cartrige via the anlogue pocket's menu.
        4. re-sync the internal clock with real time
        5. launch your game
        6. follow the in-game prompts to re-set your in-game clock
    - rom hacks
- gen 3
    - **authentic carts** - desolder the internal battery, solder in a new one.
    - rom hacks

# convert save data to 2/3DS Virtual Console save data and back
- there are a couple reasons why you'd want to transfer your save data between your Pocket and your 2/3DS virtual console
    1. To acquire the GS Ball in Pokémon Crystal, so you can capture Celebi.
        1. save in-front of Lance (doesn't have to be your first time battling him)
        2. backup your save data
        3. convert your save data to VC data using [this tool](https://inject.sigkill.tech/converter/3dsvc)
        4. transfer your save into Crystal Virtual Console edition using checkpoint (see [relevant-guides](#relevant-guides))
        5. defeat lance
        6. enter the Goldenrod City Pokémon Center
        7. exit the Goldenrod City Pokémon Center
        8. receive the GS Ball
        9. backup your save data using checkpoint (see [relevant-guides](#relevant-guides))
        10. re-convert you save data using [this tool](https://savefileconverter.com/#/flash-carts)
        11. re-inject your save into your core/cart
    2. To transfer Pokémon into Pokémon Home (see [interfacing with Pokémon Home](#interfacing-with-Pokémon-Home))
- To transfer saves into the Virtual Console versions, you'll need a modded 2/3DS running Checkpoint. See [relevant-guides](#relevant-guides) below for more info.
- save files are slightly different for GBC carts & cores vs Virtual Console save data, so you'll want to use converters to avoid corruption and incompatability.
    - [normal save to Virtual Console converter](https://inject.sigkill.tech/converter/3dsvc)
        - This is only required for gen 2, gen 1 saves don't need in-bound conversion.
        - Note that once converted to a VC save, save files will no longer be compatible with PKHeX. Use the next converter to solve this.
    - [Virtual Console to normal save converter](https://savefileconverter.com/#/flash-carts)

# interfacing with Pokémon Home
- **note that you can can transfer Gen 4-6 from 3DS into Pokémon Home *without using retail cartridges* as mentioned in https://github.com/ninbura/pokemon-on-the-analogue-pocket/issues/3**
- gen 1&2
   - backup your save file
   - [load your save file onto the virtual console version of said game via a modded 2/3DS running checkpoint](https://www.youtube.com/watch?v=pe9mw25mHGA)
   - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go) guide
- gen 3
   - method 1 (authentic carts & EZ-Flash Omega DE only)
      - if you're using the EZ-Flash Omega DE the game must be running in Mode B
      - [use a Nintendo ds + Pal Park to trade Pokémon from gen 3 to gen 4](https://bulbapedia.bulbagarden.net/wiki/Pal_Park)
      - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go) guide
   - method 2
      - backup your gen 3 save file
      - [use desume to emulate Pal Park transfer](https://www.youtube.com/watch?v=o0RkljY3UMw) using your save file
      - [load your save file onto an authentic Gen 4 cart using a modded 3DS running checkpoint](https://projectpokemon.org/home/tutorials/save-editing/managing-3ds-saves/using-checkpoint-r25/)
      - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3ds-switch-pokemon-go) guide

# product links
- [EZ-Flash Junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-EverDrive/dp/B08379XZWY/ref=sr_1_2?crid=2827XS0JEDDSF&keywords=ez+flash+jr&qid=1677688333&sprefix=ez+flash+j%2Caps%2C200&sr=8-2&ufe=app_do%3Aamzn1.fos.08f69ac3-fd3d-4b88-bca2-8997e41410bb)
- [EverDrive GB X7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=EverDrive+GB+X7&qid=1700286142&sprefix=EverDrive+GB+%2Caps%2C138&sr=8-1)
- [BennVenn MBC3000](https://BennVenn.myshopify.com/products/MBC3000-rtc-GBc-cart-v5)
- [insideGadgets GBC RTC cart](https://shop.insidegadgets.com/product/gameboy-2mb-32kb-fram-mbc3-with-rtc-flash-cart/)
- [insideGadgets GBC RTC LinkNLoad cart](https://shop.insidegadgets.com/product/gameboy-mbc3-rtc-linknload-usb-flash-cart-works-with-pokemon-games-hacks-like-cc/)
- [BennVenn Joey Jr](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr)
- [EZ-Flash Omega](https://www.amazon.com/EZ-Flash-MicroSDHC-Version-Latest/dp/B01GZMNRP6/ref=sr_1_2?crid=6NN7MN3GBTZT&dib=eyJ2IjoiMSJ9.SmTKXapduSgeZ_JdvicuRg4thNulTgxNWppXvD3cVmruPRG7yPAjotgKgyc1wKtwigxpazDeuFgHgnOV_zpsq1mn0Th_iDztT9kPZp5RSn1s009V88zbHYb2gZu2KCi1AXAahSIB0-D1KX4pFzYBNVapK8S44b1lRS1ymXw7bVqD1TB05gF5hRpm_DUvT8SIlbhwbS5v5MCekxO5ftuNDT7xiU0v1pjWvHZYN8TdPRg.dN_DrbgQmKs7ELYJycj41FE9W46kpq8ZMmUnn0-giik&dib_tag=se&keywords=EZ-Flash+Omega&qid=1710045811&sprefix=ez-flash+omeg%2Caps%2C157&sr=8-2)
- [EZ-Flash Omega Definitive edition](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1)
- [EverDrive GBA Mini x5](https://krikzz.com/our-products/cartridges/everdrive-gba-mini.html)
- [micro SD card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
- [EZ-Flash Junior, EverDrive GB X7, BennVenn MBC3000, & EverDrive GBA Mini battery replacement](https://www.amazon.com/dp/B014WXZO0G?psc=1&smid=A19DY5EK03NION&ref_=chk_typ_imgToDp) (CR1220)
- [EZ-Flash Omega DE battery replacement](https://www.amazon.com/dp/B001ERBLME?psc=1&smid=AI62U825BKVWC&ref_=chk_typ_imgToDp) (CR1025)
- [insideGadgets GBC carts battery replacement](https://www.amazon.com/Duracell-Lithium-Battery-Lasting-Count/dp/B07G7L5M4J/ref=sr_1_5?crid=S8BXXRKK17U9&dib=eyJ2IjoiMSJ9.-RhhqUEnEOUs7D29Trl6RogHqs206TL6e6n5L7pSAl1br6q03Tfm3K4nS6fBIe4rznz_6OgGFnjYbd1KIaXPH_2DlClztaNuUo1962X7ICQRFpPhqZ0fNok0NfB2E-yT3koLoGA5fbcgxq1mmAxANS5WWkHt50NRjaB8x79fklkhFerQuPeiivzhDLxWabxHeCGZMOv65BHLEvpN_JZ6oLkV8QoNHC3fpNaVlp1j3tdRsRROgEd0_KkfLDRMTy2arffaFUnGANqODgo-P4WiB2puy9XqRisKxKLrXTz1CBo.4emsr5u1FMxmbiqDdSz23-MjSU7cgupwFs0Wx0yXqLE&dib_tag=se&keywords=cr2025&qid=1710049061&sprefix=cr2025%2Caps%2C123&sr=8-5) (CR2025)

# cores / software / firmware
- cores/software
    - [Pocket Sync](https://github.com/neil-morrison44/pocket-sync/releases) (gui core installer | [guide](https://github.com/neil-morrison44/pocket-sync))
    - [fat32 formatter](http://ridgecrop.co.uk/index.htm?guiformat.htm) (required for >32GB micro SD cards used with EverDrive carts)
    - [PKHeX](https://projectpokemon.org/home/files/file/1-pkhex/)
- firmware
    - [EZ-Flash Junior](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) (**use this specific firmware** with [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) specific micro SD card | [guide](https://www.youtube.com/watch?v=inus-2l5oeg))
    - [EverDrive GB X7](https://krikzz.com/pub/support/EverDrive-GB/x-series/OS/) ([guide](https://ddavegames.neocities.org/guides/EverDriveGBX7/))
    - [BennVenn Joey Jr.](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr) ([guide](https://BennVenn.myshopify.com/pages/the-joey-junior-GB-GBc-GBA-cart-dumper-and-flasher))
    - [EZ-Flash Omega DE](https://www.ezflash.cn/download/) ([guide](https://www.ezflash.cn/omegade-en.pdf#page=10))
    - [EverDrive GBA Mini](https://krikzz.com/pub/support/EverDrive-GBA/OS/) ([guide](https://ddavegames.neocities.org/guides/EverDriveGBX7/))

# relevant guides
- [Pocket Sync](https://github.com/neil-morrison44/pocket-sync/blob/main/README.md)
- [EZ-Flash Junior](https://www.youtube.com/watch?v=rqeFD8SRbVA) (please use [this](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) firmware & [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro SD card)
- [EverDrive GB X7](https://www.youtube.com/watch?v=p9IYgMTvl2c)
- BennVenn MBC3000 (basically just a normal cart | see Joey Jr guide below for usage)
- [BennVenn Joey Jr](https://BennVenn.myshopify.com/pages/the-joey-junior-GB-GBc-GBA-cart-dumper-and-flasher)
- [EZ-Flash Omega DE manual](https://www.ezflash.cn/omegade-en.pdf)
- [EZ-Flash Omega DE](https://www.youtube.com/watch?v=CBPoAjBfV0M&t)
- [EZ-Flash Omega DE Mode B / standalone mode](https://youtu.be/MSWgdfbpgPI?t=129)
- [EverDrive GBA Mini](https://www.youtube.com/watch?v=epLif4ju4F0)
- [replace batteries in flash carts](https://GBAtemp.net/threads/ez-flash-omega-de-replacing-the-battery.612300/)
- [backup saves on authentic carts](https://www.reddit.com/r/Gameboy/comments/4w8xjf/guide_how_to_backup_your_game_save_files/)
- [mod 2/3DS systems & load checkpoint for save management](https://www.youtube.com/watch?v=ttHCJ1oFpDc)

# frequently asked questions
### Why do I want to interface my gen 1&2 games with the N64 transfer pack / Pokémon Stadium 1&2
Pokémon Stadium 1&2 provide these unique benefits
- much easier Pokémon box orginzation
- much faster / bulk transfer of Pokémon between games
- [shiny hunting eggs in gen 2](https://www.youtube.com/watch?v=Nywbm5ZZZvQ&t)
    
### Why can't most flash carts interface with specialized Nintendo hardware/software (Game Pak, Pal Park, etc)?
Most flash carts launch to a menu in-which you first have to select a rom to interact with it. The BennVenn & insideGadgets carts only ever have one game flashed at time. Likewise, the Omega DE has the option (Mode B) to run a single game standalone. this allows these carts to interface with specialized Nintendo hardware/software, as they are viewed as single authentic game by the receiving hardware.

### Why can't most flash carts utilize the Analogue Pocket's sleep functionality?
Similarly to my previous answer, only carts that offer a standalone game mode can utilize the analogue pocket's sleep functionality. This is because this sleep functionality is really a save state *for a specific game* in disguise. When you sleep your analogue pocket a save state is stored, when you wake your analogue pocket it attempts to load that save state. If you're using a flash cart that loads to a menu before it can load a specific game, it's impossible to load a state for a specific game before it is manually selected.
