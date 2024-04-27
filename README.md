# Thunderstore package updator

## Purpose of this script
This script is used to obtain the latest versions of a Thunderstore package list your povide. 
It will automatically update the version number in the `packagelist.txt` file you provide and create a new packagelist_updated.txt file with the updated versions from Thunderstore.

## How to use example

### arguments
- `--input_file` default `package_list.txt` : The file that must exist in the same directory as the script. This file should contain the list of packages you want to update.
- `--output_file` default `package_list_updated.txt` : The file that will be created with the updated versions of the packages.
- `--server_delay` default `1` : The delay between each request to the Thunderstore server. This is to prevent the server from blocking you for making too many requests in a short period of time. Not sure what the limit is, but I would recommend not going below 1 second.

## Image of the script running
![image](img.png)


Below is an example `packagelist.txt` and its expected format.

# Example package file

### Note we have 4 categories of packages and these must be present in the file.
- Core
- Cosmetics
- Cosmos
- Extras

```text
Core
          "BepInEx-BepInExPack-5.4.2100",
          "mrgrm7-LethalCasino-0.5.2",
          "x753-Mimics-2.5.0",
          "veri-ShipWindows-2.0.6",
          "Rolevote-The_Fiend-1.0.5",
          "LethalResonance-LETHALRESONANCE-4.2.4",
          "FlipMods-TooManyEmotes-2.1.12",
          "Evaisa-LethalThings-0.10.4",
          "IntegrityChaos-Diversity-2.0.3",
          "AinaVT-LethalConfig-1.4.2",
          "EladNLG-EladsHUD-1.2.1",
          "taffyko-NameplateTweaks-1.0.6",
          "Jordo-NeedyCats-1.2.1",
          "Woecust-Immersive_Visor-0.5.2",
          "TheDeadSnake-Touchscreen-1.1.2",
          "saint_kendrick-Lethal_Doors-1.0.4",
          "AnythingGoesGit-MoreDeathNotes-1.4.0",
          "Monkeytype-HideChat-1.0.0",
          "XuXiaolan-ImmersiveScrap-1.0.0",
          "AmesBoys-ImmortalSnail-0.7.4",
          "Kittenji-Herobrine-1.3.3",
          "qwbarch-Mirage-1.6.0",
          "mrov-WeatherTweaks-0.5.4",
          "Ryokune-Better_Lobbies-1.1.1",
          "BlueAmulet-LCBetterClock-1.0.3",
          "Entity378-SellBodiesFixed-1.8.1",
          "PopleZoo-BetterItemScan-3.0.2",
          "Orion-DontBlink-1.1.1",
          "Zaggy1024-OpenBodyCams-1.3.0",
          "LegoMaster3650-FairGiants-1.1.1",
          "TanmanG-Forest_Giant_Motionsense-1.0.2",
          "vasanex-ItemQuickSwitch-1.1.0",
          "lethal_coder-BetterBrackenModel-1.2.4",
          "Piggy-MaskedAIRevamp-0.2.1",
          "Coppertiel-MaskedEnemyOverhaulFork-3.3.0",
          "monkes_mods-JumpDelayPatch-1.0.1",
          "mrov-LethalRichPresence-0.5.8",
          "Nases-Quick_Drop-1.0.1",
          "lethal_coder-BetterCoilheadModel-1.1.4",
          "Scoliosis-StrangerThingsMod-0.0.32",
          "CTNOriginals-CrossHair-1.1.2",
          "Pooble-LCBetterSaves-1.7.3",
          "Ccode_lang-SirenHead-1.4.3",
          "zealsprince-Locker-1.1.2",
          "Sparble-FacelessStalker-1.1.3",
          "XuXiaolan-TheGiantSpecimens-2.0.5",
          "zealsprince-Malfunctions-1.8.5",
          "Kittenji-Football-1.1.7",
          "mrov-IntroTweaks-1.0.0",
          "FutureSavior-Hold_Scan_Button-1.1.1",
          "darmuh-darmuhsTerminalStuff-3.0.4",
          "NiceHairs-Symbiosis-1.0.5",
          "NutNutty-SellTracker-1.2.1",
          "DBJ-ShipScanRange-0.0.1",
          "x753-Peepers-0.9.7",
          "CHILLAX-ChillaxSCRAPS-0.6.0",
          "Kittenji-Dont_Touch_Me-1.2.2",
          "mrov-UnlockableDefaults-0.0.1",
          "taffyko-QuickQuitToMenu-1.0.1",
          "PloufJPEG-CompanyCreatures-0.2.0",
          "Toskan4134-LethalRegeneration-1.3.0",
          "DiFFoZ-BepInEx_Faster_Load_AssetBundles_Patcher-0.5.0",
          "Darkbrewery-Emblem-1.3.2",
          "Nyxchrono-DoorBreach-1.1.0",
          "Bob123-Haunted_Harpist-1.3.11",
          "TheWeavers-NightmareFoxy-1.1.10",
          "Sconeys-Gnomes-2.1.15",
          "lethal_coder-AdvanceModChecker-1.0.2",
          "MoonJuice-BuyRateSettings-1.3.2",
          "Swaggies-BetterPaycheck-0.9.0",
          "mrov-LightsOut-0.1.3",
          "MaxWasUnavailable-LethalModDataLib-1.2.2",
          "stefan750-LCUltrawide-1.1.1",
          "BMX-LobbyCompatibility-1.1.0",
          "Yoshify-DiscJockey-1.2.1",
          "Sconeys-abandonedcompanyassets-0.15.79",
          "coderCleric-Poltergeist-1.0.2,
          "Clemonade_Stand-ClemsEscapeMusic-3.0.5",
          "Jordo-BombCollar-1.0.0",
          "axd1x8a-LCAmmoCheck-1.1.1",
          "loaforc-FacilityMeltdown-2.6.4",
          "Scoliosis-StrangerThingsMod-0.0.32",
          "YaBoiDucki-men_stalker-1.2.1",
          "MoonsweptTeam-Moonswept-0.5.5",
          "Aubarino-Sentinel_Mod-1.1.0",
          "BaronDrakula-MoreCounterplay-1.2.1",
          "sfDesat-Celestial_Tint-1.2.0"

Cosmetics
          "	Shinobi-MCC-1.0.0",
          "	404_Dom-Doms_Basic_Suit_Colors-1.4.4",
          "FoxGod-ThiccCompanyModelReplacement-2.0.1",
          "x753-More_Suits-1.4.3",
          "Verity-TooManySuits-1.0.9",
          "RT0405-TooManySuitsInWorldButtons-1.0.3"

Cosmos
          "Magic_Wesley-Wesleys_Moons-3.1.10",
          "Zingar-Atlas_Abyss-1.1.8",
          "skidz-PoolRooms-0.1.20",
          "Tolian-EchoReach-0.5.5",
          "Tolian-Celestria-0.7.1",
          "Dantor-Dantors_Mental_Hospital-1.2.2",
          "AudioKnight-StarlancerMoons-1.6.1",
          "Major_And_Skiz-MoreInteriors-2.5.0",
          "scoopy-Scoopys_Variety_Mod-1.2.0",
          "Piggy-LC_Office-1.1.27",
          "Tolian-Maritopia-0.6.0",
          "Tolian-PsychSanctum-0.5.2",
          "sfDesat-Celest-1.1.0",
          "Tolian-Harloth-0.2.5",
          "Tolian-Zenit-0.3.0",
          "RosiePies-Sector0_Interior-1.1.4",
          "LethalMatt-Bozoros-1.0.1",
          "Tolian-Nimbus-0.1.5",
          "Tolian-Azure-0.2.0",
          "Tolian-Spectralis-0.2.0",
          "Tolian-Crystallum-0.2.3",
          "Tolian-Echelon-0.1.8

Extras
        "IAmBatby-LethalLevelLoader-1.2.2",
        "mrov-MrovLib-0.0.6",
        "Aubarino-AubPiggybackAPI-1.0.1",
        "ShaosilGaming-GeneralImprovements-1.2.3",
        "BGN-PizzaTowerEscapeMusic-2.4.0",
        "Hardy-LCMaxSoundsFix-1.1.0",
        "Lordfirespeed-OdinSerializer-2022.11.9",
        "xilophor-LethalNetworkAPI-2.1.7",
        "qwbarch-BarchLib-1.0.0",
        "Bobbie-NAudio-2.2.2",
        "Bobbie-UniTask-2.5.0",
        "Evaisa-HookGenPatcher-0.0.5",
        "Zaggy1024-PathfindingLagFix-1.2.1",
        "Kittenji-NavMeshInCompany-1.0.3",
        "sfDesat-ViewExtension-1.1.0",
        "ViViKo-ItemClippingFix-1.1.4",
        "Rune580-LethalCompany_InputUtils-0.7.4",
        "NotAtomicBomb-TerminalApi-1.5.4",
        "no00ob-LCSoundTool-1.5.1",
        "Clementinise-CustomSounds-2.3.2",
        "Evaisa-LethalLib-0.15.1",
        "Ozone-BepInUtils-1.2.1",
        "fumiko-CullFactory-1.1.0",
        "loaforc-loaforcsSoundAPI-1.0.10",
        "mrov-MainMenuVersion-0.0.1",
        "AudioKnight-StarlancerAIFix-3.6.0",
        "IntegrityChaos-LCCutscene-1.0.0",
        "IntegrityChaos-GraphicsAPI-1.0.0",
        "SylviBlossom-SmartItemSaving-1.2.1",
        "mattymatty-AsyncLoggers-1.6.2",
        "NiceHairs-NuclearLib-1.0.4",
        "BunyaPineTree-ModelReplacementAPI-2.4.4",
        "HGG-JigglePhysicsPlugin-1.1.2",
        "AdiBTW-Loadstone-0.0.6",
        "TheWeavers-LethalBestiary-1.2.1",
        "Sigurd-CSync-4.1.0"
```