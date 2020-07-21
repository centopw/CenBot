CenBot.
===========

Discord bot make with [nodejs](https://nodejs.org)


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

Ex: to make bot say hi go to ``commands`` create a file name ``hi.js`` and add the modules

```node
const Discord = require("discord.js")
const botconfig = require("../botsettings.json");

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
Or make a Issues post 
