---
title: "Laser Tag on a Budget"
excerpt: "A fully functioning 4-player laser tag game with a $60 budget.<br/><img src='/images/laser_tag.jpg' width='500'>"
collection: portfolio
---

[GitHub Repo](https://github.com/ECE445L-Classroom/final-lab-tag_youre_it)<br>
[Go back](../)

Design Description
------
A medium-range, battery-powered, laser tag game fit with 4 custom blasters, 1 hub controlling the game, and 4 vests made out of cardboard all built from scratch using the TM4C microcontroller and Eagle PCB software without exceeding a $60 budget.<br><br>
**Skills:** _C, Firmware, UART, PCB Design, Eagle, Microcontrollers_

Technical Details
------
- **The Hub:** Equipped with an LCD display and RF antenna. A pregame lobby that allows the players to connect upon request. Can support up to 16 players per game. 4 game modes: 1-min 1v1, 3-min 1v1, 1-min teams, 3-min teams. When a player is connected, they are given a unique 4-bit ID, color, and player number, which are displayed upon a successful connection. When a game begins, the Hub will periodically update the score, current leaderboard, and time for all connected players via RF.
- **The Player:** Equipped with 3D printed IR blaster with a trigger switch, high-current narrow-beam IR LED, LCD display, RF antenna, and 8-ohm speaker. Upon powering up, a player will connect via RF. When a player connects, they are shown their player number and color. When the game begins, the LCD shows the player's score, rank, and game time (supplied by the Hub). Every time a player fires, their unique ID is encoded in their IR blast. The hit player will inform the Hub what 4-bit ID hit them. If the 4-bit ID is one of the registered players, then the Hub will update the global score and leaderboard. A sound is played every time a player fires or gets hit. At the end of the game, the final score and rank are displayed on the player's screen and the Hub is equipped to start another game!

Deliverables
------
- My team won the class design competition for Spring 2023!
- [Photos from the class project showcase](https://www.flickr.com/photos/utece/albums/72177720307763148/)
- _See the GitHub for hardware and software files._

Acknowledgments
------
Thank you Avyay, Vivek, and Vincent for being great teammates!