# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: James Laux

Time spent: 3 hours spent in total

Link to project: https://impartial-resilient-dietician.glitch.me

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!
1) "Your Turn" and "Computer Turn" Indicator
2) Total # of Guesses Made For the Turn and Total # of Guesses Needed For the Turn
3) Bind the buttons to keys on the keyboard for a more interactive experience
4) Endless mode -> Try to get a high score!
5) Clearly marked hover cursor that displays when you hover over a square

## Video Walkthrough

General + Losing Showcase:
https://cdn.glitch.com/7e4a182c-41ae-4b8c-b05c-9ec99b3cf5a3%2Flightsandsoundsdemo.gif?v=1616655197360

Random 8 Each Time Showcase
https://cdn.glitch.com/7e4a182c-41ae-4b8c-b05c-9ec99b3cf5a3%2Frandomset.gif?v=1616655214872

Winning Showcase
https://cdn.glitch.com/7e4a182c-41ae-4b8c-b05c-9ec99b3cf5a3%2Fwinning.gif?v=1616655234685

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
https://stackoverflow.com/questions/12482961/change-values-in-array-when-doing-foreach

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
Syntax in css was a big challenge for me. For instance, I was writing "btn1:lit", when it was supposed to be "btn1.lit" because it was something I was pushing to the class list.

Another challenge I've encountered was the sounds not playing in some instances. Still trying to figure that out.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
-I'm curious about how to setup User Login and track high scores. This seems like a great project for a local user, but I'm curious about the technologies I would need to use to make it save such information.
Not only save such information, but have it available if I close the window and then reopen it.


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
-For starters, I would reorganize a lot of the code in script.js. I think it could be organized in a much more human-readable way. For instance, I can organize the functions in the .js file by what part of the game they're related to and 
comment them as such (i.e. //button lighting).

-After making quality-of-life changes for myself and other developers, I will make quality-of-life changes for the User. This will include binding the 'asl;' keys to the left, middle left, middle right, and right buttons respectively.
  At the bottom of each button will be a visual reminder of the key its binded to. I will also create a "Your Turn" and "Computer Turn" indicator. I imagine doing that by having a <h1> element that contains "Your Turn" as "hidden", until
  the computer turn ends. The "Computer Turn" <h1> will be "hidden" until its turn begins. What will really tie this together is disabling pressing of buttons when it isn't the user's turn, avoiding weird behavior that could result from 
  pressing while the computer is going.

-Afterwards, I would work on Endless Mode, where the pattern is never-ending. The twist is that the turns get successively faster until a certain speed. The goal of this mode is to get the highest score possible. 
  To implement this, I would first have a toggle on the Start Screen between "Random 8" and "Random Infinite". "Random 8" is what's currently implemented. "Random Infinite", when selected upon "Start", will run the mode described above.
  There will be a score counter that gets incremented after each successful User Turn. This gets reset to 0 when User loses. The end screen will prominently display the Current Score.



## License

    Copyright James Laux

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.