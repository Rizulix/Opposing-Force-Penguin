# Opposing Force Penguin

> Op4 "weapon_penguin" for Sven Co-op

## Installation Guide

1. [Download this repository](https://github.com/Rizulix/Classic-Weapons/archive/refs/heads/main.zip) and extract its content inside `Steam\steamapps\common\Sven Co-op\svencoop_addon\`.

2. Open your map_script: *`my_map_script.as`*. (this name is only for reference)

3. In the header add `#include 'opfor/weapon_penguin'` and in the `MapInit()` function add `CPenguin::Register();` this will register the weapon.

	It should look like this:
	```angelscript
	// Assuming that your map_script is in `../scripts/maps/`
	#include 'opfor/weapon_penguin'
	
	void MapInit()
	{
		CPenguin::Register();
	}
	```

4. Add `map_script my_map_script` in the *.cfg* corresponding to the map.

5. Now you can create this weapon for your maps, enjoy!

## Credits

* Code format based on [KernCore's Custom Weapon Projects](https://github.com/KernCore91#sven-co-op-plugins)

* Weapon code was ported/based from SamVanheer's [Half-Life Unified SDK](https://github.com/SamVanheer/halflife-unified-sdk) and [Half-Life Op4 Updated](https://github.com/SamVanheer/halflife-op4-updated)