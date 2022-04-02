# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Animesh Deb
Time spent: **4** hours spent in total

Link to project: (insert your link here, should start with https://glitch.com...)

## Required Functionality

The following **required** functionality is complete:

* [x ] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [ x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [ x] Game buttons each light up and play a sound when clicked. 
* [x ] Computer plays back sequence of clues including sound and visual cue for each button
* [ x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x ] User wins the game after guessing a complete pattern
* [x ] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ x] More than 4 functional game buttons
* [ x] Playback speeds up on each turn
* [x ] Computer picks a different pattern each time the game is played
* [x ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)


If you recorded multiple GIFs for all the implemented features, you can add them here:

![](https://i.imgur.com/JmVm3Kd.gif)
![](https://i.imgur.com/BY4NQiN.gif)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[https://www.w3schools.com/jsref/jsref_random.asp] 

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
[One major challenge that I faced was when I was doing the additional option of speeding up the cue playback on each turn. The problem was that the cueHoldTime variable didn't reset for succeeding games. This meant that after I finishd the first game and began another, this second game began with a fast speed right away. I understood that I didn't reset the value of cueHoldTime after decreasing its value each turn. This is why I resumed by placing "cueHoldTime=1000;" after the for loop in the function playClueSequence(). I thought that by placing the said code after the for loop, the variable cueHoldTime would be reinitialized to have the value 1000 and this in turn would cause succeeding games to start off with a normal speed. However, this method didn't work. After thinking for some time, I realized that when a new game began, startGame() ran, and this function basically reinitialized variables for each turn. This gave me the idea to place "cueHoldTime=1000;" in the startGame() function instead of in the playClueSequence(). The idea was that when startGame() is called at the beginning of each turn, the speed would be set to normal or at the default value. After testing out numerous games, I discovered that this method worked. ]

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
[ How would you use python or c++ to do some of the things that were done using javascript, such as making the sounds and switching the colors of the buttons when they get pressed/ unpressed? I am interested in knowing about this because I haven't learned web development specific programming from the perspectives of c++ and python yet. Another question is how would you implement security features for websites? How would you also build a contact aspect in a website using javascript? By this, I mean having an area in a website where users can input their contact information so that you can reach them. How would you store the contact information securly using javascript? ]

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
[If I had additional time, I would possible make each button sound like different musical instruments. I think this would be a great way to further entertain the players and keep them heavily engaged. I also think that by having each button sound a different instrument, the project would serve as a warm up in helping me understand the very basics of a musical application, which I am interested in exploring. Another equally possible idea is to have voicelines for when players win or lose. So if they win, a voice line would congratulate them and if they lose, a voice line would say that they lost. I like this idea particularly because it adds a subtle depth to this basic game.]



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright [Animesh Deb]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.