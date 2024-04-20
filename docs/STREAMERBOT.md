# Streamer.Bot Guide for Windows

### Needs

* **Broadcasting Software**: OBS for Windows ([Download](https://obsproject.com/download))

* **Livestream ChatBot**: Streamer.Bot ([Download](https://streamer.bot/downloads))

* **Chatbot Configurations**: Streamer.Bot Command Configs (Download All)

    * !alarm

    * !alert

    * !censor

    * !valarm

    * !valert

### Install OBS

* Configure OBS
    * Create Scene 2 named "BRB" with Privacy Overlay Image Source
    * Enable Websocket Server Settings
        * Copy Websocket Server password

### Install Streamer.Bot

* Configure Streamer.Bot
    * Link Streamer.Bot to Twitch
    * Link Streamer.Bot to OBS
    * Import Commands
    * Enable Commands

### Test Out Streaming and DBIS Commands

### Voice Commands

Import the following code into your ```settings.json``` file:
```
**
    {
        "id": "4ab050ee-a954-4bd8-a999-ab826d740412",
        "enabled": true,
        "name": "privacy",
        "type": 0,
        "command": "oddysey",
        "overrideGlobalConfidence": true,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "ed71b0ad-b454-4a25-aeeb-b437ba479dfd",
        "enabled": true,
        "name": "vBACK",
        "type": 0,
        "command": "return",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "4213a66a-495a-4ff9-b0ea-b5e94cfc7917",
        "enabled": true,
        "name": "vBACK2",
        "type": 0,
        "command": "stream",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "3a417120-7ac6-4f18-a6e4-5738e07821d5",
        "enabled": true,
        "name": "disconnect",
        "type": 0,
        "command": "shut down the stream",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "432618a0-c736-4532-9c5a-d4d5355bafdd",
        "enabled": true,
        "name": "connect",
        "type": 0,
        "command": "start the stream",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "3964c246-f350-4d84-aee9-719715eb3c88",
        "enabled": true,
        "name": "subtitles",
        "type": 0,
        "command": "subtitles please",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "7bbda7d3-b2cf-4af2-9119-b4388626437d",
        "enabled": true,
        "name": "checkinOkay",
        "type": 0,
        "command": "vSafetyCheck",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "53e892e7-d841-462f-8be1-0dd92898daad",
        "enabled": true,
        "name": "checkinokay2",
        "type": 0,
        "command": "I'll need a minute",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "45104a37-87d8-499f-8de7-df0bc135619d",
        "enabled": true,
        "name": "privatebroadcastmessage",
        "type": 1,
        "command": "armadillo",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "8e1e4642-c773-452a-87be-d61c58727c29",
        "enabled": true,
        "name": "vodReviewReminder",
        "type": 0,
        "command": "reminder",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "628ff598-7ac9-4165-b796-35cfb782f649",
        "enabled": true,
        "name": "voiceSocials",
        "type": 0,
        "command": "social",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "5868c6fb-a9d7-4349-a49e-aa30114c2806",
        "enabled": true,
        "name": "voiceAlert",
        "type": 0,
        "command": "emergency",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "8093ca24-a1fe-4770-9460-2fe52759ab0c",
        "enabled": true,
        "name": "voiceCam",
        "type": 0,
        "command": "toggle camera",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "b2dde7db-b332-4de7-bf1a-4071d4a0f63d",
        "enabled": true,
        "name": "voiceMute",
        "type": 0,
        "command": "Toggle Microphone",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "dc526721-c65f-4f50-8f92-9bea52009b53",
        "enabled": true,
        "name": "staff notification",
        "type": 0,
        "command": "signaling",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "52d2015a-be99-4a37-8492-a442670c6444",
        "enabled": true,
        "name": "voiceFalseAlarm",
        "type": 0,
        "command": "false alarm",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "04205cca-00b7-45b9-912f-585721ab3306",
        "enabled": true,
        "name": "startRecording",
        "type": 0,
        "command": "action please",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "c0f3cf52-ddc3-4b5d-8814-518c11290740",
        "enabled": true,
        "name": "voiceGeo",
        "type": 0,
        "command": "city explorer",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "5fa99c30-8348-481e-9741-85483ad02097",
        "enabled": true,
        "name": "slow mode",
        "type": 0,
        "command": "vSlowmode activate",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "1ef656fc-0c5d-4fb1-9e84-20628d754aef",
        "enabled": true,
        "name": "slowmode Off",
        "type": 0,
        "command": "vSlowmode off",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "8048e675-a104-41fb-a541-7cb754c7b6a9",
        "enabled": true,
        "name": "shieldMode",
        "type": 0,
        "command": "safe talking",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "85c4a9b3-d357-40e9-8ba2-4f500fb4e7a9",
        "enabled": true,
        "name": "stopRecording",
        "type": 0,
        "command": "stop the stream please",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "71797c2b-f12b-48da-a060-bdefd8ea04d6",
        "enabled": true,
        "name": "voiceVodMarker",
        "type": 0,
        "command": "time stamp please",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "ac5758c7-0c92-4b9e-8182-e3963f4e80bc",
        "enabled": true,
        "name": "checkinRequest",
        "type": 0,
        "command": "Cyprus Hill",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "9579ad37-4043-4c81-b23c-8421ee7eb4ef",
        "enabled": true,
        "name": "focusOBS",
        "type": 0,
        "command": "toggle open broadcaster",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "e4adccc9-88b9-4d0c-80c5-dc39a25c41ea",
        "enabled": true,
        "name": "voiceAssistantToggle",
        "type": 0,
        "command": "voiceAccess",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      },
      {
        "id": "1788160f-8b7e-4e69-8f17-f30b454e94a9",
        "enabled": true,
        "name": "openChat",
        "type": 0,
        "command": "displayChat",
        "overrideGlobalConfidence": false,
        "confidenceThreshold": 0.0,
        "stopAfter": false
      }
```

## [Coming Soon]