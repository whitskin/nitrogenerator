# nitrogenerator
```js
const Discord = require('discord.js'); const generator = require('generate-password'); const talkedRecently = new Set(); exports.run = function(client, message, args) {       var password = generator.generate({         length: 16,         numbers: true,         //random: true,     }) if(!message.guild) return;     message.channel.send( new Discord.RichEmbed() .setColor('#7FFF00') .setDescription("**✅ Nitro code sent in DMs!**")) message.author.send('https://discord.gift/' + password) message.author.send('Nitro Kodları Kontrol Edilmez'); };    exports.conf = {   enabled: true,    guildOnly: false,    aliases: [],   permLevel: 0  };  exports.help = {   name: 'nitro',    description: 'Rastgele Nitro Kodu Üretir',   usage: '' };
```
