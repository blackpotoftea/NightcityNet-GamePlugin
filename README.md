# NightCityNet

An LLM-driven NPC brain for Cyberpunk 2077: NPCs who remember what you said, know where they are,
and answer in a voice of their own — cloned from their lines in your game, if you say you have
permission.

## Download

Get the latest build from **[Releases](https://github.com/blackpotoftea/NightcityNet-GamePlugin/releases/latest)**.

Each release has one zip per game patch. Pick the one whose name matches your game:

| Zip | Game version |
|---|---|
| `NightCityNet-<version>-game2.31.zip` | Cyberpunk 2077 2.31 |
| `NightCityNet-<version>-game2.5.zip` | Cyberpunk 2077 2.5 |
| `NightCityNet-<pack>-adapter-<version>.zip` | Optional — maps a sound pack you own (see the README in the zip) |

## Required mods

Install these first.

| Mod | Why |
|---|---|
| [RED4ext](https://github.com/WopsS/RED4ext) | loads the brain DLL |
| [Cyber Engine Tweaks](https://github.com/maximegmd/CyberEngineTweaks) | the Lua bridge |
| [redscript](https://github.com/jac3km4/redscript) | compiles our scripts |
| [Codeware](https://github.com/psiberx/cp2077-codeware) | the UI |
| [ArchiveXL](https://github.com/psiberx/cp2077-archive-xl) | mounts our archives |
| [TweakXL](https://github.com/psiberx/cp2077-tweak-xl) | applies our tweaks |
| [Boneware v0.1.3](https://github.com/Mozz3d/Boneware/releases/tag/v0.1.3) | NPC faces. **Not on Nexus, and the one most people miss — without it nothing of ours loads** |

Optional: [Input Loader](https://github.com/jackhumbert/cyberpunk2077-input-loader) for default key
bindings and clean hold-to-talk.

## Install

- **Manual:** extract the zip into your Cyberpunk 2077 folder, so `bin\`, `r6\`, `archive\` and
  `red4ext\` land beside `Cyberpunk2077.exe`.
- **MO2 / Vortex:** install the zip as a mod. It is already in game-root layout.

Then start the game (a full restart, not a CET reload) and open the control panel at
<http://127.0.0.1:8477/>. A fresh install opens on the setup screen: an API key for the AI
(OpenRouter by default, or a local model with no key), a voice service (or none), and an optional
microphone.

The full guide — settings, sound packs, how to pay, promote, recruit and equip NPCs — is
`NightCityNet\README.txt` inside the zip.

## Something wrong?

1. Run `NightCityNet\NightCityNet-CheckInstall.bat` first. It names every missing, damaged or
   left-over file and writes `NightCityNet\install-check.txt`.
2. After a crash, run `NightCityNet\NightCityNet-CrashReport.bat`. It writes one zip to your
   Desktop with API keys and your user folder taken out.
3. No crash but something is off: in the panel, **Debug → Report → Generate zipped report**.

Attach those to your report in [Issues](https://github.com/blackpotoftea/NightcityNet-GamePlugin/issues).
The crash dump inside the zip is a snapshot of the game's memory — send it to the developers rather
than posting it in public.

## Licence

NightCityNet is © 2026 blackpotoftea. See [LICENSE](LICENSE). Bundled third-party components keep
their own licences, shipped in `licenses\` inside the zip.

## Credits

Inspired by these mods — go and endorse them:

- [Night City Allies - Immersive Companion System](https://www.nexusmods.com/cyberpunk2077/mods/27625)
- [The Grid (Custom Street Light Hours - Weather Effects - Blackouts)](https://www.nexusmods.com/cyberpunk2077/mods/34592)
