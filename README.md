## What happened in 7.07?
#### -LV launch option has been removed, for no other reason than to kill this mod or at least make it more of a hassle.

Other client-side modding are unaffected!
So Valve does not give a fuck about soviet d2?s and clones cheats that can do 85-90% of what ensa?e can do with client-side modding via gameinfo.gi, but throws a tantrum towards harmless particles-only No-Bling mod. Got it.

Could be an unintended side-effect of some refactoring going on with low violence, but who does not like a little drama flavoured conspiracy? Fact is, mod is dead atm, and the fix is uglier since I can't just safely change `m_hLowViolenceDef` and be done with it. Might as well get rid of resource-compiling and do blind file-replacing. Launch options gets complicated now as it's language-depended, unlike convenient, unified, stand-alone `-LV` _( RIP 2017-11-1 )_

Stay tuned.

---

## No-Bling DOTA "GlanceValue" restoration mod  
#### We all know where we are headed looking at the Immortals spam in the last two years...  

### Glance  
<table>  
	<tr>  
		<td><img src="http://i.imgur.com/QhB7BkT.jpg"></td>  
		<td><img src="http://i.imgur.com/hr0lFC4.jpg"></td>  
	</tr>  
	<tr>  
		<td><img src="http://i.imgur.com/kUIQ7Jh.png"></td>  
		<td><img src="http://i.imgur.com/JShyXKs.png"></td>  
	</tr>  
</table>  
 
## About  
Simply a competent alternative to *Settings -- Video -- Effects Quality* with the main focus on GlanceValue.  
No-Bling<sup>tm</sup> mod is economy-friendly, gracefully disabling particle spam while leaving hats model untouched.  
Might say it even helps differentiate great artistic work, shadowed by the particle effects galore Valve slaps on top.  
  
### How to manually install the zip / vpk releases?  
1. Browse with a filemanager to:  
`\steamapps\common\dota 2 beta\game\`  
2. Delete content of directory:  
`dota_lv`  
3. Unpack release zip file / copy pak01_dir.vpk there  
4. Verify that this file exists:  
`\steamapps\common\dota 2 beta\game\dota_lv\pak01_dir.vpk`  
5. Add Dota 2 LAUNCH OPTIONS:  
`-LV`  
6. Profit!  

### How to quickly restore default particle spam DOTA?
Simply remove / rename the `-LV` launch option!
  
### Before you ask about VAC:  
Don't worry, this is a perfectly safe, well intended, hats friendly, good behaviour particles-only mod,  
ingeniously and optimally using the built-in LowViolence interface, and whitelist-able at a glance...  
  
## No-Bling DOTA mod builder.bat released!  
1. Download `No-Bling DOTA mod builder.zip`, unpack all files, run the included batch script, select build choices  
2. Profit!  
*Requires Windows x64. Does not need Workshop Tools DLC installed, but runs better / faster / more reliable if you have it.*  
  
### No-Bling DOTA mod builder choices:  
Category       | GlanceValue | Description                                                              | Note  
-------------- | ----------- | ------------------------------------------------------------------------ | ----------  
-LowViolence   | **+++**     | Restore Blood: undo -lv launch option turning all blood into alien green | **Essential!**  
Events         | **++++**    | Event Rewards: the International 7 custom tp, blink etc.                 |  
Spells         | **+++++**   | Custom Spells: penguin Frostbite and stuff like that..                   |  
Hats           | **+++**     | Workshop Hats: cosmetic particles spam - slowly turning into TF2..       |  
Heroes!        | **-**       | Default Heroes: model particles, helps potato pc, glancevalue can drop   | **care!**  
Wards          | **++**      | Custom Wards: only a few make the ward and the sentry item similar       |  
Couriers       | **+++**     | Custom Couriers: these are fine.. until a dumber abuses gems on hats     | 
Towers         | **+**       | Penis Contest: just the tower particle effects, models remain unchanged  |  
Soundboard     | **bonus**   | Chatwheel Sounds: silence the annoying chatwheel sounds                  | **temporarily**
*@verbose*     |             | *print file names and export detailed per-hero item lists*               |  
*@refresh*     |             | *recompile mod instead of reusing cached files - usually not needed*     | **dynamic**  
  
*@refresh is shown only if a new patch is detected or source files missing; choices are remembered between runs.*  
  
## DOTA Updates  
With Workshop Tools DLC:  
- Simply run the builder script again to refresh the mod after major patches - it only takes a minute or two  
  
Without Workshop Tools DLC:  
- Builder script creates a local cache directly from game files that gets outdated - simply select @refresh choice  
  
### Notes:  
Due to -lv (lowviolence) being used, you might want to add to your autoexec.cfg:  
`violence_ablood 1; violence_agibs 1; violence_hblood 1; violence_hgibs 1;`  
 
Published under [MIT](LICENSE) license.  
  
