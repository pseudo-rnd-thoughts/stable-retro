# Stable-Retro

A fork of gym-retro with additional games. Since gym-retro is in maintenance now and doesn't accept new games, plateforms or bug fixes, you can instead submit PRs with new games or features here in stable-retro.

Currently added games on top of gym-retro:
*	Super Mario Bros 2 Japan (Lost Levels) - NES
*	Hang On - SMS
*	Punch Out - NES
*	WWF Wrestlemania the Arcade Game - Genesis
*	NHL 94 - Genesis
*	NHL 94 (1 on 1 rom hack) - Genesis
*	Super Hang On - Genesis
*	Tetris - GameBoy
*	Virtua Fighter 2 - Genesis

PvP game that support two models fighting each other:
*	Samurai Showdown - Genesis
*	WWF Wrestlemania the Arcade Game - Genesis
*	Mortal Kombat II - Genesis
*	NHL 94 - Genesis

As well as additional states on already integrated games.

## Bug Fixes
*	Fixed UI flickering issue in OpenAI integration tool
*	fix compile with c++ >=17

## Installation

```
git clone https://github.com/MatPoliquin/stable-retro.git
cd stable-retro
pip3 install -e .
```

## Citation

```
@misc{stable-retro,
  author = {Mathieu and Poliquin},
  title = {Stable Retro, a fork of OpenAI's gym-retro},
  year = {2021},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/MatPoliquin/stable-retro}},
}
```

## Tutorials

Game Integration tool:
https://youtube.com/playlist?list=PLmwlWbdWpZVtH6NXqWbrnWOf6SWv9nJBY

# Gym Retro

Gym Retro lets you turn classic video games into [Gym](https://gym.openai.com/) environments for reinforcement learning and comes with integrations for ~1000 games.  It uses various emulators that support the [Libretro API](https://www.libretro.com/index.php/api/), making it fairly easy to add new emulators.

Supported platforms:

- Windows 7, 8, 10
- macOS 10.13 (High Sierra), 10.14 (Mojave)
- Linux (manylinux1)

CPU with `SSSE3` or better

Supported Pythons:

- 3.6
- 3.7
- 3.8

Each game integration has files listing memory locations for in-game variables, reward functions based on those variables, episode end conditions, savestates at the beginning of levels and a file containing hashes of ROMs that work with these files.

Please note that ROMs are not included and you must obtain them yourself.  Most ROM hashes are sourced from their respective No-Intro SHA-1 sums.

# Documentation

Documentation is available at https://retro.readthedocs.io/en/latest/

You should probably start with the [Getting Started Guide](https://retro.readthedocs.io/en/latest/getting_started.html).

# Contributing

[See CONTRIBUTING.md](https://github.com/openai/retro/blob/master/CONTRIBUTING.md)

# Changelog

[See CHANGES.md](https://github.com/openai/retro/blob/master/CHANGES.md)

# Emulated Systems

- Atari
	- Atari2600 (via Stella)
- NEC
	- TurboGrafx-16/PC Engine (via Mednafen/Beetle PCE Fast)
- Nintendo
	- Game Boy/Game Boy Color (via gambatte)
	- Game Boy Advance (via mGBA)
	- Nintendo Entertainment System (via FCEUmm)
	- Super Nintendo Entertainment System (via Snes9x)
- Sega
	- GameGear (via Genesis Plus GX)
	- Genesis/Mega Drive (via Genesis Plus GX)
	- Master System (via Genesis Plus GX)

See [LICENSES.md](https://github.com/openai/retro/blob/master/LICENSES.md) for information on the licenses of the individual cores.

# Included ROMs

The following non-commercial ROMs are included with Gym Retro for testing purposes:

- [the 128 sine-dot](http://www.pouet.net/prod.php?which=2762) by Anthrox
- [Sega Tween](https://pdroms.de/files/gamegear/sega-tween) by Ben Ryves
- [Happy 10!](http://www.pouet.net/prod.php?which=52716) by Blind IO
- [512-Colour Test Demo](https://pdroms.de/files/pcengine/512-colour-test-demo) by Chris Covell
- [Dekadrive](http://www.pouet.net/prod.php?which=67142) by Dekadence
- [Automaton](https://pdroms.de/files/atari2600/automaton-minigame-compo-2003) by Derek Ledbetter
- [Fire](http://privat.bahnhof.se/wb800787/gb/demo/64/) by dox
- [FamiCON intro](http://www.pouet.net/prod.php?which=53497) by dr88
- [Airstriker](https://pdroms.de/genesis/airstriker-v1-50-genesis-game) by Electrokinesis
- [Lost Marbles](https://pdroms.de/files/gameboyadvance/lost-marbles) by Vantage

# Citation

Please cite using the following BibTeX entry:

```
@article{nichol2018retro,
  title={Gotta Learn Fast: A New Benchmark for Generalization in RL},
  author={Nichol, Alex and Pfau, Vicki and Hesse, Christopher and Klimov, Oleg and Schulman, John},
  journal={arXiv preprint arXiv:1804.03720},
  year={2018}
}
```
