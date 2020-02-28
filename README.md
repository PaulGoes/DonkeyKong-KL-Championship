# Donkey Kong Arcade - Kong League Championship

Kong League Championship

This is the Donkey Kong - Kong League Championship rom-hack for the arcade version of Donkey Kong.

The idea is to have a Donkey Kong version with a shorter gameplay by introducing the famous Kill Screen at an earlier level. 
This version could be used in one-on-one or head-to-head games and tournaments.

![DKC Title Screen](https://github.com/PaulGoes/DonkeyKong-KL-Championship/blob/master/Title%20Screen.jpg)

The game defaults to a Kill Screen at level 11. But this is configurable using the dip switches that normally control the bonus life threshold. The bonus life threshold is now fixed at 7000. The following dip switch settings control the Kill Screen level:

- Dip switches - 00 - Kill Screen at level 11 (originally bonus life at 7000)
- Dip switches - 01 - Kill Screen at level 09 (originally bonus life at 10000)
- Dip switches - 10 - Kill Screen at level 07 (originally bonus life at 15000)
- Dip switches - 11 - Kill Screen at level 05 (originally bonus life at 20000)       

The selected Kill Screen level is shown in the level progress screen:

--> plaatje invoegen met Let's Go For The KS At L=... waarin KS level te zien

As an extra the game detects it when the player loses his/her last life because of the Kill Screen. Then it doesn't display the normal 'GAME OVER' message but displays a 'KILL SCREEN REACHED' message instead and plays an accompanying melody.

--> plaatje invoegen met melding Kill Screen Reached

One additional thing. During the design I restricted myself to the following constraints:
- Use the orginal dkong rom (US version). This meant that I only had around 256 bytes of free space to put my changes in. Quite a challenge I must say!
- Do not change anything in the core gameplay logic. This was possible because the bonus timer is calculated before the level/screen starts to play so the required change doesn't impact the gameplay itself.

On most other emulators (e.g. WolfMame) you can play this game by replacing the original dkong.zip by this Kong League Championship version of the dkong.zip. You have to start the emulator without checksum checking (in WolfMame by starting it from the command line and specifying the romname).

