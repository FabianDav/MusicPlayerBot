# Telegram Music Player

An Telegram Bot to Play Radio/Music in Channel or Group Voice Chats.

This is also the source code of the bot which is being used for playing Music in [FlixAr](http://t.me/FlixAr_uniqX) official Movie, TV Series Channel of UNIQX Family.

## Special Features

- Playlist, queue, 24x7 radio stream
- Loop one track when there is only one track in the playlist
- Automatically downloads audio for the first two tracks in the playlist to ensure smooth playing
- Show current playing position of the audio
- Control with buttons and commands
- Download songs from youtube as audio

## Deploy to Heroku (The Easy Way)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/FabianDav/MusicPlayerBot)

## Heroku Vars:
1. `API_ID` : Get From my.telegram.org
2. `API_HASH` : Get From my.telegram.org
3. `BOT_TOKEN` : Get it From @Botfather
4. `SESSION_STRING` : Generate From [@genStr robot](http://t.me/genStr_robot).
5. `CHAT` : ID of Channel/Group where the bot plays Music/Radio.
6. `LOG_GROUP` : Group to send Playlist, if CHAT is a Group.
7. `ADMINS` : ID of users who can use admin commands.
8. `STREAM_URL` : Stream URL of radio station to stream when the bot starts or with /radio command.

- Enable the worker after deploy the project to Heroku.
- Bot will starts radio automatically in given `CHAT` with given `STREAM_URL` after deploy. 
- 24x7 Music even if heroku restarts, radio stream restarts automatically.  
- To play a song just send the audio file to Bot or reply to an audio with `/play` to start playing it in the voice chat.
- To download audio you can use `/song` command.
- Use `/help` to know about other commands & its usage.

## Requirements

- Python 3.6 or higher.
- A
  [Telegram API key](https://docs.pyrogram.org/intro/quickstart#enjoy-the-api)
  and a Telegram account.
- [FFmpeg Python](https://www.ffmpeg.org/)
- Userbot Needs To Be Admin In The Channel or Group.
- Must Start A Voice Chat In Channel/Group Before Running The Bot.

## Run On VPS (The Hard Way)

```sh
$ git clone https://github.com/FabianDav/MusicPlayerBot
$ cd MusicPlayerBot
$ sudo apt-get install ffmpeg
$ pip3 install -U pip
$ pip3 install -U -r requirements.txt
```
Edit **config.py** with your own values.

```sh
$ python3 main.py
```

## License
```sh
MusicPlayerBot, Telegram Voice Chat Userbot
Copyright (C) 2021  UNIQX Family

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>
```
## Credits

- [Asm Safone](https://github.com/AsmSafone) [Dev]
- [Dash Eclipse](https://github.com/dashezup) [For tgvc-userbot]
- [Il'ya](https://github.com/MarshalX) [For tgcalls]
- [Subin](https://github.com/subinps) [For bot support]
