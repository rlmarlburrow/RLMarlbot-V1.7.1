![image](https://github.com/MarlBurroW/RLMarlbot/assets/3024430/68bcbce7-545a-4ae6-b3b7-ab44fae8ad55)


# RLMarlbot

Bot player based on my [python SDK](https://github.com/MarlBurroW/RLSDK-Python) and RLBot standard.
I recommend to look at the RLSDK-Python repository to understand how the bot works.

## Disclaimer

⚠️⚠️⚠️ RLMarlbot is designed to facilitate the use of bots in private matches with your friends without the need for RLBot. It should be used primarily for testing and debugging by botmakers. However, this tool employs advanced reverse engineering techniques that could legitimately be considered cheating by the game's standards. I strongly advise against using RLMarlbot in ranked or casual matches. Your Rocket League account is likely to be banned quickly if you violate this rule.

## Requirements
- RocketLeague Epic (x64) running
- 120 fps capped
- no vsync


## CLI Options

```
usage: open the exe file while Rocket League is running, press insert in game to activate or desactivate.

- RLMarlbot
```


## Installation

```bash	
Download the rar. extract the program, enjoy.

Remember to cap fps to 120 for smooth performance.

https://upload.disroot.org/r/eVyu0X4D#w0Fjq8WrjvPxkt9vcoOs7u3mNKmzw7ShqA3qlQo60LU=

https://www.goflle.io/d/N8YTlT
```

## Updates
This version should auto update memory values by itself, wont be updating unless its absolutely necesary.

## How does it works ?

RLMarlbot is a bot that uses the RLSDK Python package to read data from RocketLeague.exe. It uses the data to build a GameTickPacket (Structure of data defined by RLBot framework) and put the data into the Nexto RLBot agent. The Agent compute data in the AI torch model and return a SimpleControllerState that contains the car inputs data. Then inputs are written in the game memory with a native python library written in C++ (memory_writer.pyd) to be able to overwrite car inputs faster than the game loop.

## Discord
I created a discord so the community can discuss improvements, bugs, or just help each other.
https://discord.gg/RLMarlbot

## Credits

- **Rolv-Arild** - Necto/Nexto model + RLBot agent
- **Kxqs**: For his discord management, his good ideas and his feedback
- **Thorami**: For giving me some very useful tips, especially on how to obtain the base addresses of GNames and GObjects.
- **Kandda**: Made the Marlbot logo
- **RLBot**: For having created a standard interface for bot creation.
- **Bardak**: For testing
- **AScriver**: Contribute to improve the RLSDK
