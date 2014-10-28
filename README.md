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
### Fix List:

##### Cvars:
* z3n_coloredname: Show colors also on the scoreboard and killed-by messages.

##### Rcon Commands:
* gw & gi: Allow give many weapons/items at the same time (with commas or whatever).

##### Other:
* Fix curb stomp when NoFallDamage activated
* Fix $location, $weapon... in chat
* Fix ammo drops in maps (currently not working at deathrun, thats why we had to put ammo regen)

-

### Whish List:
* Add server-side Guns system: https://github.com/TheLouK/Urt-Source-Code/blob/master/guns42.c

        Check the SV_Check_Com_Printf & the added cvar "sv_Guns". This code was made for 4.2 but also, please take a look to the SV_Event_Kill_Guns cause i'm not 100% sure it will work fine with your mod :)

* Team config (Free/Blue/Red):
    * RegenStamina: like the RegenHealth but for stamina :D (it could behave like the 4.1 mod if possible: it starts to regen when the player is not in the air)
    * ForceWeapons & ForceItems: The player will spawn with these weapons. If you can, it would be great if we can add "ForceSettings":
    * ForceSettings:
        * <strong>+</strong> symbol: Allow the player to set his weapons/items, the weapon/item set after the "+" will be ADDED to his "inventory" (just if the player doesn't have it).
        * <strong>-</strong> symbol: Allow the player to set his weapons/items, the weapon/item set after the "-" will be REMOVED from his "inventory" (if the player have it).
        * <strong>@</strong> symbol: A reference to all weapons (your current "-").

                Force Example:

                    ForceWeapons: +14, -6 // Give Sr8 and remove UMP5K

                    ForceGear: 19, -@ // Give medkit and remove the rest of items

* Hide "!pm " in chat: https://github.com/TheLouK/Urt-Source-Code/commit/88074d19603331be46943cc0542e024ea8483af8

##### Cvars:

##### Rcon Commands:
* spoof: Send a server command as a specific client.
    code:
        https://bitbucket.org/urtlux/iourt-server-4.1/commits/3df483ae0ad8fea766afd3c357999bf9c2ff987d
* teleport or tp: no explanation needed x)
    code:
        https://bitbucket.org/urtlux/iourt-server-4.1/commits/68cfb456101d1f733b3671f01a5eb219e0dcaa0d
        https://bitbucket.org/urtlux/iourt-server-4.1/commits/2b527a5298af7437e2a284463b3235fd83349a99
* setweapon or sw: remove all weapons except the given (would be wreat if we can set more than one).
* setitem or si: remove all items except the given (would be wreat if we can set more than one).

-