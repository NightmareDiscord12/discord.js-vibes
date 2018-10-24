__Support server__

[Discord Vibes](https://discord.gg/zf46prb)

__Commands__

play {Search String} | Plays the song selected.

pause | Pauses the playing song.

resume | Resumes the paused song.

leave | Leaves the channel the bot is on.

skip | Skips the playing song.

queue | Shows you all songs in the queue.

loop | Enables or disables song repeat.

volume {Number || current} | Shows you the current volume or changes the volume depending on what you type.

__Basic Example__

```javascript
const Discord = require("discord.js");
const Music = require("discord.js-vibes");

let bot = new Discord.Client();

Music.start(bot, {
    youtubeAPIKey: 'YOUTUBE_API_KEY'
  });

bot.login("BOT_TOKEN");
```

__Full Example__

```javascript
const Discord = require("discord.js");
const Music = require("discord.js-vibes");

let bot = new Discord.Client();

Music.start(bot, {
    youtubeAPIKey: 'YOUTUBE_API_KEY',
    prefix: 'BOT_PREFIX', //Default if '!'
    embedColor: 'EMBED_COLOR', //Use a HTML color code
    maxVolume: 200 //Default 200 
  });

bot.login("BOT_TOKEN");
```

__Infomation__

This module is my first. For getting options and queue i got some of the code from telk-music and discord.js-musicbot-addon. The rest of the code is from me.