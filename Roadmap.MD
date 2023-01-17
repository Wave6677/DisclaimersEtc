# This roadmap is tentative and carries no guarentee that any of this will be done in any period of time specified.

## CarBar
### Q1 2023: Release a public alpha version within this scope:
* **Material You** support, including light and dark themes.
* **Bottom Bar Navigation**, featuring 4 custom app launcher buttons. Defaults being set as following:
* **Car Bar Notification Screen** - This will be built into CarBar. It will show the Android System notifcations, enlarged for easier viewing while driving. Features are planned for this screen beyond just notifications, but will most likely not be implimented in Q1 2023.
* **Default Navigation App** - CarBar will pull the system default navigation app. If there is none selected CarBar will prompt the user to install [Organic Maps](https://github.com/organicmaps/organicmaps)
* **Default Dialer App** - CarBar will pull the system default Dialer app. If there is none selected, CarBar will prompt the user to select an alternative app from the all apps list.
* **Music App** - Further research needs to be done, however if it is possible I'd like to have CarBar ask for a list of media apps, and give the user a selection from this list. If not the all apps list will be used.

### Q2 2023: Small improvements
This quarter will mostly be R&D with issues, and feature requests. I don't want to make promises I can't keep here.

### Q3 2023+: These features are wanted, but definitely not planned to be implimented anytime soon in any capacity.
* **Screen Reader Support** - This feature is for reading notifications, with options for only reading IM specific apps, and an app black/white list.
* **"Voice Assistant" Support**. The idea for this is using the VOSK Voice model to make responding to texts and navigating within your music and nav. apps easier, as well as quick location based searches, like "Restrooms near me" "Hotels in Springfield", and pulling from the users search engine of choice with location data. For example, when enabled, I basically plan to have it work like this:
- "Search for McDonald's Near me" -> Vosk STT -> Pull current location -> https://search.brave.com/?q=mcdonalds+near+Springfield -A-> TTS Responds: "The closest mcdonalds is in 3.7 miles. Would you like to start navigation?" -1-> "Yes" -> TTS: "Starting Navigation to {Address}" -> Sends request to default/selected Nav app.
- -B-> TTS Responds "No McDonald's found. Would you like to try another search?" -> End
- -2-> "No" -> TTS: "Would you like to try another search?" -> "No" -> End

### Don't expect anytime soon: Raspberry Pi <4 HeadUnit, a-la Android Auto Headunit.
**This is outside my current expectations for my skills within the next year.** However, I'd still like to research it and see if I can make it work for fun. Basically, if possible I'd like to make companion software for the Raspberry Pi, and have it work as a 3rd party drop in replacement for Stock car stereos. This will complete the other side of features specific to android auto headunits. Being able to sync with the phone for information. This feature is currently **only an idea.** I don't know how difficult it will be to make a custom harness for a Pi to fit my car, and how difficult it will be to program features like in built steering wheel controls, or auto starting when the car is on, and turning off when the car turns off, and if I'd need to include a custom android build to get those features working or not. 

## BPR (BladePlayerRevived)

### Q2 2023: Get a basic app working from the code of the old Blade Player.
* **Material You** - Basically redesign the entire app with Material You in mind. Taking inspiration from the Spotify App, YouTube Music App, and ViMusic. No definitive design is planned, as I will see how things feels when I get to it.
* **Fix Playback** - There's currently an issue with Blade Player that causes music playback to start ~.5 seconds after the track has actually started. It is very annoying and I want it fixed.

### Q3 2023+: Feature overhaul- The features here have no planned timeframe, but will be implemented in this order of priority.
* **Invidious support** - Add support to log into Invidious and import playlists. Invidious will also proxy the songs through Invidious. Instance support will feature a list of trusted instances will support to add your own.
* **Piped support** - Same as Invidious, not sure if I'll implement both. We'll see how I feel when I get there lol.
* **Music Caching** - Cache/download music for offline listening 
* **NewPipe Extractor Support** - "Okay, now you're just being extra, why do you need 3 ways to get to YouTube? You haven't even included a way to get to YouTube Music." I know, but the NPE has support for SoundCloud and BandCamp. The extractor wil be used to grab these sources unless I become aware of a better solution that proxies these sources for privacy.
* **Syncronised Lyrics Support** - I'd like to implement the same [synced lyrics provider](https://www.kugou.com/) [ViMusic](https://github.com/vfsfitvnm/ViMusic/) uses, as it seems to work pretty well. In addition I may also see how [InnerTune](https://github.com/z-huang/InnerTune) uses unsynced lyrics, and possibly implement a custom GitHub repo for users to source their own lyrics if they don't exist on these platforms.
* **Currently Listening Service & Listening tracker** - The whole reason I want FOSS spotify support is because I like the social features of Spotify. Linking to other services to allow people to see what you're listening to on that service, and spotify wrapped are really cool concepts to me. I'd like to possibly implement these features on my own, with privacy in mind. For now I will allow Spotify to be what takes care of these services (obviously only if you log into your spotify.) but in the future I'd like to see if I can tackle these small oddities on my own.
* **CarBar Integration** - If i have an app ecosystem, i might as well find ways to make them play nice together.

## Everything after this point is only ideas. They are not projects that I have any true timeline or roadmap for. They are simply ideas I want to persue at **some point**

### Profriend (E2E P2P FOSS Mental Health tool)
#### Planned features:
At this time this tool is only an idea with no planning of how it will work, or the logistics of making it. I only have ideas for the moment.
* **Premise** - A social app to keep track of your friends current state of mental health, current pronouns, current mood, current triggers, and current fronting alter(s) (for those with OSDD and DID). It will feature user made "profriendfiles" in which the user can specify all of the above information, and assign it a name and color.
* Android and iOS App
* Push Notifications based on when user changes profiles.
* j
