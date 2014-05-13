IT-266-102-Quake4-Source
========================
README:

Super-Fast Jelly Fish: Extreme Speed Mod 

By Ryan Campanella

In order to play Super-Fast Jelly Fish to the fullest, you will need at least two players in the game. You will need to pull the actual mod folder off of github, which can be obtained via the link: https://github.com/Rc287/IT-266-102-Quake4-Mods/tree/master
To start playing the mod, put the folder in the Quake 4 directory and then run the game. Once you are in the game, select mods and click on superfastjellyfish. Then, the mod should be ready to be played in multiplayer.

Below, I have included all changes that I have made in the game. The first list refers to a summary of what was changed. For more specifics, please refer to the second list which is a progress report of all mechanics in the mod.

Enjoy!

-Ryan Campanella
=======================
•	The fire-rate of all weapons in the multiplayer game will be increased to an appropriate amount.

•	The reload speed of all weapons (time it takes to ready the next round) will be decreased to an appropriate amount proportional to the fire-rate.

•	The maximum ammunition of all weapons will be greatly increased, as well as the amount of ammunition received from item pickups (Same as other mod).

•	The movement speed of each player will be initialized to an appropriate speed. This will allow for players to be able to dodge incoming projectiles.

•	Specific item pickups will alter movement speeds of players in different way. See powerup/item designs below.

•	Specific weapons will influence the speed of the players in the game. See weapon designs below.

•	Upon killing an enemy player, the score that the killer receives will differ, depending on what the victim’s current speed was. This will work based on the nearest hundred percent. For example, if the victim’s speed was 200% of the original speed, then the score received will be doubled. Score = Victim Speed // Initial Speed. (Victim Speed integer divison Initial Speed)

•	The speed limits will be 100% speed as the lower limit (initial speed) and 500% speed as the upper limit (max speed).

•	Upon death, the player’s speed will be reset to the initial speed. The killer’s speed is increased by 25% of the victims speed before death.

========================
Super-Fast Jelly Fish Progress Report

4/16/14:

Shotgun Fire Rate set to 0.2 from 1.0. (Works)
Shotgun Pellet Damage set to 3 from 14. (Works)
Shotgun Starting Ammo set to 50 from 10. (Works) 

Rocket Launcher Fire Rate set to 0.01 from 0.8. (Works)
Rocket Launcher Reload Rate set to 0.1 from 0.8. (Works)
Rocket Launcher Damage set to 0 from 100. (Works)
Rocket Launcher Splash Damage set to 0 from 100. (Works)
Rocket Launcher Starting Ammo set to 40 from 10. (Works)

Railgun Fire Rate set to 0.25 from 1.5. (Works)
Railgun Damage set to 20 from 100. (Works)
Railgun Starting Ammo set to 35 from 10. (Works)

Nailgun Fire Rate set to 0.01 from 0.16. (Works)
Nailgun Damage set to 0 from 30. (Works)
Nailgun Splash Damage set to 0 from 30. (Works)
Nailgun Starting Ammo set to 300 from 50. (Works)

Machinegun Fire Rate set to 0.01 from 0.1. (Works)
Machinegun Damage set to 3 from 7. (Works)
Machinegun Starting Ammo currently unchanged from 40. 

Lightning Gun Fire Rate set to 0.01 from 0.05. (Works)
Lightning Gun Damage set to 1 from 8. (Works)
Lightning Gun Starting Ammo set to 300 from 100. (Works)

Hyperblaster Fire Rate set to 0.02 from 0.08. (Works)
Hyperblaster Damage set to 4 from 14. (Works)
Hyperblaster Starting Ammo set to 400 from 60. (Works)

Grenade Launcher Fire Rate set to 0.2 from 0.8. (Works)
Grenade Launcher Damage set to 25 from 100. (Works)
Grenade Launcher Splash Damage set to 25 from 100. (Works)
Grenade Launcher Starting Ammo set to 50 from 10. (Works)

No edits made to Gauntlet.

No edits made to Blaster.
 
Future Notes: Haste Appears in MultiplayerGame.cpp in CheckSpecialLights

5/8/14:

Score Implementation Completed (Works)

Hyperblaster Damage changed to 1 from 10. (Works)
Hyperblaster Splash Damage set to 1 from 10. (Works)

Initial Player Movement Speed created and set to 200. (Works)
Initial Player Movement Speed Increase created and set to 0. (Works)
Total Player Speed must be between the initial movement speed and 5*initial movement speed. (Works)

5/11/14:

Weapon Upgrades:

1. Shotgun will cost 5 units of speed per shot, regardless of a hit or miss, and deals bonus damage equal to 25% of attacker bonus speed. (Works)

2. Rocket Launcher deals no damage to players, but can be used as a utility to rocket jump around the map. (Works)

3. Railgun gives speed de-buff to the victim that can only be removed upon that player shooting another player with the railgun (Similar to tag). De-buff halves bonus speed of victim. (Works)

4. Nailgun works similarly to The Needler from Halo. Upon being hit with a nail, a de-buff will be applied to the victim that will stack up to thirty times. If the stack hits thirty, the victim will be killed. De-buff can only be removed one stack at a time by transferring them to another player. (Works)

5. Machinegun increases speed by 10 for each bullet that hits the victim. (Works)

6. Lightning Gun steals 5 units of speed from victim per hit. (Works)

7. Hyperblaster speeds up victim by 10 and decreases speed of the attacker by 10. This can be used to make the victim more valuable before killing them, while decreasing the value of the attacker. (Works)

8. Grenade Launcher bursts 50 units of speed from victim per hit. (Works)

Item/Powerup Upgrades:

Picking up any item or weapon will increase speed by 10 units. (Works)

Haste Power Up no longer increases speed and fire rate. Now, the player who grabs this Power Up will automatically be given maximum speed for thirty seconds. After the power up wears off, the player will keep the maximum speed. (Works)

Quad Damage Power Up no longer increases damage output. Upon pickup, all but the player who picked up the item will be reset to the initial speed. The other players will be unable to gain speed for thirty seconds. (Works)
