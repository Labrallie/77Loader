# 77Loader

Hacky Mac OneLoader port that adds support for the official macOS port of OMORI, which does not use the /www subfolder. Forked from its currently inactive version to add the latest OneLoader features.

77Loader features:
- adds support for the official macOS port of OMORI, which does not use the /www subfolder
- brings back support for nwjs 0.77.0 (required by the Apple Silicon compatibility patch) which was present in 1.2.1

To install on a Mac:
1. If you are on a Apple Silicon machine: Apply [this compatibility patch](https://github.com/SnowpMakes/omori-apple-silicon/blob/master/patch.md)
2. Download [77Loader](https://github.com/Labrallie/77Loader/releases/latest) and extract the ZIP file
3. In your Steam library, right-click OMORI and open local game files
4. Right-click the file `OMORI.app` and press "View package contents"
5. Enter `Contents`, then `Resources`, then `app.nw` folders
6. In another Finder window, open the `www` folder you extracted from the ZIP file earlier, copy all files inside it (NOT the folder itself) and paste it into the `app.nw` folder, then replace files when asked
7. Have fun!

If you want to install this on a Windows machine for easier modpack distribution or using newer nwjs versions, this is working just fine - you can install exactly like you would install OneLoader.

Please note that I am not normally a dev, as such there may be bugs present in this version.

Please feel free to report any bugs on the tracking page, or reach out to me over Discord (Username is labrallie) through DMs, via the [OMORI discord](https://discord.gg/omori) (Simply tag me in modding-discussion), via the [mods.one discord](https://discord.gg/EDTMF85Hnp) or through the OMORI Modding Discord!

A very special thanks to [rphsoftware](https://github.com/rphsoftware), [nift4](https://github.com/nift4), and [Gilbert142](https://github.com/Gilbert142) for their contributions to OMORI modding!

## Credits/Licensing
This project contains in part or in full the following projects:

- [GOMORI](https://github.com/gilbert142/gomori) | License: **MIT** | Degree of use: Certain encryption primitives, the index.html used for backwards compatibility
- [node-stream-zip](https://github.com/antelle/node-stream-zip) | License: **MIT** | Degree of use: Library used in full to process mods bundled in zip files
- [JSON-Patch](https://github.com/Starcounter-Jack/JSON-Patch) | License: **MIT** | Degree of use: Library used in full to apply patches to game data
- [Rollup](https://github.com/rollup/rollup) | License: [Multiple](https://github.com/rollup/rollup/blob/master/LICENSE.md) | Degree of use: Building plugins shipped as ES modules
- [OneLoader](https://github.com/rphsoftware/OneLoader) | Licesnse: **MIT** | Degree of use: Source code based on this project