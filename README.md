# Patch Notes

## Weapons

- Pitchfork
  - up damage: 		61 -> 48
  - left damage: 	45 -> 40
  - right damage: 	45 -> 40
  - down damage: 	25 -> 34
  - down damage_type: 	blunt -> piercing

- Galloglass Axe
  - up damage: 		54 -> 50
  - left damage: 	53 -> 48
  - right damage: 	53 -> 48
  - down damage: 	36 -> 18
    
- Partisan spear
  - down damage: 	35 -> 32

- Battle-axe
  - up damage:		50 -> 45
  - left damage:		40 -> 35
  - right damage:	40 -> 35

- Horseman Hammer
  - up damage:		51 -> 40
  - left damage:		40 -> 35
  - right damage:	40 -> 35

- Mace
  - up damage: 		34 -> 30
  - left damage:		28 -> 25
  - right damage:	28 -> 25

- 2h Swords
  - quick swing charge time right/left up: 	0.45 -> 0.3
  - quick swing charge time down: 		0.45 -> 0.25
  - minimum pose time right/left/up: 		0.43 -> 0.3
  - minimum pose time down: 			0.29 -> 0.25

- Pointy stick
  - up damage:		31 -> 15
  - left damage:		25.1 -> 12
  - right damage:	25.6 -> 12
  - down damage: 	25.5 -> 12

- Daggers
  - penalties non-penetrated:	+25%
  - penalties hard:		+25%
  - penalties.blocked:		+25%
  - penalties.parried:		+25%
  - penalties.miss:		+25%

- Blunt absorption modifiers
  - armour mail: 	0 -> 0.75
  - armour cloth:	0 -> 0.5
  - armour leather:	0 -> 0.75
  - weapon metal: 	0.64 -> 0.8
  - weapon wood:		0.48 -> 0.6

- Cutting absorption modifiers
  - armour plate:	0.75 -> 1
  - weapon metal:	0.56 -> 0.7
  - weapon wood:		0.42 -> 0.525

- Piercing projectile absorption modifiers
  - armour plate:	0.35 -> 0.5

- Fire arrow 
  - damage: 	1.0 -> 0.7

- Barbed arrow 
  - damage:	0.9 -> 0.7

- Swallow tail arrow 
  - damage:	0.9 -> 0.8

- Burning 
  - dps: 	4 -> 3
  - duration:	6 -> 5

- Bleeding 
  - duration:	12 -> 10

- Crossbow active reload succes bonus:
  - standard:	1 -> 0.5
  - pull-lever:	4.5 -> 2.25
  - push-lever:	3.5 -> 1.75

- Eagle-Eyed perk halfed zoom values

## Shields
- Targe 
  - health:		100 -> 80

- Steel Domed Shield
  - health:		100 -> 80
  - encumbrance:		15 -> 12.5

- Hand Pavise 
  - health:		100 -> 80

- Shield bash
  - cooldown		1 - > 4

## Armour

- Almain Munitions Harness 
  - encumbrance: 	11.25 -> 16


## Helmets

- Bascinet
  - absorption:		0.5 -> 0.45
  - encumbrance:		6 -> 7

- Galloglass Bascinet
  - absorption:		0.6 -> 0.5
  - encumbrance:		4 -> 8

- Armet
  - encumbrance:		12 -> 10

- Coifs encumbrances
  - Maille:		0.1 -> 2
  - Galloglass' Mail:	0.1 -> 2
  - Arming cap:		0.1 -> 0
  - Armet bevor:		10 -> 2

- Crests 
  - encumbrance: 	0.1 -> 0.0

- Plumes 
  - encumbrance: 	0.1 -> 0.0

- Feathers 
  - encumbrance: 	0.1 -> 0.0


## Officer Buffs

- For reinforce, courage, and berserker the values per level (number of players) are lowered
  
- Changed that buffs are in cooldown when spawning


## Player Movement

- Interaction priorities changed

- Max rotation speed
  - Regular:		      nil -> 3.0
  - Readying attack:	nil -> 2.0

## Horses

- Hunting horse
  - health:	100 -> 110

- War horse:	
  - health:	100 -> 130

- Noble horse:	
  - health: 	100 -> 120

- Standard Horse armour type:	none -> leather

- Handbrake turn speed:	2.1 -> 1.0

- Changed that braking sets gear to idle

- Changed that charging is only possible at canter speed

- Changed that horses can only bump when charging (server-side)


## Profiles

- Made the first four profiles costumizable

- Added four more profiles


## Server

- Server on previous version are shown yellow (you can still play on them)

- Added option to select tdm map size (small/medium/large) when changing levels (server-side and not test yet)
e.g.: /vote_map St_Albans tdm small

- Added nostalgia settings. When an option is set to true, the old values are used. The following settings can be changed:
  - Weapons - by default false
  - Armour - by default false
  - Backswing - by default true (needs more adjustments to work correctly)
  - Rotation speed - by default false

If you want to change settings: in server_settings.ini add at the end:

```
nostalgia = {
	weapons = true
	armour = true
	backswing = true
	rotation_speed = true
}
```


## Bug Fixes

- Fixed bug that encumbrance of destroyed gear was not calculated correctly

- Fixed bug that during reloading crossbow double speed already could be reached

- Fixed bug that dead horses could bump when running over them
