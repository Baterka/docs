# AOneBlock

**AOneBlock** is our take on **IJAminecraft**'s popular survival map: OneBlock.
Players have to survive on a single block, which appears to be magic...

Created and maintained by [tastybento](https://github.com/tastybento).

{{ addon_description("AOneBlock") }}

## About
OneBlock puts you on a block in space. There is only one block. What do you do next?

## Development Status

The game is in Beta stage.

## Commands

The user command is `/ob`. The admin command is `/oba`.

## FAQ

Q: What phases are there?

A: There are 11 phases: Plains, Underground, Winter, Ocean, Jungle, Swamp, Dungeon, Desert, The Nether, Plenty, Desolation, and The End. Each phase features a set of blocks, items, and mobs appropriate for the setting.

Q: How many blocks are there in the 11 phases?

A: There are currently 11 thousand blocks!

Q: What happens after the last phase?

A: The phases repeat.

Q: Why do I keep falling and dying!

A: There are tricks to surviving, but it might be difficult! You need to build defenses.

Q: Why do certain blocks spawn more frequently than others?

A: They just do! You can set the relative probability in the config files in the phases folder.

Q. How do I know which is the magic block?

A. Hit it and it will give out green particles.

Q. My magic block is no longer there! How do I get another one?

A. You will have to place a block there. Worse case, kill yourself and one will be generated.

Q. My magic block is liquid! How can I mine it?

A. Use a bucket.

Q: Which mobs can spawn?

A: Each phase has a different set of mobs that can spawn. Be careful because they may push you off! If you listen carefully, you may hear hostile mobs coming.

Q. I have no chance to react to hostile mobs spawning!

A. Be prepared. Listen carefully when you mine a block and you will hear hostile mobs coming before they spawn. If you are in a hostile phase, then expect mobs and build defenses to protect yourself. You can mine a block from quite far away.

Q. When mobs spawn, my defenses are destroyed! Why?

A. Mobs make space to spawn. If there's anything in the way, it'll be broken and dropped. You'll have to build accordingly.

Q: Do chests spawn?

A: Yes. Chests spawn with random items in them from the current phase. There are common, uncommon, rare and epic chests. Chests with sparkles are good.

Q: Is it possible to reach the Nether or End in this map?

A: The vanilla Nether exists by default but there is no End world. 

Q: What is the end goal?

A: It's whatever you want it to be! 

Q: How to use holograms?

A: AOneBlock uses [Holographic Displays](https://dev.bukkit.org/projects/holographic-displays) for holograms. You need to install this plugin to use holograms sections! 

Q. Should I use the Levels addon?

A. It's up to you, but if you do be aware that levels could get high because players have an infinite block. I prefer not to use it and instead use the Likes addon.

## Installation

0. Install BentoBox and run it on the server at least once to create its data folders.
1. Place this jar in the addons folder of the BentoBox plugin.
2. Restart the server.
3. The addon will create worlds and a data folder and inside the folder will be a config.yml and config files in phases folder.
4. Stop the server.
5. Edit config.yml and the .yml config files how you want.
6. Delete any worlds that were created by default if you made changes that would affect them.
7. Restart the server.

## Phase config files

The config files to make the phases are in the phases folder.

There are two files per phase - a file that contains the blocks and mobs, and a file that contains the chests.

The first number of any file is how many blocks need to be mined to reach that phase. This is the phase's key number.
Each phase also has a name, a biome and the following sections:

- blocks
- mobs

In the chests file, it just has the phase number and a chests section.


### blocks

The blocks section list Bukkit Materials followed by a relative probability. All the probability values are added up for the whole phase and the chance of the block being placed is the relative probability divided by the total of all the probabilities.

### mobs

The mob section list mobs that can spawn and their relative probability along with blocks. You can only list entities that are alive and can spawn in this list.

### chests

If CHEST is listed in the blocks section, then it will be randomly filled according to this section. You can define as many chests as you like. The first number is a unique chest number. Then follows the chest contents that includes the slot number and the item stack contents. Finally there is the chest's rarity, which can be COMMON, UNCOMMON, RARE or EPIC. The best way to set chests is to do it in game. Fill a chest with the contents you want and then while looking at it enter the command `/oba setchest <phase> <rarity>` where <phase> is the name of the phase and rarity is the rarity. Use Tab Complete to see the options. The chest will be automatically added to the oneblocks.yml file and be ready to use. Deleting chests must be done by editing the oneblocks.yml file for now and reloading the addon.

Be very careful when editing the chest items and check that the material is a true Bukkit material and spelled correctly.

### Other Add-ons

OneBlock is an add-on that uses the BentoBox API. Here are some other ones that you may be interested in:

* [**Addons**](https://github.com/BentoBoxWorld/BentoBox/blob/develop/ADDON.md)

You can add all the usual addons to OneBlock, like Challeges, Likes, Level, Warps, etc. but it is not required.

## Permissions

Permissions can be found [here](Permissions).

## Commands

Commands can be found [here](Commands).

## Placeholders

Placeholders can be found [here](Placeholders).

## Translations

{{ translations(4481, ["cs", "de", "es", "fr", "hr", "hu", "id", "it", "ja", "tr", "vi", "zh-CN", "zh-TW"]) }}
