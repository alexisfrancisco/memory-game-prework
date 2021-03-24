# Pre-work - _Memory Game_

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program.

Submitted by: Alexis Francisco

Time spent: 4 hours spent in total

Link to project: https://glitch.com/edit/#!/quilted-vanilla-mimosa

## Required Functionality

The following **required** functionality is complete:

- [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
- [x] "Start" button toggles between "Start" and "Stop" when clicked.
- [x] Game buttons each light up and play a sound when clicked.
- [x] Computer plays back sequence of clues including sound and visual cue for each button
- [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess.
- [x] User wins the game after guessing a complete pattern
- [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

- [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
- [x] Buttons use a pitch (frequency) other than the ones in the tutorial
- [ ] More than 4 functional game buttons
- [x] Playback speeds up on each turn
- [x] Computer picks a different pattern each time the game is played
- [x] Player only loses after 3 mistakes (instead of on the first mistake)
- [ ] Game button appearance change goes beyond color (e.g. add an image)
- [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
- [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [x] I added an alert message each time the user gets a strike before losing

## Video Walkthrough

Here's a walkthrough of Memory Game:
![](http://g.recordit.co/MnAXSKPrbv.gif)

## Reflection Questions

1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.

   https://www.w3schools.com/
   
   https://www.c-sharpcorner.com/blogs/initializing-empty-arrays-in-javascript1
   
   https://developer.mozilla.org/en-US/docs/web/javascript/reference/global_objects/math/random

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words)

   One challenge that I encountered in my submission was that at one point, none of my colored buttons were working and would not register as "user guessed: _insert button num_" in the console and would instead give me an error. The very first line I checked were my button elements in my index.html file, since those what trigger the button press in the first place. When I found that the code had no typos, I figured that there was an error being caused by something in the script.js file that would not allow for the program to initiate properly. In order to figure out where I had gone wrong, I would debug the code by commenting out one function at a time, starting with the most recent function, in order to see if my program would run without the error in earlier iterations of my code. I found the error rather quickly within my guess function, as I forgot to pass in the btn variable through the function, resulting in the error. After realizing this I edited the code to pass the btn variable through the function and made sure to carefully read over and test my functions after completing them. Learning from this ultimately helped me add more features onto my code as it showed me to troubleshoot in groups and have a better understanding of how to solve problems in javascript.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)

   I would love to learn more about styling and formatting web pages and overall learn more about how CSS can improve a webpage. I have always wanted to learn more about the ways people create clean user interfaces in web development and would love to be able to tinker with some styling options that were not introduced in this project. I would also love to learn more about frameworks such as Node.js or React.js and how they can be implemented to create a more dynamic and responsive website. Knowing that some of the most popular websites and social media platforms are using these frameworks, I am interested in learning more about how these frameworks have added on to their webpages’ functionalities and created an overall better experience for their users. 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)

   If I had a few more hours to work on this, I would add a feature that would allow the user to select their difficulty (easy, medium, or hard) and have the timing of the playback and the number of steps in the hidden pattern change based on the difficulty chosen. For this, I would make it so that the easiest game mode has no shortened playback and have less iterations of their pattern, while hard would have a shorter playback hold and more iterations to solve the pattern. This would make it so that users can have more difficult modes in case they decide that the current mode is too easy for them.

   Another feature I would like to add is an "infinite" game mode, which would be a form of the memory game that would go on infinitely until the player misses a guess, similar to how the classic Simon game is played. With this infinite game mode, there would be a counter at the top of the screen that would record the user's current number of best guesses and another counter next to it that would record the user’s best record in the game. This game would also gradually shorten the playback hold over time (until a reasonable limit), making it more difficult to keep track of the pattern as the game progresses. Like the last feature, this would add a sense of competition into the game, allowing users to keep track of their progress and motivate them to compete against their previous score and keep playing the game.

## License

    Copyright Alexis Francisco

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
