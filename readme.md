# Definitive Guide to Playing Pokémon on the Analogue Pocket
- [introduction](#introduction)
- [optimal play method per game](#optimal-play-method-per-game)
- [play methods & pros/cons](#play-methods--proscons)
- [relevant Cores & surrounding nuance](#relevant-cores--surrounding-nuance)
- [relevant flash carts & surrounding nuance](#relevant-flash-carts--surrounding-nuance)
    - [Game Boy Color](#Game-Boy-Color)
    - [Game Boy Advanced](#Game-Boy-Advanced)
    - [micro SD cards](#micro-SD-cards)
- [manually reset RTC data](#manually-reset-RTC-data)
- [backing up / extracting save data](#backing-up--extracting-save-data)
- [convert save data (Virtual Console)](#convert-save-data-Virtual-Console)
- [acquiring the GS Ball in Pokémon Crystal](#acquiring-the-GS-Ball-in-Pokémon-Crystal)
- [interfacing with Pokémon Home](#interfacing-with-Pokémon-Home)
- [product links](#product-links)
- [cores / software / firmware](#cores--software--firmware)
- [relevant guides](#relevant-guides)
- [frequently asked questions](#frequently-asked-questions)

# introduction
Some Pokémon games are unique due to their utilization of real-time clock, aka RTC. RTC keeps track of time while you aren't playing, essentially it syncs in-game time with real-time. In-game events/functions such as Pokémon catchability, the Move Tutor, Kurt's Apricorn Pokéballs, certain Pokémon evolutions, berry growth, lotteries, Secret Base battles, etc. depend on RTC. This causes complications depending on what method you're using to play Pokémon games on the Analogue Pocket. Bulbagarden has a nice [write up](https://bulbapedia.bulbagarden.net/wiki/Time) on what time/RTC effects in each generation of Pokémon. Generation 2 is much more dependant on RTC than generation 3, but it's important enough in both generations that I wouldn't consider playing without functional RTC.

# optimal play method per game
### preface
- The below methods are selected as the optimal methods as they allow for in-game time to properly track (RTC) without de-sync, even when using Analogue Pocket's save state & sleep functionality.
- Note that when using the EZ-Flash Omega DE you must utilize "Standalone Mode" / "Mode B" for the Analogue Pocket's sleep function to work (see [relevant guides](#relevant-guides)). 
- See [product links](#product-links) & [cores / software / firmware](#cores--software--firmware) for purchase & download links.
- See [play methods & pros/cons](#play-methods--proscons) for detailed pro/cons of each play method.
### optimal play methods
- games with RTC
    - Silver -> budude's GBC core
    - Gold -> budude's GBC core
    - Crystal -> budude's GBC core
    - Ruby -> EZ-Flash Omega DE
    - Sapphire -> EZ-Flash Omega DE
    - Emerald -> EZ-Flash Omega DE
- games without RTC
    - Red -> budude's GBC core
    - Blue -> budude's GBC core
    - Green -> budude's GBC core
    - Yellow -> budude's GBC core
    - Fire Red -> GBA core
    - Leaf Green -> GBA core
- interop with Pokémon Stadium
    - BennVenn MBC3000
    - insideGadgets GBC RTC carts
- interop with Pokémon Pal Park
    - EZ-Flash Omega DE (Standalone Mode / Mode B)

# play methods & pros/cons
There are three methods of playing pokemon on the Analogue Pocket.
1. #### cores
    - pros
        - GBC RTC Core
            - time is tracked while you aren't playing the game
            - sleep/save states are fully functional
            - time does not desync with the use of sleep/save states
            - basically a flawless implementation
        - GBA Core
            - sleep/save states are partially functional
        - both
            - free
            - save files are easily accesible for backup
            - save data & RTC functionality is not dependant on the finite life of a non-rechargable battery
    - cons
        - GBA Core
            - time is only tracked when playing the game
            - time is not re-calculated when sleep/save states are loaded on cores that utilize said functionality
        - both
            - additional setup required  
            - incapable of interfacing with some Nintendo hardware/software (N64 Transfer Pak, Pal Park, etc.)
2. #### flash carts
    - pros
        - GBC carts
            - save states are partially functional
            - **EverDrive GB X7** - Time is recalculated when utilizing the cart's internal save state function. However, many users have reported that loading a save state breaks in-game saving.
            - **EZ-Flash Junior** - in-game clock can be reset via manipulation of cart's internal clock
            - **BennVenn MBC3000 & insideGadgets RTC carts** - compatible with N64 Gam Pak for use with Pokémon Stadium 1&2
        - GBA carts
            - save states are fully functional
            - time is recalculated when save states are loaded (always in sync)
            - **EZ-Flash Omega DE** - Mode B allows for use of the Pocket's sleep functionality
            - **EZ-Flash Omega DE** - Mode B allows for interop with Pokémon Pal Park
        - both
            - much cheaper than authentic carts in the grand scheme of things
            - time is tracked while you aren't playing
            - easy to replace internal batteries
            - save files are easily accessible for backup
    - cons
        - GBC carts
            - time is desynced when save states are loaded via the Analogue Pocket (see [manually reset RTC data](#manually-reset-RTC-data))
        - GBA carts
            - **EverDrive GBA Mini X5** - incompatible with Analogue Pocket's sleep feature
        - both
            - You typically require access to authentic Nintendo hardware to perform updates neccesary for flash carts to function with the Analogue Pocket.
            - costs money
            - additional setup required
            - RTC relies on internal batteries that eventually die 
3. #### authentic cartridges
    - pros
        - time is tracked while you aren't playing the game
        - sleep/save states are partially functional
        - no setup required
        - interfaces with official Nintendo hardware/software (N64 Transfer Pak, Pal Park, etc.)
        - karts r kool
    - cons
        - extremely expensive
        - time is not re-calculated when sleep/save states are loaded (desync)
        - gen 2 cartridge save data is lost when the cart's internal battery dies
        - gen 3 cartridge time is no longer tracked when the cart's internal battery dies
        - cartridge battery replacement requires soldering
        - additional hardware is required to backup save data
     
# relevant cores & surrounding nuance
- There are currently 2 GBC cores & 1 GBA core available for the Analogue Pocket.
- Only 1 of 3 cores currently supports RTC, and it's a GBC core.
- There are no GBA cores that support RTC, so you'll want to use a GBA flash cart. Several are mentioned below.
- I recommend installing all cores using [Pocket Sync](https://github.com/neil-morrison44/Pocket-sync), but make sure you select the proper GBC core, the one that supports RTC (budude2's core).
- direct links
    - [GBC by budude2](https://github.com/budude2/openfpga-GBC) (RTC implemented ✅)
    - GBA by budude2 (work in progress)
    - [GBC by spiritualized1997](https://github.com/spiritualized1997/openFPGA-GB-GBC) (RTC not implemented ❌)
    - [GBA by spiritualized1997](https://github.com/spiritualized1997/openFPGA-GBA) (RTC not implemented ❌)

# relevant flash carts & surrounding nuance
### preface
- Note that if you're only using the Analogue Pocket, [budude's GBC RTC core](https://github.com/budude2/openfpga-GBC) is the most reasonable option for GB/GBC. You only need a GBC cart if you're interfacing with other hardware.
- GBA flash carts cannot be used to play GBC games without utilizing emulation. This defeats the purpose of FPGA, and games are noticably letterboxed, taking up only a small fraction of the Pocket's display.
- It is likely *required* that you have authentic Nintendo hardware on hand to perform inital firmware updates. Most carts ship with old firmware that is incompatible with the Analogue Pocket.
- I would argue that the best combination of carts for use with the Analogue Pocket are the [BennVenn MBC3000](#BennVenn-MBC3000-compatible-w-N64-Game-Pak), and the [EZ-Flash Omega Definitive Edition](#EZ-Flash-Omega-Definitive-Edition-highly-recommended-). Why? Because this gives you the most compatibility with official Nintendo hardware/software (N64 Transfer Pak, Pal Park, etc). Functionality with the N64 Transfer Pak is particularly relevant given [the announcment of the Analogue 3D](https://x.com/Analogue/status/1713933239327273452?s=20).
### Game Boy Color
- #### [EverDrive GB X7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=EverDrive+GB+X7&qid=1700286142&sprefix=EverDrive+GB+%2Caps%2C138&sr=8-1)
    - 3x more expensive than the EZ-Flash Junior, albeit with a superior physical build quality.
    - When utilizing the cart's internal save state function, RTC data is recalculated upon loading a state, keeping in-game time in-sync with real time. However, for some users this seems to break the ability to save your game via the in-game saving mechanism.
    - When utilizing the Analogue Pocket's save state function, in-game time will become desynced with real time (see [manually reset RTC data](#manually-reset-RTC-data)).
    - Incompatible with N64 Transfer Pak, and thus Pokémon Stadium.
- #### [EZ-Flash Junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-EverDrive/dp/B08379XZWY/ref=sr_1_1?crid=27VHV05U1YVS0&keywords=ez-flash+jr&qid=1700286287&sprefix=ez-flash+jr%2Caps%2C124&sr=8-1)
    - **!!! important !!!**
        - an unlisted / hard to find [firmware](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) is currently required for the Junior to function with an Analogue Pocket
        - this unlisted firmware will cause your Junior to brick / die if you're not using a [fast enough micro SD card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
    - 3x cheaper than the EverDrive GB X7, albiet wtih an inferior physical build quality.
    - while time isn't recalculated after loading a save state, the in-game clock can be reset by manipulating the cart's internal clock
        1. set the internal clock 2 years ahead
        2. launch your game
        3. return the Junior's menu by pressing the button in the cart (press on front), or by resetting the cartrige via the anlogue Pocket's menu.
        4. re-sync the internal clock with real time
        5. launch your game
        6. follow the in-game prompts to re-set your in-game clock
    - Incompatible with N64 Transfer Pak, and thus Pokémon Stadium.
- #### [BennVenn MBC3000](https://BennVenn.myshopify.com/products/MBC3000-RTC-GBC-cart-v5) (**compatible w/ N64 Transfer Pak**)
    - Requires [BennVenn's Joey Jr](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr), or something comparable (like the [GB Operator](https://www.epilogue.co/product/gb-operator)), to flash games to the cartridge.
    - significantly less expensive that insideGadgets offerings
    - time is desynced when save states are loaded without use of external applications or in-game exploits (see [manually reset RTC data](#manually-reset-RTC-data))
    - Unlike other carts, there is no SD card, and only one game can be stored on the cart at a time.
    - As only one game is loaded at a time, *this cart **is compatible** with the N64 Transfer Pak / Pokémon Stadium*.
- #### [insideGadgets GBC RTC cart](https://shop.insidegadgets.com/product/gameboy-2mb-32kb-fram-mbc3-with-RTC-flash-cart/) (**compatible w/ N64 Transfer Pak**)
    - Requires [BennVenn's Joey Jr](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr), or something comparable (like the [GB Operator](https://www.epilogue.co/product/gb-operator)), to flash games to the cartridge.
    - significantly more expensive that BennVenn's MBC3000
    - time is desynced when save states are loaded without use of external applications or in-game exploits (see [manually reset RTC data](#manually-reset-RTC-data))
    - Unlike other carts, there is no SD card, and only one game can be stored on the cart at a time.
    - As only one game is loaded at a time, *this cart **is compatible** with the N64 Transfer Pak / Pokémon Stadium*.
- #### [insideGadgets GBC RTC LinkNLoad cart](https://shop.insidegadgets.com/product/gameboy-mbc3-RTC-linknload-usb-flash-cart-works-with-pokemon-games-hacks-like-cc/) (**compatible w/ N64 Transfer Pak**)
    - **Does not** require an additional cart flashing tool, you can flash games directly via the USB-C port on the card.
    - Significantly more expensive that BennVenn's MBC3000 & insideGadgets non "LinkNLoad" cart, but possibly more convenient as an additonal flasher is not required.
    - time is desynced when save states are loaded without use of external applications or in-game exploits (see [manually reset RTC data](#manually-reset-RTC-data))
    - Unlike other carts, there is no SD card, and only one game can be stored on the cart at a time.
    - As only one game is loaded at a time, *this cart **is compatible** with the N64 Transfer Pak / Pokémon Stadium*.
### Game Boy Advanced
- #### [EZ-Flash Omega Definitive Edition](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1) (**highly recommended 👑**)
    - 40% cheaper than the EverDrive GBA Mini X5 with similar build quality and *more features*
    - a physical switch on the outside of the cart allows you to enter standalone mode / Mode B (see [relevant guides](#relevant-guides))
        - Allows for use of the Analogue Pocket's sleep functionality.
        - Allows for interop with Pokémon [Pal Park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park) to transfer Pokémon from gen 3 to gen 4 via a Nintendo DS.
- #### [EZ-Flash Omega](https://www.amazon.com/EZ-Flash-MicroSDHC-Version-Latest/dp/B01GZMNRP6/ref=sr_1_2?crid=6NN7MN3GBTZT&dib=eyJ2IjoiMSJ9.SmTKXapduSgeZ_JdvicuRg4thNulTgxNWppXvD3cVmruPRG7yPAjotgKgyc1wKtwigxpazDeuFgHgnOV_zpsq1mn0Th_iDztT9kPZp5RSn1s009V88zbHYb2gZu2KCi1AXAahSIB0-D1KX4pFzYBNVapK8S44b1lRS1ymXw7bVqD1TB05gF5hRpm_DUvT8SIlbhwbS5v5MCekxO5ftuNDT7xiU0v1pjWvHZYN8TdPRg.dN_DrbgQmKs7ELYJycj41FE9W46kpq8ZMmUnn0-giik&dib_tag=se&keywords=EZ-Flash+Omega&qid=1710045811&sprefix=ez-flash+omeg%2Caps%2C157&sr=8-2)
    - much cheaper than the Omega DE & GBA Mini
    - Not compatible with stand alone cart functions, like Pokémon [Pal Park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park).
    - Battery is soldered in, making it much more difficult to replace.
- #### [EverDrive GBA Mini X5](https://krikzz.com/our-products/cartridges/everdrive-gba-mini.html)
    - 40% more expensive than the EZ-Flash Omega DE with similar build quality and *less features*
    - Not compatible with stand alone cart functions like Pokémon [Pal Park](https://bulbapedia.bulbagarden.net/wiki/Pal_Park).
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
    - the Omega DE requires that cards >32GB must be formatted as exfat
- It is my recommendation that you use 32GB cards for everything to make things simple, realistically you'll never fill 32GB with GB/GBC/GBA roms.
- As mentioned above the EZ-Flash Junior specifically requires a fast micro SD card to function, the others will benefit from a fast micro SD card as well.
- I recommend [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro SD card
 
# manually reset RTC data

- [PKHeX](https://projectpokemon.org/home/files/file/1-pkhex/) (gen 2&3)
    - Some flash carts store their RTC data in a separate file from the save file, you may need to delete the RTC file as part of the RTC reset process.
    - steps to reset RTC
        1. backup save data
        2. run PKHeX
        3. load backed up save file
        4. select the "SAV" tab
        5. select "Clock (RTC)"
        6. click "Yes"
        7. export edited save data to new file (File > Export SAV)
        8. re-inject your edited save data into your cart/core
        9. set time when prompted in-game
- gen 2
    - [in-game exploit](https://www.youtube.com/watch?v=Vupz6vwylGM&t)
    - EZ-Flash Junior
        1. set the internal clock 2 years ahead
        2. launch your game
        3. Return the Junior's menu by pressing the button in the cart (press on front), or by resetting the cartrige via the anlogue Pocket's menu.
        4. re-sync the internal clock with real time
        5. launch your game
        6. follow the in-game prompts to re-set your in-game clock
    - rom hacks
- gen 3
    - **authentic carts** - desolder the internal battery, solder in a new one.
    - rom hacks
 
# backing up / extracting save data
### preface
Note that after you extract your save, it is very likely you mess up your RTC data. See the [manually reset RTC data](#manually-reset-RTC-data) section in this guide to learn how you can reset your RTC data as needed.
### cores & flash carts
- As mentioned in the pro/cons section, backing up / extracting save data created by cores & flash carts is trivial.
- It would be impractical to list save locations for all flash carts in this guide, best to refer to the official documentation of the cart you're using. See [relevant guides](#relevant-guides) for product documentation, and video guides that should cover this topic.
- Saves created by Cores can be found in the `Saves` folder in the root of the Micro SD card in your Analogue Pocket.
### retail cartridges
- As mentioned in the pro/cons section, you need additional hardware to backup/extract saves on retail cartridges.
- The two most popular cart/save dumping tools are the BennVenn Joey Jr. and the GB Operator.
- See [product links](#product-links) and [relevant guides](#relevant-guides) for purchase links and more information regarding these products.

# convert save data (Virtual Console)
### preface
- there are a couple reasons why you'd want to transfer your save data between your Pocket and your 2/3DS virtual console
    1. To Capture Celebi in Pokémon Crystal (see [acquiring the GS Ball in Pokémon Crystal](#acquiring-the-GS-Ball-in-Pokémon-Crystal)).
    2. To transfer Pokémon into Pokémon Home (see [interfacing with Pokémon Home](#interfacing-with-Pokémon-Home)).
- To transfer saves into the Virtual Console versions, you'll need a modded 2/3DS running Checkpoint. See [relevant guides](#relevant-guides) below for more info.
- See [backing up / extracting save data](#backing-up--extracting-save-data) for instructions as to how you acquire your `.sav` files.
### gen 1
- Simply rename your save `[game name].sav` file to `sav.dat` before injecting it with Checkpoint.
- When you extract your save from the Virtual Console version using Checkpoint, you will need to rename the file from `sav.dat` to `[game].sav`, where `[game]` is the name of the rom (ie `pokemonyellow.sav`).
- There appears to be an extra KB of data in Gen 1 Virtual Console saves that prevents them from being loaded in PKHeX. To fix this, you need to load your save file via the Analogue Pocket, and overwrite it in-game. This should recondition the file, making it compatible with PKHeX again.
### gen 2
- Generation 2 save files need to be converted when moved between Virtual Console & your Analogue Pocket.
- [normal save to Virtual Console converter](https://inject.sigkill.tech/converter/3Dsvc)
    - Note that once converted to a VC save, save files will no longer be compatible with PKHeX. Use the next converter to solve this.
- [Virtual Console to normal save converter](https://savefileconverter.com/#/flash-carts)
    - After conversion with this tool, you will need to rename the converted save to `[game].sav`, where `[game]` is the name of the rom (ie `pokemoncrystal.sav`).

# acquiring the GS Ball in Pokémon Crystal
- see [convert save data (Virtual Console)](#convert-save-data-Virtual-Console) for more context.
- steps
    1. save in-front of Lance (doesn't have to be your first time battling him)
    2. backup your save data
    3. convert your save data to VC data using [this tool](https://inject.sigkill.tech/converter/3Dsvc)
    4. transfer your save into Crystal Virtual Console edition using checkpoint (see [relevant guides](#relevant-guides))
    5. defeat lance
    6. enter the Goldenrod City Pokémon Center
    7. exit the Goldenrod City Pokémon Center
    8. receive the GS Ball
    9. backup your save data using checkpoint (see [relevant guides](#relevant-guides))
    10. re-convert you save data using [this tool](https://savefileconverter.com/#/flash-carts)
        - After conversion with this tool, you may need to rename the converted save to `[game].sav`, where `[game]` is the name of the rom (ie `pokemoncrystal.sav`).
    12. re-inject your save into your core/cart

# interfacing with Pokémon Home
**Note that you can can transfer Gen 4-6 from 3DS into Pokémon Home *without using retail cartridges* as mentioned in https://github.com/ninbura/pokemon-on-the-Analogue-Pocket/issues/3**.
- gen 1&2
   - backup your save file
   - [load your save file onto the virtual console version of said game via a modded 2/3DS running checkpoint](https://www.youtube.com/watch?v=pe9mw25mHGA)
   - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3Ds-switch-pokemon-go) guide
- gen 3
   - method 1 (authentic carts & EZ-Flash Omega DE only)
      - if you're using the EZ-Flash Omega DE the game must be running in Mode B
      - [use a Nintendo ds + Pal Park to trade Pokémon from gen 3 to gen 4](https://bulbapedia.bulbagarden.net/wiki/Pal_Park)
      - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3Ds-switch-pokemon-go) guide
   - method 2
      - backup your gen 3 save file
      - [use desume to emulate Pal Park transfer](https://www.youtube.com/watch?v=o0RkljY3UMw) using your save file
      - [load your save file onto an authentic Gen 4 cart using a modded 3DS running checkpoint](https://projectpokemon.org/home/tutorials/save-editing/managing-3Ds-saves/using-checkpoint-r25/)
      - from there follow [this](https://www.gamerevolution.com/guides/633108-transfer-to-pokemon-home-from-ds-3Ds-switch-pokemon-go) guide

# product links
- [EverDrive GB X7](https://www.amazon.com/EverDrive-GB-X7-Game-Boy/dp/B07JZG3452/ref=sr_1_1?crid=1L2H6CSD8PIKM&keywords=EverDrive+GB+X7&qid=1700286142&sprefix=EverDrive+GB+%2Caps%2C138&sr=8-1)
- [EZ-Flash Junior](https://www.amazon.com/EZ-Flash-EZ-FlashJr-Original-EverDrive/dp/B08379XZWY/ref=sr_1_2?crid=2827XS0JEDDSF&keywords=ez+flash+jr&qid=1677688333&sprefix=ez+flash+j%2Caps%2C200&sr=8-2&ufe=app_do%3Aamzn1.fos.08f69ac3-fd3D-4b88-bca2-8997e41410bb)
- [BennVenn MBC3000](https://BennVenn.myshopify.com/products/MBC3000-RTC-GBC-cart-v5)
- [insideGadgets GBC RTC cart](https://shop.insidegadgets.com/product/gameboy-2mb-32kb-fram-mbc3-with-RTC-flash-cart/)
- [insideGadgets GBC RTC LinkNLoad cart](https://shop.insidegadgets.com/product/gameboy-mbc3-RTC-linknload-usb-flash-cart-works-with-pokemon-games-hacks-like-cc/)
- [BennVenn Joey Jr](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr)
- [GB Operator](https://www.epilogue.co/product/gb-operator)
- [EZ-Flash Omega](https://www.amazon.com/EZ-Flash-MicroSDHC-Version-Latest/dp/B01GZMNRP6/ref=sr_1_2?crid=6NN7MN3GBTZT&dib=eyJ2IjoiMSJ9.SmTKXapduSgeZ_JdvicuRg4thNulTgxNWppXvD3cVmruPRG7yPAjotgKgyc1wKtwigxpazDeuFgHgnOV_zpsq1mn0Th_iDztT9kPZp5RSn1s009V88zbHYb2gZu2KCi1AXAahSIB0-D1KX4pFzYBNVapK8S44b1lRS1ymXw7bVqD1TB05gF5hRpm_DUvT8SIlbhwbS5v5MCekxO5ftuNDT7xiU0v1pjWvHZYN8TdPRg.dN_DrbgQmKs7ELYJycj41FE9W46kpq8ZMmUnn0-giik&dib_tag=se&keywords=EZ-Flash+Omega&qid=1710045811&sprefix=ez-flash+omeg%2Caps%2C157&sr=8-2)
- [EZ-Flash Omega Definitive edition](https://www.amazon.com/EZ-Definitive-GBA-IMPEX-Source/dp/B097NQ6HV8/ref=sr_1_1?crid=318IO187XHCX6&keywords=ez+flash+omega+definitive+edition&qid=1700285292&sprefix=ezflash+%2Caps%2C157&sr=8-1)
- [EverDrive GBA Mini x5](https://krikzz.com/our-products/cartridges/everdrive-gba-mini.html)
- [micro SD card](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13)
- [EZ-Flash Junior, EverDrive GB X7, BennVenn MBC3000, & EverDrive GBA Mini battery replacement](https://www.amazon.com/dp/B014WXZO0G?psc=1&smid=A19DY5EK03NION&ref_=chk_typ_imgToDp) (CR1220)
- [EZ-Flash Omega DE battery replacement](https://www.amazon.com/dp/B001ERBLME?psc=1&smid=AI62U825BKVWC&ref_=chk_typ_imgToDp) (CR1025)
- [insideGadgets GBC carts battery replacement](https://www.amazon.com/Duracell-Lithium-Battery-Lasting-Count/dp/B07G7L5M4J/ref=sr_1_5?crid=S8BXXRKK17U9&dib=eyJ2IjoiMSJ9.-RhhqUEnEOUs7D29Trl6RogHqs206TL6e6n5L7pSAl1br6q03Tfm3K4nS6fBIe4rznz_6OgGFnjYbd1KIaXPH_2DlClztaNuUo1962X7ICQRFpPhqZ0fNok0NfB2E-yT3koLoGA5fbcgxq1mmAxANS5WWkHt50NRjaB8x79fklkhFerQuPeiivzhDLxWabxHeCGZMOv65BHLEvpN_JZ6oLkV8QoNHC3fpNaVlp1j3tdRsRROgEd0_KkfLDRMTy2arffaFUnGANqODgo-P4WiB2puy9XqRisKxKLrXTz1CBo.4emsr5u1FMxmbiqDdSz23-MjSU7cgupwFs0Wx0yXqLE&dib_tag=se&keywords=cr2025&qid=1710049061&sprefix=cr2025%2Caps%2C123&sr=8-5) (CR2025)

# cores / software / firmware
- cores/software
    - [Pocket Sync](https://github.com/neil-morrison44/Pocket-sync/releases) (gui core installer | [guide](https://github.com/neil-morrison44/Pocket-sync))
    - [fat32 formatter](http://ridgecrop.co.uk/index.htm?guiformat.htm) (required for >32GB micro SD cards used with EverDrive carts)
    - [PKHeX](https://projectpokemon.org/home/files/file/1-pkhex/)
- firmware
    - [EverDrive GB X7](https://krikzz.com/pub/support/everdrive-gb/x-series/OS/) ([guide](https://ddavegames.neocities.org/guides/everdrivegbx7/))
    - [EZ-Flash Junior](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) (**use this specific firmware** with [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) specific micro SD card | [guide](https://www.youtube.com/watch?v=inus-2l5oeg))
    - [BennVenn Joey Jr.](https://BennVenn.myshopify.com/products/usb-GB-c-cart-dumper-the-joey-jr) ([guide](https://BennVenn.myshopify.com/pages/the-joey-Junior-GB-GBC-GBA-cart-dumper-and-flasher))
    - [EZ-Flash Omega DE](https://www.ezflash.cn/download/) ([guide](https://www.ezflash.cn/omegade-en.pdf#page=10))
    - [EverDrive GBA Mini](https://krikzz.com/pub/support/everdrive-gba/OS/) ([guide](https://ddavegames.neocities.org/guides/everdrivegbx7/))

# relevant guides
- [Pocket Sync](https://github.com/neil-morrison44/Pocket-sync/blob/main/README.md)
- [EverDrive GB X7](https://www.youtube.com/watch?v=p9IYgMTvl2c)
- [EZ-Flash Junior](https://www.youtube.com/watch?v=rqeFD8SRbVA) (please use [this](https://www.ezflash.cn/zip/ezjunior-fw5-0918.zip) firmware & [this](https://www.amazon.com/Sandisk-MicroSDHC-V30-32GB-Extreme/dp/B01LRW8FWY/ref=sr_1_13?crid=387E7GIAA8IBU&keywords=extreme+pro+micro+SD+card&qid=1700288123&sprefix=extreme+pro+mi%2Caps%2C130&sr=8-13) micro SD card)
- [BennVenn Joey Jr](https://BennVenn.myshopify.com/pages/the-joey-Junior-GB-GBC-GBA-cart-dumper-and-flasher)
- [GB Operator](https://support.epilogue.co/hc/en-us/articles/360018602980-GB-Operator-FAQ)
- [EZ-Flash Omega DE manual](https://www.ezflash.cn/omegade-en.pdf)
- [EZ-Flash Omega DE](https://www.youtube.com/watch?v=CBPoAjBfV0M&t)
- EZ-Flash Omega DE Standalone Mode / Mode B ([manual](https://www.ezflash.cn/omegade-en.pdf#page=13) | [video tutorial](https://youtu.be/MSWgdfbpgPI?t=129))
- [EverDrive GBA Mini](https://www.youtube.com/watch?v=epLif4ju4F0)
- [replace batteries in flash carts](https://GBAtemp.net/threads/ez-flash-omega-de-replacing-the-battery.612300/)
- [backup saves on authentic carts](https://www.reddit.com/r/Gameboy/comments/4w8xjf/guide_how_to_backup_your_game_save_files/)
- [mod 2/3DS systems & load checkpoint for save management](https://www.youtube.com/watch?v=lAOvQTuVW5o)

# frequently asked questions
### Why do I want to interface my gen 1&2 games with the N64 Transfer Pack / Pokémon Stadium 1&2?
Pokémon Stadium 1&2 provide these unique benefits
- much easier Pokémon box orginzation
- much faster / bulk transfer of Pokémon between games
- [shiny hunting eggs in gen 2](https://www.youtube.com/watch?v=Nywbm5ZZZvQ&t)
    
### Why can't most flash carts interface with specialized Nintendo hardware/software (Transfer Pak, Pal Park, etc)?
Most flash carts launch to a menu in-which you first have to select a rom to interact with it. The BennVenn & insideGadgets carts only ever have one game flashed at time. Likewise, the Omega DE has the option (Mode B) to run a single game . This allows these carts to interface with specialized Nintendo hardware/software, as they are viewed as single authentic game by the receiving hardware.

### Why can't most flash carts utilize the Analogue Pocket's sleep functionality?
Similarly to my previous answer, only carts that offer a standalone game mode can utilize the Analogue Pocket's sleep functionality. This is because this sleep functionality is really a save state *for a specific game* in disguise. When you sleep your Analogue Pocket a save state is stored, when you wake your Analogue Pocket it attempts to load that save state. If you're using a flash cart that loads to a menu before it can load a specific game, it's impossible to load a state for a specific game before it is manually selected.
