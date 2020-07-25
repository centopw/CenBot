CenBot.
===========
[![Discord Users Online](https://discordapp.com/api/guilds/483209992980135936/widget.png?style=shield)](https://discord.gg/BVu2SaC)

A Discord bot make with Love and [nodejs](https://nodejs.org)


Setup.
=============

Make sure you have install [nodejs](https://nodejs.org)

Navigate to project folder and install all dependencies:
   
   ``$ npm i``

Add your bot token (Create one [here](https://discord.com/developers/applications)) in ``botsettings.json``

To run the bot:

   ``npm index.js``

Add or remove command.
=====================

Go to ``/commands`` 

Ex: to make bot say hi, go to ``commands`` create a file name ``hi.js`` and add

```node
const Discord = require("discord.js")
const botconfig = require("../botsettings.json");//load bot config

module.exports.run = async (bot, message, args) => {
    return message.channel.send("Hello") //return the text Hello
}

module.exports.config = {
    name: "hi",//Name of the command
    description: "",//description for the command
    usage: "hi",//run the command 
    accessableby: "Members", //what permission requre to run the command
    aliases: ['h'] //another way to use the command
}
```
Dependencies.
============
  - discord.js
  - moment

ToDo.
====

 - Optimize the code
 - Add more modules
 - A full document on how to setup & run
 
 
Source code
===========

https://github.com/centopw/CenBot

Contact
=======
For all Question contact me:
centopw@gmail.com

Join out community [DevHub](https://discord.gg/BVu2SaC)

[![Support Server](https://discordapp.com/api/guilds/483209992980135936/widget.png?style=banner2)](https://discord.gg/BVu2SaC)
