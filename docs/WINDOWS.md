# Windows Setup (for Secure Twitch  Livestreams in Long Term Care Facilities)

If you’re considering using a monitoring device in a long term care facility, a livestream may be a more beneficial option. Read about the benefits of care streaming here.

This tutorial offers care streamers (and their caregivers) privacy options through simple viewer/administrator chat commands that change the OBS scene, obscuring viewer video/audio fee.

Don’t get too overwhelmed, a tutorial will be up shortly! 

## Needs (* means required)
* **Broadcasting Software**: [OBS](https://obsproject.com/*)
* Twitch Account* ([Signup](https://www.twitch.tv/signup))
* **Digital Bystander Intervention Strategies*** (Privacy Overlay, Alarm Commands, Alert Notification Commands)
* [Twitchat](https://twitchat.fr/) (**easy**) or [Streamer.Bot](https://streamer.bot/) (**harder but customizable**)
* [Streamer.Bot Care Stream DBIS Configuration](https://hastebin.com/share/socejiluye.bash) or Twitchat (TBD) 

## OBS Setup
* Install OBS [Install](obsproject.com/downloads/)
* Install Streamer.Bot [Install](https://streamer.bot/)
* Link OBS to Twitch: File < Settings < Stream < Connect Account (**Recommended**) < **Login with Twitch Credentials**

##### Alternatively:
* **Get Stream Key**([Here's How](https://help.twitch.tv/s/article/twitch-stream-key-faq?language=en_US&quot)) < Navigate to **Creator Dashboard** < Settings < Stream < **Copy Stream Key** < Paste into OBS Stream Key < Ok

### Connect Twitch to Streamer.Bot
* Open Streamer.Bot < Platforms < Accounts < Click Login under Broadcaster Account < Sign in with Twitch Credentials

### Connect OBS to Streamer.Bot
* Open **OBS** < Tools < **WebSocket Server Settings** < **Show Connect Info** < Copy **Password**
* Click **Stream Apps** < Right Click Empty Space < Paste Password from WebSocketServer Settings < Enable Auto Connect on Startup < Enable Reconnect on Disconnect

## Import Streamer.Bot Configuration:
* Open **Streamer.Bot** < Click **Import** < Paste the following string into the "String":

```
U0JBRR+LCAAAAAAABADtWNtu3DYQfS/Qf1C2cJECoUuKokjlLd42bVC0KOI2QFHkYUiO1kJ02VKSLwj876W0V620wcJ1ggTok1c85Ax5Zjhn6PdffxUEs2t0dVaVs+cBf9YPZMWycs2bw+EiK7OiLXbjM3oenvPZGsUG/Nj77sN/llBgN+WycQjFX1Xr5uAwuHh9EXwbXIB5t1rmZ0LbXFWum5tn11m5yEq4uULMzRVkbjtrt8kZO6fndAtYrI3Lls0avLzJGnOFdaCxuUEsg0uDJT7vHUNpN5/9n+A6g+CJdrpHnuiDXVWv2/KFWRsu2zzvoPvVaS0MTgv9tNqP/L0aCTZQD2e225oxBtIkTgjXIiIRpTEBJjWxQJlglkuRhhv//bJ/Wmxx7Xt/HEvQOXY2G9fiALk1eWvxpauKn7O6qdydn5RCXg9mbWLjORn4W7iqXXbADxevLgcI5DdwV3s+psw5z15VbJka4aYqTescls0U2rhssfDB3efugL+1laLwjl71VKaUR1wyRqg21FMpQqK5lkRKHsZM8iRJ5f4B9qOgQTOIkChLDYk0pUSHYInhqBlGSUS1HS1t7pYdYxFlh8jRWOziUW9S4+0+er/7eDugepxKU3TUXQL/Nh3IDesl9rZWlIWhZyW2mggaS09ZyknCeUzCOPFs2DSm7BhlYWSAG+nnKslJJDT4xEVLJEOeMGu1VjBaeoPZ4qqLuL+sR+jk0SGwycCDjD+B6ay0eNvZHHD87EMUXkPeX6/ZWVYu24adjc5QwO2bzSQ6Qld5P5HTe9RZlAq4tiSKEEiECSPK5y4xilmldJgo9iDqGKXh45MXnU5eg7fdDme/u+wazF1Q+QKdw11wBV3p9XV37TFIKxecaVeBNVA3f9bozgJogrMmK/B5OuZ86TBFXy3sC2Oqtq8ZIxLW3MaR5TTxtCoTE5+jQBKhkNgwjWOuMWURPozbY8zORuZO45Wdzuv6aNZIa8KYpBL9jUt8aVNCpj6BdMKlNNao6CFHC0f1678ejT7gvm01uqmC5TB/vn/qa9l3E8UsX7UI31D68iUd38UVbYwlBqwvajGPBYlCkCRRUUx4EsZa+pvIonFtP+22JY9NXHi6GPzUuVopyFBX8xyWNdo9fAPvIjHuQzBEVAIVCWWSeJZi9Pem+wxDyhAMw0R/2j7kxfyXL7QRUbFNQcVArGG+EFl/W0HalGjFla8/yifcuL6vGxGhZWwFEBqC72EEl0T7ykmk8nLKfFQgFV9aI9K31R+zFQGZWJEKRYT1LEfg1ytlkaQWY+F/cGHM59KKDG/4aaWRCTpR3R6hDxGCK6Gk5y3qBDM1JEEFvuvlEQCG0vcjj92HfAK1HEtK94jrdOUGtYHi+6erhx57sKQIJiREKiI29mkW8VASSCwnyFjEQUMcRuxzkZShFj+6pKx+bOavVGFgYlMaj76D66p1BkclhR7Z6hJdkTUN2q5rHG92Cx85TPagp+JWlbQbquAuBiPpyMpe7iaEsKj6YTokuWep8/Hk0InDBd7+eLvMM5M1c1g2rcMpj3llYC1zA9vZoqwcXlTNrnse77af86ps0JWQT2x62f2vpW7mnQF000q6gejEwi5cH1jc7uAuaO/vB5ahxkss66zJridPvsgrDfm8qnJb3YzOv7I9jU1eLz8KZfPH6lJuE3G6ffro6btvdfarTx0HvneqZ0ccrCUxYalmQpNQGF+htG9GEk69pHYPCMEs41xMJvjc01y5j5/jZuzn/zT/PNL8oKR70awr8w6bS3TXBzm7A+d55lvoIdi95t1OL7zh+38BOd1jv10WAAA=
```

* Click **Ok**

## Enable DBIS Commands
* Go to the **Commands** tab in **Streamer.Bot**:

* Right Click !brb < Enable 

* Right Click “!back” < Enable 

* Right Click “!censor” < Enable

## Test the Commands
* Open OBS < Click “Start Streaming”

* Open your Twitch chat and type !brb, the following screen should come up.(example)

* Typing !back should take you back to your webcam scene.

    * (Optional) !censor 10000 - changes scene to privacy screen for 10 seconds.

If you'd like to help seniors or their families set up monitoring livestreams, please get in touch with the Faulkner Foundation via [Discord](https://discord.gg/KG6Jj6k9tF)
