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

    * [Streamer.Bot Care Stream DBIS Configuration](https://hastebin.com/share/socejiluye.bash)

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
