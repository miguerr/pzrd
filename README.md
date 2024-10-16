
![Arte PZRD](https://github.com/user-attachments/assets/e07fac06-bbac-43c1-a744-8813db5495ec)

</br>
</br>
</br>

<h1 align="center"><strong>« BASIC INFO »</strong></h1>

</br>

<h4 align="center">
Current PZ Version: 41.78.16<br/>
Last Wipe: 16/10/2024<br/>
Player Capacity: 4<br/>
Active Mods: 0
</h4>

</br>
</br>

<h1 align="center"><strong>« TOOLS »</strong></h1>

</br>

<h4 align="center">Official PZ Map<br/></h4>
  <h4 align="center"><a href="https://map.projectzomboid.com"> Official Project Zomboid Map </a></h4>
  <h4 align="center"><a href="https://github.com/blind-coder"> Github </a></h4>
 
  <br/>
  <br/>
  
  <h4 align="center">Map Cell Checker<br/></h4>
  <h4 align="center"><a href="https://rakib-ryan.itch.io/is-this-cell-taken"> Is This Cell Taken? </a></h4>
  <h4 align="center"><a href="https://github.com/RakibRyan"> Github </a></h4>
</h4>

</br>
</br>

<h1 align="center"><strong>« GAME SETTINGS »</strong></h1>

</br>

<details>
  
  <summary>pzserver.ini - This is the main config file for server options.</summary>
  
```ruby
# Players can hurt and kill other players
PVP=true

# Game time stops when there are no players online
PauseEmpty=true

# Toggles global chat on or off.
GlobalChat=true

ChatStreams=s,r,a,w,y,sh,f,all

# Clients may join without already having an account in the whitelist. If set to false, administrators must manually create username/password combos.
Open=true

# The first welcome message visible in the chat panel. This will be displayed immediately after player login. you can use RGB colours to chance the colour of the welcome message. You can also use <LINE> to create a separate lines within your text.
# Use: <RGB:1,0,0> This message will show up red!
ServerWelcomeMessage=Welcome to PZRD! <LINE> <LINE> Click the Gear icon to customize chat. <LINE> <LINE> Happy surviving!

# Add unknown usernames to the whitelist when players join. Clients will supply their own username/password on joining. (This is for Open=true servers)
AutoCreateUserInWhiteList=false

# Display usernames above player's heads in-game.
DisplayUserName=true

# Display first & last name above player's heads.
ShowFirstAndLastName=false

# Force every new player to spawn at these set x,y,z world coordinates. Find desired coordinates at map.projectzomboid.com. (Ignored when 0,0,0)
SpawnPoint=0,0,0

# Players can enter and leave PVP on an individual basis. A player can only hurt another player when at least one of them is in PVP mode - as shown by the unobscured skull and crossbones on the left of the screen. When SafetySystem=false, players are free to hurt each other at any time if PVP is enabled.
SafetySystem=true

# Display a skull icon over the head of players who have entered PVP mode
ShowSafety=true

# The time it takes for a player to enter and leave PVP mode\nMinimum=0 Maximum=1000 Default=2
SafetyToggleTimer=2

# The delay before a player can enter or leave PVP mode again, having recently done so\nMinimum=0 Maximum=1000 Default=3
SafetyCooldownTimer=3

# Item types new players spawn with.\nSeparate multiple item types with commas.\nExample: Base.Axe,Base.Bag_BigHikingBag
SpawnItems=

# Default starting port for player data. If UDP, this is this one of two ports used.\nMinimum=0 Maximum=65535 Default=16261
DefaultPort=27020

# Minimum=0 Maximum=65535 Default=16262
UDPPort=27021

# Reset ID determines if the server has undergone a soft-reset. If this number does match the client, the client must create a new character. Used in conjunction with PlayerServerID. It is strongly advised that you backup these IDs somewhere\nMinimum=0 Maximum=2147483647 Default=451305027
ResetID=6361100

# Enter the mod loading ID here. It can be found in \Steam\steamapps\workshop\modID\mods\modName\info.txt
Mods=

# Enter the foldername of the mod found in \Steam\steamapps\workshop\modID\mods\modName\media\maps\
Map=Muldraugh, KY

# Kick clients whose game files don't match the server's.
DoLuaChecksum=true

DenyLoginOnOverloadedServer=true

# Shows the server on the in-game browser. (Note: Steam-enabled servers are always visible in the Steam server browser)
Public=false

# Name of the server displayed in the in-game browser and, if applicable, the Steam browser
PublicName=PZRD

# Description displayed in the in-game public server browser. Typing \n will create a new line in your description
PublicDescription=Read me at bitly

# Maximum number of players that can be on the server at one time. This excludes admins.
# WARNING: Server player counts above 32 will potentially result in poor map streaming and desync. Please advance with caution.\nMinimum=1 Maximum=100 Default=32
MaxPlayers=4

# Ping limit, in milliseconds, before a player is kicked from the server. (Set to 100 to disable)\nMinimum=100 Maximum=2147483647 Default=400
PingLimit=400

# After X hours, all containers in the world will respawn loot. To spawn loot a container must have been looted at least once. Loot respawn is not impacted by visibility or subsequent looting.\nMinimum=0 Maximum=2147483647 Default=0
HoursForLootRespawn=0

# Containers with a number of items greater, or equal to, this setting will not respawn\nMinimum=1 Maximum=2147483647 Default=4
MaxItemsForLootRespawn=4

# Items will not respawn in buildings that players have barricaded or built in
ConstructionPreventsLootRespawn=true

# Remove player accounts from the whitelist after death. This prevents players creating a new character after death on Open=false servers
DropOffWhiteListAfterDeath=false

# All forms of fire are disabled - except for campfires
NoFire=false

# If checked, every time a player dies a global message will be displayed in the chat
AnnounceDeath=false

# The number of in-game minutes it takes to read one page of a book\nMinimum=0.00 Maximum=60.00 Default=1.00
MinutesPerPage=1.0

# Loaded parts of the map are saved after this set number of real-world minutes have passed. (The map is usually saved only after clients leave a loaded area)\nMinimum=0 Maximum=2147483647 Default=0
SaveWorldEveryMinutes=0

# Both admins and players can claim safehouses
PlayerSafehouse=false

# Only admins can claim safehouses
AdminSafehouse=false

# Allow non-members to enter a safehouse without being invited
SafehouseAllowTrepass=true

# Allow fire to damage safehouses
SafehouseAllowFire=true

# Allow non-members to take items from safehouses
SafehouseAllowLoot=true

# Players will respawn in a safehouse that they were a member of before they died
SafehouseAllowRespawn=false

# Players must have survived this number of in-game days before they are allowed to claim a safehouse\nMinimum=0 Maximum=2147483647 Default=0
SafehouseDaySurvivedToClaim=0

# Players are automatically removed from a safehouse they have not visited for this many real-world hours\nMinimum=0 Maximum=2147483647 Default=144
SafeHouseRemovalTime=144

# Governs whether players can claim non-residential buildings.
SafehouseAllowNonResidential=false

# Allow players to destroy world objects with sledgehammers
AllowDestructionBySledgehammer=true

# Allow players to destroy world objects only in their safehouse (require AllowDestructionBySledgehammer to true).
SledgehammerOnlyInSafehouse=false

# Kick players that appear to be moving faster than is possible. May be buggy -- use with caution.
KickFastPlayers=false

# ServerPlayerID determines if a character is from another server, or single player. This value may be changed by soft resets. If this number does match the client, the client must create a new character. This is used in conjunction with ResetID. It is strongly advised that you backup these IDs somewhere
ServerPlayerID=804159479

# The port for the RCON (Remote Console)\nMinimum=0 Maximum=65535 Default=27015
RCONPort=27015

# RCON password (Pick a strong password)
RCONPassword=S1eFwUeiMbdh

# Enables global text chat integration with a Discord channel
DiscordEnable=false

# Discord bot access token
DiscordToken=

# The Discord channel name. (Try the separate channel ID option if having difficulties)
DiscordChannel=

# The Discord channel ID. (Use if having difficulties with Discord channel name option)
DiscordChannelID=

# Clients must know this password to join the server. (Ignored when hosting a server via the Host button)
Password=PZRD2024

# Limits the number of different accounts a single Steam user may create on this server. Ignored when using the Hosts button.\nMinimum=0 Maximum=2147483647 Default=0
MaxAccountsPerUser=0

# Allow co-op/splitscreen players
AllowCoop=true

# Players are allowed to sleep when their survivor becomes tired, but they do not NEED to sleep
SleepAllowed=false

# Players get tired and need to sleep. (Ignored if SleepAllowed=false)
SleepNeeded=false

KnockedDownAllowed=true

SneakModeHideFromOtherPlayers=true

# List Workshop Mod IDs for the server to download. Each must be separated by a semicolon. Example: WorkshopItems=514427485;513111049
WorkshopItems=

# Show Steam usernames and avatars in the Players list. Can be true (visible to everyone), false (visible to no one), or admin (visible to only admins)
SteamScoreboard=true

# Enable the Steam VAC system
SteamVAC=true

# Attempt to configure a UPnP-enabled internet gateway to automatically setup port forwarding rules. The server will fall back to default ports if this fails
UPnP=true

# VOIP is enabled when checked
VoiceEnable=true

# The minimum tile distance over which VOIP sounds can be heard.\nMinimum=0.00 Maximum=100000.00 Default=10.00
VoiceMinDistance=10.0

# The maximum tile distance over which VOIP sounds can be heard.\nMinimum=0.00 Maximum=100000.00 Default=100.00
VoiceMaxDistance=100.0

# Toggle directional audio for VOIP
Voice3D=true

# Minimum=10.00 Maximum=150.00 Default=70.00
SpeedLimit=70.0

LoginQueueEnabled=false

# Minimum=20 Maximum=1200 Default=60
LoginQueueConnectTimeout=60

# Set the IP from which the server is broadcast. This is for network configurations with multiple IP addresses, such as server farms
server_browser_announced_ip=

# Players can respawn in-game at the coordinates where they died
PlayerRespawnWithSelf=false

# Players can respawn in-game at a split screen / Remote Play player's location
PlayerRespawnWithOther=false

# Governs how fast time passes while players sleep. Value multiplies the speed of the time that passes during sleeping.\nMinimum=1.00 Maximum=100.00 Default=40.00
FastForwardMultiplier=40.0

# Safehouse acts like a normal house if a member of the safehouse is connected (so secure when players are offline)
DisableSafehouseWhenPlayerConnected=false

# Players can create factions when true
Faction=true

# Players must survive this number of in-game days before being allowed to create a faction\nMinimum=0 Maximum=2147483647 Default=0
FactionDaySurvivedToCreate=0

# Number of players required as faction members before the faction owner can create a group tag\nMinimum=1 Maximum=2147483647 Default=1
FactionPlayersRequiredForTag=1

# Disables radio transmissions from players with an access level
DisableRadioStaff=false

# Disables radio transmissions from players with 'admin' access level
DisableRadioAdmin=true

# Disables radio transmissions from players with 'gm' access level
DisableRadioGM=true

# Disables radio transmissions from players with 'overseer' access level
DisableRadioOverseer=false

# Disables radio transmissions from players with 'moderator' access level
DisableRadioModerator=false

# Disables radio transmissions from invisible players
DisableRadioInvisible=true

# Semicolon-separated list of commands that will not be written to the cmd.txt server log. For example: \n-vehicle. Inputting * means do NOT write any vehicle command. Inputting: \n+vehicle.installPart means DO write that command
ClientCommandFilter=-vehicle.*;+vehicle.damageWindow;+vehicle.fixPart;+vehicle.installPart;+vehicle.uninstallPart

# Semicolon-separated list of actions that will be written to the ClientActionLogs.txt server log.
ClientActionLogs=ISEnterVehicle;ISExitVehicle;ISTakeEngineParts;

# Track changes in player perk levels in PerkLog.txt server log
PerkLogs=true

# Maximum number of items that can be placed in a container.  Zero means there is no limit. (PLEASE NOTE: This includes individual small items such as nails. A limit of 50 will mean only 50 nails can be stored.)\nMinimum=0 Maximum=9000 Default=0
ItemNumbersLimitPerContainer=0

# Number of days before old blood splats are removed.
# Removal happens when map chunks are loaded.
# Zero means they will never disappear\nMinimum=0 Maximum=365 Default=0
BloodSplatLifespanDays=0

# Allow use of non-ASCII (cyrillic etc) characters in usernames
AllowNonAsciiUsername=false

BanKickGlobalSound=true

# If enabled, when HoursForCorpseRemoval triggers, it will also remove player’s corpses from the ground.
RemovePlayerCorpsesOnCorpseRemoval=false

# If true, player can use the "delete all" button on bins.
TrashDeleteAll=false

# If true, player can hit again when struck by another player.
PVPMeleeWhileHitReaction=false

# If true, players will have to mouse over someone to see their display name.
MouseOverToSeeDisplayName=true

# If true, automatically hide the player you can't see (like zombies).
HidePlayersBehindYou=true

# Damage multiplier for PVP melee attacks.\nMinimum=0.00 Maximum=500.00 Default=30.00
PVPMeleeDamageModifier=30.0

# Damage multiplier for PVP ranged attacks.\nMinimum=0.00 Maximum=500.00 Default=50.00
PVPFirearmDamageModifier=50.0

# Modify the range of zombie attraction to cars. (Lower values can help with lag.)\nMinimum=0.00 Maximum=10.00 Default=0.50
CarEngineAttractionModifier=0.5

# Governs whether players bump (and knock over) other players when running through them.
PlayerBumpPlayer=false

# Controls display of remote players on the in-game map.\n1=Hidden 2=Friends 3=Everyone\nMinimum=1 Maximum=3 Default=1
MapRemotePlayerVisibility=1

# Minimum=1 Maximum=300 Default=5
BackupsCount=5

BackupsOnStart=true

BackupsOnVersionChange=true

# Minimum=0 Maximum=1500 Default=0
BackupsPeriod=0

# Disables anti-cheat protection for type 1.
AntiCheatProtectionType1=true

# Disables anti-cheat protection for type 2.
AntiCheatProtectionType2=true

# Disables anti-cheat protection for type 3.
AntiCheatProtectionType3=true

# Disables anti-cheat protection for type 4.
AntiCheatProtectionType4=true

# Disables anti-cheat protection for type 5.
AntiCheatProtectionType5=true

# Disables anti-cheat protection for type 6.
AntiCheatProtectionType6=true

# Disables anti-cheat protection for type 7.
AntiCheatProtectionType7=true

# Disables anti-cheat protection for type 8.
AntiCheatProtectionType8=true

# Disables anti-cheat protection for type 9.
AntiCheatProtectionType9=true

# Disables anti-cheat protection for type 10.
AntiCheatProtectionType10=true

# Disables anti-cheat protection for type 11.
AntiCheatProtectionType11=true

# Disables anti-cheat protection for type 12.
AntiCheatProtectionType12=true

# Disables anti-cheat protection for type 13.
AntiCheatProtectionType13=true

# Disables anti-cheat protection for type 14.
AntiCheatProtectionType14=true

# Disables anti-cheat protection for type 15.
AntiCheatProtectionType15=true

# Disables anti-cheat protection for type 16.
AntiCheatProtectionType16=true

# Disables anti-cheat protection for type 17.
AntiCheatProtectionType17=true

# Disables anti-cheat protection for type 18.
AntiCheatProtectionType18=true

# Disables anti-cheat protection for type 19.
AntiCheatProtectionType19=true

# Disables anti-cheat protection for type 20.
AntiCheatProtectionType20=true

AntiCheatProtectionType21=true

AntiCheatProtectionType22=true

AntiCheatProtectionType23=true

AntiCheatProtectionType24=true

# Threshold value multiplier for anti-cheat protection: type 2.\nMinimum=1.00 Maximum=10.00 Default=3.00
AntiCheatProtectionType2ThresholdMultiplier=3.0

# Threshold value multiplier for anti-cheat protection: type 3.\nMinimum=1.00 Maximum=10.00 Default=1.00
AntiCheatProtectionType3ThresholdMultiplier=1.0

# Threshold value multiplier for anti-cheat protection: type 4.\nMinimum=1.00 Maximum=10.00 Default=1.00
AntiCheatProtectionType4ThresholdMultiplier=1.0

# Threshold value multiplier for anti-cheat protection: type 9.\nMinimum=1.00 Maximum=10.00 Default=1.00
AntiCheatProtectionType9ThresholdMultiplier=1.0

# Threshold value multiplier for anti-cheat protection: type 15.\nMinimum=1.00 Maximum=10.00 Default=1.00
AntiCheatProtectionType15ThresholdMultiplier=1.0

# Threshold value multiplier for anti-cheat protection: type 20.\nMinimum=1.00 Maximum=10.00 Default=1.00
AntiCheatProtectionType20ThresholdMultiplier=1.0

# Minimum=1.00 Maximum=10.00 Default=1.00
AntiCheatProtectionType22ThresholdMultiplier=1.0

# Minimum=1.00 Maximum=10.00 Default=6.00
AntiCheatProtectionType24ThresholdMultiplier=6.0
```
</details>

</br>

<details>
  
  <summary>pzserver_SandboxVars.lua - This is the main config file for sandbox options.</summary>
  
```ruby
SandboxVars = {
    VERSION = 5,
    -- Changing this sets the "Population Multiplier" advanced option. Default=Normal
    -- 1 = Insane
    -- 2 = Very High
    -- 3 = High
    -- 4 = Normal
    -- 5 = Low
    Zombies = 3,
    -- Default=Urban Focused
    -- 1 = Urban Focused
    Distribution = 1,
    -- Default=1 Hour
    -- 1 = 15 Minutes
    -- 2 = 30 Minutes
    -- 3 = 1 Hour
    -- 4 = 2 Hours
    -- 5 = 3 Hours
    -- 6 = 4 Hours
    -- 7 = 5 Hours
    -- 8 = 6 Hours
    -- 9 = 7 Hours
    -- 10 = 8 Hours
    -- 11 = 9 Hours
    -- 12 = 10 Hours
    -- 13 = 11 Hours
    -- 14 = 12 Hours
    -- 15 = 13 Hours
    -- 16 = 14 Hours
    -- 17 = 15 Hours
    -- 18 = 16 Hours
    -- 19 = 17 Hours
    -- 20 = 18 Hours
    -- 21 = 19 Hours
    -- 22 = 20 Hours
    -- 23 = 21 Hours
    -- 24 = 22 Hours
    -- 25 = 23 Hours
    DayLength = 3,
    StartYear = 1,
    -- Default=July
    -- 1 = January
    -- 2 = February
    -- 3 = March
    -- 4 = April
    -- 5 = May
    -- 6 = June
    -- 7 = July
    -- 8 = August
    -- 9 = September
    -- 10 = October
    -- 11 = November
    StartMonth = 7,
    StartDay = 9,
    -- Default=9 AM
    -- 1 = 7 AM
    -- 2 = 9 AM
    -- 3 = 12 PM
    -- 4 = 2 PM
    -- 5 = 5 PM
    -- 6 = 9 PM
    -- 7 = 12 AM
    -- 8 = 2 AM
    StartTime = 2,
    -- Default=0-30 Days
    -- 1 = Instant
    -- 2 = 0-30 Days
    -- 3 = 0-2 Months
    -- 4 = 0-6 Months
    -- 5 = 0-1 Year
    -- 6 = 0-5 Years
    -- 7 = 2-6 Months
    WaterShut = 2,
    -- Default=0-30 Days
    -- 1 = Instant
    -- 2 = 0-30 Days
    -- 3 = 0-2 Months
    -- 4 = 0-6 Months
    -- 5 = 0-1 Year
    -- 6 = 0-5 Years
    -- 7 = 2-6 Months
    ElecShut = 2,
    -- Minimum=-1 Maximum=2147483647 Default=14
    WaterShutModifier = 14,
    -- Minimum=-1 Maximum=2147483647 Default=14
    ElecShutModifier = 14,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    FoodLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    CannedFoodLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    LiteratureLoot = 4,
    -- Seeds, Nails, Saws, Fishing Rods, various tools, etc... Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    SurvivalGearsLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    MedicalLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    WeaponLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    RangedWeaponLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    AmmoLoot = 4,
    -- Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    MechanicsLoot = 4,
    -- Everything else. Also affects foraging for all items in Town/Road zones. Default=Rare
    -- 1 = None (not recommended)
    -- 2 = Insanely Rare
    -- 3 = Extremely Rare
    -- 4 = Rare
    -- 5 = Normal
    -- 6 = Common
    OtherLoot = 4,
    -- Controls the global temperature. Default=Normal
    -- 1 = Very Cold
    -- 2 = Cold
    -- 3 = Normal
    -- 4 = Hot
    Temperature = 3,
    -- Controls how often it rains. Default=Normal
    -- 1 = Very Dry
    -- 2 = Dry
    -- 3 = Normal
    -- 4 = Rainy
    Rain = 3,
    -- Number of days until 100% growth. Default=Normal (100 Days)
    -- 1 = Very Fast (20 Days)
    -- 2 = Fast (50 Days)
    -- 3 = Normal (100 Days)
    -- 4 = Slow (200 Days)
    ErosionSpeed = 3,
    -- Number of days until 100% growth. -1 means no growth. Zero means use the Erosion Speed option. Maximum 36,500 (100 years). Minimum=-1 Maximum=36500 Default=0
    ErosionDays = 0,
    -- Modifies the base XP gain from actions by this number. Minimum=0.00 Maximum=1000.00 Default=1.00
    XpMultiplier = 1.0,
    -- Determines if the XP multiplier affects passively levelled skills eg. Fitness and Strength.
    XpMultiplierAffectsPassive = false,
    -- Use this to multiply or reduce engine general loudness. Minimum=0.00 Maximum=100.00 Default=1.00
    ZombieAttractionMultiplier = 1.0,
    -- Governs whether cars are locked, need keys to start etc.
    VehicleEasyUse = false,
    -- Controls the speed of plant growth. Default=Normal
    -- 1 = Very Fast
    -- 2 = Fast
    -- 3 = Normal
    -- 4 = Slow
    Farming = 3,
    -- Controls the time it takes for food to break down in a composter. Default=2 Weeks
    -- 1 = 1 Week
    -- 2 = 2 Weeks
    -- 3 = 3 Weeks
    -- 4 = 4 Weeks
    -- 5 = 6 Weeks
    -- 6 = 8 Weeks
    -- 7 = 10 Weeks
    CompostTime = 2,
    -- How fast character's hunger, thirst and fatigue will decrease. Default=Normal
    -- 1 = Very Fast
    -- 2 = Fast
    -- 3 = Normal
    -- 4 = Slow
    StatsDecrease = 3,
    -- Controls the abundance of fish and general forage. Default=Normal
    -- 1 = Very Poor
    -- 2 = Poor
    -- 3 = Normal
    -- 4 = Abundant
    NatureAbundance = 3,
    -- Default=Sometimes
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    Alarm = 4,
    -- How frequently homes and buildings will be discovered locked Default=Very Often
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    LockedHouses = 6,
    -- Spawn with chips, water bottle, school bag, baseball bat and a hammer.
    StarterKit = false,
    -- Nutritional value of food affects the player's condition.
    Nutrition = true,
    -- Define how fast the food will spoil inside or outside fridge. Default=Normal
    -- 1 = Very Fast
    -- 2 = Fast
    -- 3 = Normal
    -- 4 = Slow
    FoodRotSpeed = 3,
    -- Define how much a fridge will be effective. Default=Normal
    -- 1 = Very Low
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    FridgeFactor = 3,
    -- Items will respawn in already-looted containers in towns and trailer parks. Items will not respawn in player-made containers. Default=None
    -- 1 = None
    -- 2 = Every Day
    -- 3 = Every Week
    -- 4 = Every Month
    LootRespawn = 1,
    -- When > 0, loot will not respawn in zones that have been visited within this number of in-game hours. Minimum=0 Maximum=2147483647 Default=0
    SeenHoursPreventLootRespawn = 0,
    -- A comma-separated list of item types that will be removed after HoursForWorldItemRemoval hours.
    WorldItemRemovalList = "Base.Hat,Base.Glasses,Base.Maggots",
    -- Number of hours since an item was dropped on the ground before it is removed.  Items are removed the next time that part of the map is loaded.  Zero means items are not removed. Minimum=0.00 Maximum=2147483647.00 Default=24.00
    HoursForWorldItemRemoval = 24.0,
    -- If true, any items *not* in WorldItemRemovalList will be removed.
    ItemRemovalListBlacklistToggle = false,
    -- This will affect starting world erosion and food spoilage. Default=0
    -- 1 = 0
    -- 2 = 1
    -- 3 = 2
    -- 4 = 3
    -- 5 = 4
    -- 6 = 5
    -- 7 = 6
    -- 8 = 7
    -- 9 = 8
    -- 10 = 9
    -- 11 = 10
    -- 12 = 11
    TimeSinceApo = 1,
    -- Will influence how much water the plant will lose per day and their ability to avoid disease. Default=Normal
    -- 1 = Very High
    -- 2 = High
    -- 3 = Normal
    -- 4 = Low
    PlantResilience = 3,
    -- Controls the yield of plants when harvested. Default=Normal
    -- 1 = Very Poor
    -- 2 = Poor
    -- 3 = Normal
    -- 4 = Abundant
    PlantAbundance = 3,
    -- Recovery from being tired from performing actions Default=Normal
    -- 1 = Very Fast
    -- 2 = Fast
    -- 3 = Normal
    -- 4 = Slow
    EndRegen = 3,
    -- How regularly helicopters pass over the event zone. Default=Once
    -- 1 = Never
    -- 2 = Once
    -- 3 = Sometimes
    Helicopter = 2,
    -- How often zombie attracting metagame events like distant gunshots will occur. Default=Sometimes
    -- 1 = Never
    -- 2 = Sometimes
    MetaEvent = 2,
    -- Governs night-time metagame events during the player's sleep. Default=Never
    -- 1 = Never
    -- 2 = Sometimes
    SleepingEvent = 1,
    -- Increase/decrease the chance of electrical generators spawning on the map. Default=Sometimes
    -- 1 = Extremely Rare
    -- 2 = Rare
    -- 3 = Sometimes
    -- 4 = Often
    GeneratorSpawning = 3,
    -- How much fuel is consumed per in-game hour. Minimum=0.00 Maximum=100.00 Default=1.00
    GeneratorFuelConsumption = 1.0,
    -- Increase/decrease probability of discovering randomized safe houses on the map: either burnt out, containing loot stashes, dead survivor bodies etc. Default=Rare
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    SurvivorHouseChance = 3,
    -- Default=Rare
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    VehicleStoryChance = 3,
    -- Default=Rare
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    ZoneStoryChance = 3,
    -- Impacts on how often a looted map will have annotations marked on it by a deceased survivor. Default=Sometimes
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    AnnotatedMapChance = 4,
    -- Adds free points during character creation. Minimum=-100 Maximum=100 Default=0
    CharacterFreePoints = 0,
    -- Gives player-built constructions extra hit points so they are more resistant to zombie damage. Default=Normal
    -- 1 = Very Low
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    ConstructionBonusPoints = 3,
    -- Governs the ambient lighting at night. Default=Normal
    -- 1 = Pitch Black
    -- 2 = Dark
    -- 3 = Normal
    NightDarkness = 3,
    -- Governs the time from dusk to dawn. Default=Normal
    -- 1 = Always Night
    -- 2 = Long
    -- 3 = Normal
    -- 4 = Short
    NightLength = 3,
    -- Increase and decrease the impact injuries have on your body, and their healing time. Default=Normal
    -- 1 = Low
    -- 2 = Normal
    InjurySeverity = 2,
    -- Enable or disable broken limbs when survivors receive injuries from impacts, zombie damage and falls.
    BoneFracture = true,
    -- How long before zombie bodies disappear. Minimum=-1.00 Maximum=2147483647.00 Default=216.00
    HoursForCorpseRemoval = 216.0,
    -- Governs impact that nearby decaying bodies has on the player's health and emotions. Default=Normal
    -- 1 = None
    -- 2 = Low
    -- 3 = Normal
    DecayingCorpseHealthImpact = 3,
    -- How much blood is sprayed on floor and walls. Default=Normal
    -- 1 = None
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    BloodLevel = 3,
    -- Governs how quickly clothing degrades, becomes dirty, and bloodied. Default=Normal
    -- 1 = Disabled
    -- 2 = Slow
    -- 3 = Normal
    ClothingDegradation = 3,
    FireSpread = true,
    -- Number of in-game days before rotten food is removed from the map. -1 means rotten food is never removed. Minimum=-1 Maximum=2147483647 Default=-1
    DaysForRottenFoodRemoval = -1,
    -- If enabled, generators will work on exterior tiles, allowing for example to power gas pump.
    AllowExteriorGenerator = true,
    -- Controls the maximum intensity of fog. Default=Normal
    -- 1 = Normal
    -- 2 = Moderate
    MaxFogIntensity = 1,
    -- Controls the maximum intensity of rain. Default=Normal
    -- 1 = Normal
    -- 2 = Moderate
    MaxRainFxIntensity = 1,
    -- If disabled snow will not accumulate on ground but will still be visible on vegetation and rooftops.
    EnableSnowOnGround = true,
    -- When enabled certain melee weapons will be able to strike multiple zombies in one hit.
    MultiHitZombies = false,
    -- Chance of being bitten when a zombie attacks from behind. Default=High
    -- 1 = Low
    -- 2 = Medium
    RearVulnerability = 3,
    -- Disable to walk unimpeded while melee attacking.
    AttackBlockMovements = true,
    AllClothesUnlocked = false,
    -- if disabled, tainted water will not have a warning marking it as such
    EnableTaintedWaterText = true,
    -- Governs how frequently cars are discovered on the map Default=Low
    -- 1 = None
    -- 2 = Very Low
    -- 3 = Low
    -- 4 = Normal
    CarSpawnRate = 3,
    -- Governs the chances of finding vehicles with gas in the tank. Default=Low
    -- 1 = Low
    -- 2 = Normal
    ChanceHasGas = 1,
    -- Governs how full gas tanks will be in discovered cars. Default=Low
    -- 1 = Very Low
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    -- 5 = Very High
    InitialGas = 2,
    -- Governs how full gas tanks in fuel station will be, initially. Default=Normal
    -- 1 = Empty
    -- 2 = Super Low
    -- 3 = Very Low
    -- 4 = Low
    -- 5 = Normal
    -- 6 = High
    -- 7 = Very High
    -- 8 = Full
    FuelStationGas = 5,
    -- How gas-hungry vehicles on the map are. Minimum=0.00 Maximum=100.00 Default=1.00
    CarGasConsumption = 1.0,
    -- Default=Rare
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    LockedCar = 3,
    -- General condition of vehicles discovered on the map Default=Low
    -- 1 = Very Low
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    CarGeneralCondition = 2,
    -- Governs the amount of damage dealt to vehicles that crash. Default=Normal
    -- 1 = Very Low
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    CarDamageOnImpact = 3,
    -- Damage received by the player from the car in a collision. Default=None
    -- 1 = None
    -- 2 = Low
    -- 3 = Normal
    -- 4 = High
    DamageToPlayerFromHitByACar = 1,
    -- Enable or disable traffic jams that spawn on the main roads of the map.
    TrafficJam = true,
    -- How frequently cars will be discovered with an alarm. Default=Extremely Rare
    -- 1 = Never
    -- 2 = Extremely Rare
    -- 3 = Rare
    -- 4 = Sometimes
    -- 5 = Often
    CarAlarm = 2,
    -- Enable or disable player getting damage from being in a car accident.
    PlayerDamageFromCrash = true,
    -- How many in-game hours before a wailing siren shuts off. Minimum=0.00 Maximum=168.00 Default=0.00
    SirenShutoffHours = 0.0,
    --  Governs whether player can discover a car that has been maintained and cared for after the infection struck. Default=Low
    -- 1 = None
    -- 2 = Low
    -- 3 = Normal
    RecentlySurvivorVehicles = 2,
    -- Enables vehicles to spawn.
    EnableVehicles = true,
    -- Governs if poisoning food is enabled. Default=True
    -- 1 = True
    -- 2 = False
    EnablePoisoning = 1,
    -- Default=In and around bodies
    -- 1 = In and around bodies
    -- 2 = In bodies only
    MaggotSpawn = 1,
    -- The higher the value, the longer lightbulbs last before breaking. If 0, lightbulbs will never break. Does not affect vehicle headlights. Minimum=0.00 Maximum=1000.00 Default=1.00
    LightBulbLifespan = 1.0,
    Map = {
        AllowMiniMap = false,
        AllowWorldMap = true,
        MapAllKnown = false,
    },
    ZombieLore = {
        -- Controls the zombie movement rate. Default=Fast Shamblers
        -- 1 = Sprinters
        -- 2 = Fast Shamblers
        -- 3 = Shamblers
        Speed = 2,
        -- Controls the damage zombies inflict per attack. Default=Normal
        -- 1 = Superhuman
        -- 2 = Normal
        -- 3 = Weak
        Strength = 2,
        -- Controls the difficulty to kill zombies. Default=Normal
        -- 1 = Tough
        -- 2 = Normal
        -- 3 = Fragile
        Toughness = 2,
        -- Controls how the zombie virus spreads. Default=Blood + Saliva
        -- 1 = Blood + Saliva
        -- 2 = Saliva Only
        -- 3 = Everyone's Infected
        Transmission = 1,
        -- Controls how quickly the infection takes effect. Default=2-3 Days
        -- 1 = Instant
        -- 2 = 0-30 Seconds
        -- 3 = 0-1 Minutes
        -- 4 = 0-12 Hours
        -- 5 = 2-3 Days
        -- 6 = 1-2 Weeks
        Mortality = 5,
        -- Controls how quickly corpses rise as zombies. Default=0-1 Minutes
        -- 1 = Instant
        -- 2 = 0-30 Seconds
        -- 3 = 0-1 Minutes
        -- 4 = 0-12 Hours
        -- 5 = 2-3 Days
        Reanimate = 3,
        -- Controls zombie intelligence. Default=Basic Navigation
        -- 1 = Navigate + Use Doors
        -- 2 = Navigate
        -- 3 = Basic Navigation
        Cognition = 3,
        -- Controls which zombies can crawl under vehicles. Default=Often
        -- 1 = Crawlers Only
        -- 2 = Extremely Rare
        -- 3 = Rare
        -- 4 = Sometimes
        -- 5 = Often
        -- 6 = Very Often
        CrawlUnderVehicle = 5,
        -- Controls how long zombies remember players after seeing or hearing. Default=Normal
        -- 1 = Long
        -- 2 = Normal
        -- 3 = Short
        -- 4 = None
        Memory = 2,
        -- Controls zombie vision radius. Default=Normal
        -- 1 = Eagle
        -- 2 = Normal
        -- 3 = Poor
        Sight = 2,
        -- Controls zombie hearing radius. Default=Normal
        -- 1 = Pinpoint
        -- 2 = Normal
        -- 3 = Poor
        Hearing = 2,
        -- Zombies that have not seen/heard player can attack doors and constructions while roaming.
        ThumpNoChasing = false,
        -- Governs whether or not zombies can destroy player constructions and defences.
        ThumpOnConstruction = true,
        -- Governs whether zombies are more active during the day, or whether they act more nocturnally.  Active zombies will use the speed set in the "Speed" setting. Inactive zombies will be slower, and tend not to give chase. Default=Both
        -- 1 = Both
        -- 2 = Night
        ActiveOnly = 1,
        -- Allows zombies to trigger house alarms when breaking through windows and doors.
        TriggerHouseAlarm = false,
        -- When enabled if multiple zombies are attacking they can drag you down to feed. Dependent on zombie strength.
        ZombiesDragDown = true,
        -- When enabled zombies will have a chance to lunge after climbing over a fence if you're too close.
        ZombiesFenceLunge = true,
        -- Default=Some zombies in the world will pretend to be dead
        -- 1 = Some zombies in the world will pretend to be dead
        -- 2 = Some zombies in the world, as well as some you 'kill', can pretend to be dead
        DisableFakeDead = 1,
    },
    ZombieConfig = {
        -- Set by the "Zombie Count" population option. 4.0 = Insane, Very High = 3.0, 2.0 = High, 1.0 = Normal, 0.35 = Low, 0.0 = None. Minimum=0.00 Maximum=4.00 Default=1.00
        PopulationMultiplier = 1.0,
        -- Adjusts the desired population at the start of the game. Minimum=0.00 Maximum=4.00 Default=1.00
        PopulationStartMultiplier = 1.0,
        -- Adjusts the desired population on the peak day. Minimum=0.00 Maximum=4.00 Default=1.50
        PopulationPeakMultiplier = 1.5,
        -- The day when the population reaches it's peak. Minimum=1 Maximum=365 Default=28
        PopulationPeakDay = 28,
        -- The number of hours that must pass before zombies may respawn in a cell. If zero, spawning is disabled. Minimum=0.00 Maximum=8760.00 Default=72.00
        RespawnHours = 72.0,
        -- The number of hours that a chunk must be unseen before zombies may respawn in it. Minimum=0.00 Maximum=8760.00 Default=16.00
        RespawnUnseenHours = 16.0,
        -- The fraction of a cell's desired population that may respawn every RespawnHours. Minimum=0.00 Maximum=1.00 Default=0.10
        RespawnMultiplier = 0.1,
        -- The number of hours that must pass before zombies migrate to empty parts of the same cell. If zero, migration is disabled. Minimum=0.00 Maximum=8760.00 Default=12.00
        RedistributeHours = 12.0,
        -- The distance a zombie will try to walk towards the last sound it heard. Minimum=10 Maximum=1000 Default=100
        FollowSoundDistance = 100,
        -- The size of groups real zombies form when idle. Zero means zombies don't form groups. Groups don't form inside buildings or forest zones. Minimum=0 Maximum=1000 Default=20
        RallyGroupSize = 20,
        -- The distance real zombies travel to form groups when idle. Minimum=5 Maximum=50 Default=20
        RallyTravelDistance = 20,
        -- The distance between zombie groups. Minimum=5 Maximum=25 Default=15
        RallyGroupSeparation = 15,
        -- How close members of a group stay to the group's leader. Minimum=1 Maximum=10 Default=3
        RallyGroupRadius = 3,
    },
}

```

</details>

</br>
</br>

<h1 align="center"><strong>« ACTIVE MODLIST »</strong></h1>

|        LO / Mod Name        | Category |         Description         |                            Workshop ID                            | Custom Settings | Tested | Needs Wipe |                 Notes                |
|:---------------------------:|:--------:|:---------------------------:|:-----------------------------------------------------------------:|:---------------:|:------:|:----------:|:------------------------------------:|
|  1<br/>77 Pontiac Firebird  |   Cars   |           Adds car          | https://steamcommunity.com/sharedfiles/filedetails/?id=3346905070 |       Yes       |   Yes  | No         | Need to wipe server before uninstall |
| 2<br/>Filibusters Used Cars |   Cars   | Adds 50 lore friendly cars. | https://steamcommunity.com/sharedfiles/filedetails/?id=3346905070 |        No       |   Yes  | Yes        | Remove on next wipe                  |
|         3<br/>Mod 3         |    UI    |         It does this        | https://steamcommunity.com/sharedfiles/filedetails/?id=3346905070 |        No       |   No   | Yes        | Has glitches                         |
|         4<br/>Mod 4         | Gameplay |         It does that        | https://steamcommunity.com/sharedfiles/filedetails/?id=3346905070 |       Yes       |   No   | No         | Not compatible with other cars mods  |
|         5<br/>Mod 5         |   Maps   |         It does this        | https://steamcommunity.com/sharedfiles/filedetails/?id=3346905070 |        No       |   Yes  | Yes        | Runs ok                              |
