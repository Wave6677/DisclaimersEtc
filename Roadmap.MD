This roadmap is tentative and carries no guarentee that any of this will be done in a ny period of time specified.

#CarBar
Q1 2023: Release a public alpha version within this scope:
* **Material You** support, including light and dark themes.
* **Bottom Bar Navigation**, featuring 4 custom app launcher buttons. Defaults being set as following:
* **Car Bar Notification Screen** - This will be built into CarBar. It will show the Android System notifcations, enlarged for easier viewing while driving. Features are planned for this screen beyond just notifications, but will most likely not be implimented in Q1 2023.
* **Default Navigation App** - CarBar will pull the system default navigation app. If there is none selected CarBar will prompt the user to install [Organic Maps](https://github.com/organicmaps/organicmaps)
* **Default Dialer App** - CarBar will pull the system default Dialer app. If there is none selected, CarBar will prompt the user to select an alternative app from the all apps list.
* **Music App** - Further research needs to be done, however if it is possible I'd like to have CarBar ask for a list of media apps, and give the user a selection from this list. If not the all apps list will be used.

Q2 2023: Small improvements
This quarter will mostly be R&D with issues, and feature requests. I don't want to make promises I can't keep here.

Q3 2023+: These features are wanted, but definitely not planned to be implimented anytime soon in any capacity.
* **Screen Reader Support** - This feature is for reading notifications, with options for only reading IM specific apps, and an app black/white list.
* **"Voice Assistant" Support**. The idea for this is using the VOSK Voice model to make responding to texts and navigating within your music and nav. apps easier, as well as quick location based searches, like "Restrooms near me" "Hotels in Springfield", and pulling from the users search engine of choice with location data. For example, when enabled, I basically plan to have it work like this:
- "Search for McDonald's Near me" -> Vosk STT -> Pull current location -> https://search.brave.com/?q=mcdonalds+near+Springfield -A-> TTS Responds: "The closest mcdonalds is in 3.7 miles. Would you like to start navigation?" -1-> "Yes" -> TTS: "Starting Navigation to {Address}" -> Sends request to default/selected Nav app.
- -B-> TTS Responds "No McDonald's found. Would you like to try another search?" -> End
- -2-> "No" -> TTS: "Would you like to try another search?" -> "No" -> End

Don't expect anytime soon: Raspberry Pi <4 HeadUnit, a-la Android Auto Headunit.
**This is outside my current expectations for my skills within the next year.** However, I'd still like to research it and see if I can make it work for fun. Basically, if possible I'd like to make companion software for the Raspberry Pi, and have it work as a 3rd party drop in replacement for Stock car stereos. This will complete the other side of features specific to android auto headunits. Being able to sync with the phone for information. This feature is currently **only an idea.** I don't know how difficult it will be to make a custom harness for a Pi to fit my car, and how difficult it will be to program features like in built steering wheel controls, or auto starting when the car is on, and turning off when the car turns off, and if I'd need to include a custom android build to get those features working or not. 

#BPR (BladePlayerRevived)

