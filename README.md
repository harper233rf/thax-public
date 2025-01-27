# thax

Literally the most powerful minecraft cheat ever made, in a light and public release.

Updated with mods we think would be good for public use.

In case you cannot read, this is a fork of fr1kin's ForgeHax. Since the 1.12.2 branch is not actively developed, we added more stuff in ourselves.

### Maintaining

TheAlphaEpsilon, OverFloyd, FraazT0 and Fleyr have contribuited on the dev repo and will help keep this updated.

### Discord support
You can join a very Work-In-Progress discord server [HERE](https://discord.gg/8QjDRRPyeh). No guarantee is made about server being _not dead_.

## Installing

1. Get Minecraft
7. Install this as a Forge Mod
420. profit

## Wiki

If you need any help, please check the [ForgeHax Wiki](https://github.com/fr1kin/ForgeHax/wiki) before submitting an issue.
No really, fr1kin's wiki is well kept and covers some basic and generic shit. I won't make a wiki as cool as that one for this fork.

## Capes

We have extra textures! Upload [HERE](http://texture.fantabos.co)

## External Connections (Read this if you don't want to leak your IP)

This mod will get data from:
* Minecraft's API (api.mojang.com, sessionserver.mojang.com)
* 2b2tatlas.com (only if using Atlas mod, will never send your coords)
* data.fantabos.co (only if using custom Capes)
* irc.fantabos.co (only if using IRC)

This is relatively safe, as it is essentially just going to these websites on a browser. **Any connection to any service will make its source known to the receiving server**.

This mod will send data to:
* irc.fantabos.co (only if using IRC)

Please note: IRC identifies users by IP. If the server you're connecting to does not enforce IP masks, your IP will be shared will any user requesting it. `irc.fantabos.co` does mask your IP, and so does `irc.freenode.net`. Private servers might not do so, **investigate server policies before connecting to unknown IRC hosts**.

As always, use of a VPN can hide your IP address from others.

### IRC

By default, the IRC service won't connect to anything. If you wish to use IRC chat, turn on `.irc auto-connect`. It is set to connect to `irc.fantabos.co` by default and join the `#fhchat` public channel, but neither is enforced.

## Known Issues

Most recent Optifine release breaks Markers. All Optifine releases break XRay. (Also XRay isn't really XRay but install Wurst ffs)

## Building

You will need to first set up a local copy of the main repo:

**For Windows**:
1) Download, clone, or pull the files
2) In command prompt cd to the folder
3) Run `gradlew setupDecompWorkspace` (try `gradlew setupDecompWorkspace --no-daemon` if this fails)

Commands above vary slightly depending on used shell (`cmd`, `powershell`), try also `gradlew.bat` , `./gradlew.bat`, `./gradlew`.

**For Linux/MacOS**:
1) `git clone https://github.com/tonio-cartonio/fantabos.co.git`
2) `cd fantabos.co`
3) `./gradlew setupDecompWorkspace`

Once you have a local copy, you can update it every time we push a new commit just by doing `git pull` inside the project folder.
To build, run `./gradlew build`, jar will be in `build/libs`:

1) `./gradlew build` or `gradlew build` or `gradlew.bat build` or `./gradlew.bat build`
2) built jars will be in main project folder `/build/libs` (don't use the one with `-sources` at the end!)

## Why are you making this public

Because I can. I used to have quite exclusive haccs but now everyone seems to have them. I want to share the way I did things.
