# Fixing Dual's Revivify Mod to Work With Rain Meadow While Adding Daimyo's Proximity-Based Revival as an Option
___

~~Phew, what a mouthful.~~


## This mod aims to resolve any conflicts between Rain Meadow, the Rain World Multiplayer Framework (and more) mod and Dual's original CPR-based Revivify mod.

While attempting to play Rain Meadow, I had an issue where the original Rain Meadow mod would sometimes work, sometimes not, and was disappointed by that. I was also disappointed by the lack of updates, but ultimately I understand that much. After a point there's only so much more that you can do to a mod before you have to call it done, and even then keeping it updated with the game becomes a hassle.

An attempt to make it Meadow-compatible was attempted by a user of the name Daimyo, and as far as I'm aware, that worked just fine. But unfortunately, they also fundamentally changed the way that the mod worked, switching from a CPR-based revival method to a proximity-based one. That might be fine for some people, but I wasn't happy with it.

So I underwent the process of figuring out how to make Dual's original CPR-based Revivify mod Rain Meadow compatible. Ultimately, it seems like it's just a few functions revolving around updating the player's sprites, and I believe I've resolved those issues just fine. However, I also noticed that Daimyo hasn't updated their mod in a while either, once again leaving Revivify fans without any updates for current versions.

Realizing that there are probably some people who prefer the proximity-based revival, I took the time to try and combine the two methods in the now Rain Meadow compatible mod. Ultimately it was pretty easy, there was just a few tricky bits surrounding Diamyo's original implementation, as it ***seemed*** like the time to revive was based on your framerate instead of on a constant time-based function. I attempted to rectify this and also brought the time to revive a player more in-line with how long it might take to perform CPR on them, so I hope that everyone can appreciate and enjoy these changes, especially online with their friends.

### A full list of any/all changes made in this version of the mod:
* Should now work with Rain Meadow (theoretically, in all supported modes)
* Toggle between Daimyo's Proximity-based revival method, or Dual's original CPR-based revival method in the Remix menu
* Toggle whether or not corpses/comatose slugs can be piggy-backed in the Remix menu
* Daimyo's proximity-based revival has been modified to work as follows:
  * No longer based on framerate (hopefully, close enough anyways)
  * Leaving the proximity causes the dead to become more dead (the longer the corpse i~~~~s dead, the longer they'll take to revive)
  * Entering the proximity causes the dead to become more alive until they are considered alive and revive
  * Corpses should automatically be thrown away once revived

## Apart from the listed changes, the majority of the code is from the original Revivify mod by Dual, source code can be found on [Github](https://github.com/Dual-Iron/revivify/tree/master). Any code from Daimyo's version of the mod came from decompiling the version found on the [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3396726904).
## I'm not asking for any recognition or credit for the code or what it attempts to accomplish, I just wanted the original Revivify mod to be compatible with Rain Meadow. I intend to keep the mod updated with game versions, but ideally it should be pretty version agnostic.
