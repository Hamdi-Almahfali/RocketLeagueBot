# RLBot in C#

A Rocket league bot written in c#

## Usage Instructions

--

## Notes

- Bot name, description, etc, is configured by `Bot.cfg`
- Bot strategy is controlled by `Bot/Bot.cs`
- Bot appearance is controlled by `Loadouts/loadout_generator.py`
- To make your bot run as fast as possible, build it in release mode, and then change the "executable_path" in `Bot.cfg` to `./Bot/bin/Release/net6.0/Bot.exe`


## Overview of how the C# bot interacts with Python

The C# bot executable is a server that listens for Python clients.
When `python_run_file.py` is started by the RLBot framework, it connects to the C# bot server and tells it its info.
Then, the C# bot server controls the bot through the `RLBot_Core_Interface` DLL.

## Credit

--
