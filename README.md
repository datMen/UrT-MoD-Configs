UrT Mod Configurations for Z3NMOD by Z3nnY
========================
<!--
### Info -

##### Weapons:

| Key  | Weapon |
| ------------- | ------------- |
| 1  | Knife  |
| 4  | Franchi SPAS12  |
| 5  | HK MP5K  |
| 6  | HK UMP45  |
| 7  | HK69 40mm  |
| 8  | ZM LR300  |
| 9  | HK G36  |
| 10  | HK PSG1  |
| 11  | HE Grenade  |
| 12  | Flash Grenade  |
| 13  | Smoke Grenade  |
| 14  | Remington SR8  |
| 15  | AK103 7.62mm  |
| 17  | IMI Negev  |
| 19  | Colt M4A1  |

##### Items:

| Key  | Item |
| ------------- | ------------- |
| 17  | Kevlar Vest  |
| 18  | TacGoogles  |
| 19  | Medkit |
| 20  | Silencer  |
| 21  | Laser Sight  |
| 22  | Helmet  |

-

-->
### Fix List: ###

##### Cvars: #####
* <strong>[COMPLETED]</strong> z3n_coloredname: Show colors also on the scoreboard and killed-by messages.

##### Rcon Commands: #####
* gw & gi: Allow give many weapons/items at the same time (with commas or whatever).

##### Other: #####
* Fix curb stomp when NoFallDamage activated
* Fix $location, $weapon... in chat
* Fix ammo drops in maps (currently not working at deathrun, thats why we had to put ammo regen)

-

### Whish List: ###
* Add server-side Guns system: https://github.com/TheLouK/Urt-Source-Code/blob/master/guns42.c
```
        Check the SV_Check_Com_Printf & the added cvar "sv_Guns". This code was made for 4.2 but also, please take a look to the SV_Event_Kill_Guns cause i'm not 100% sure it will work fine with your mod :)
```
* Team config (Free/Blue/Red):
    * <strong>[COMPLETED]</strong> RegenStamina: like the RegenHealth but for stamina :D (it could behave like the 4.1 mod if possible: it starts to regen when the player is not in the air)
    * <strong>[COMPLETED]</strong> ForceWeapons & ForceItems: The player will spawn with these weapons.
* Hide "!pm " in chat: https://github.com/TheLouK/Urt-Source-Code/commit/88074d19603331be46943cc0542e024ea8483af8

##### Cvars: #####

##### Rcon Commands: #####
* <strong>[COMPLETED]</strong> spoof: Send a server command as a specific client.1/commits/3df483ae0ad8fea766afd3c357999bf9c2ff987d
* <strong>[COMPLETED]</strong> teleport or tp: no explanation needed x)
* <strong>[COMPLETED]</strong> setweapon or sw: remove all weapons except the given (would be wreat if we can set more than one).
* <strong>[COMPLETED]</strong> setitem or si: remove all items except the given (would be wreat if we can set more than one).

-