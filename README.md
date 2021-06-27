# Discord.py
A tutorial on how to create a discord bot on python
A modern, easy to use, feature-rich, and async ready API wrapper for Discord written in Python.

Key Features
Modern Pythonic API using async and await.
Proper rate limit handling.
100% coverage of the supported Discord API.
Optimised in both speed and memory.
Installing
Python 3.5.3 or higher is required

# Installing

To install the library without full voice support, you can just run the following command:
```# Linux/macOS
python3 -m pip install -U discord.py

# Windows
py -3 -m pip install -U discord.py```


import discord
from discord.ext import commands

bot = commands.Bot(command_prefix='>')

@bot.command()
async def ping(ctx):
    await ctx.send('pong')

bot.run('token')
