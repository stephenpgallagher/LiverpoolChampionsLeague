# Plotting Important Goals in Liverpool's 2018/19 Champions League Run

This project is an extension of a positional data analysis done by the Friends of Tracking initiative, which can be found at https://github.com/Friends-of-Tracking-Data-FoTD/Last-Row.

In this project we hand-pick certain goals scored in in Liverpool's 2018/19 Champions League run.
We use voronoi diagrams to divide the spaces on the pitch in to zones. Each player’s zone is the area of the pitch that is closer to that player than to any other. In other words, it is the area of the pitch they control at a specific moment.

The dataset used here is ``liverpool_2019.csv``, which contains 19 goals scored by Livepool FC in 2019.

Columns included:
* ``play``: the scoreline after the goal. The team who scored the goal is the one next to the brackets.
* ``frame``: the frame number for the current location. Data provided has 20 frames per second.
* ``player``: the id of the player. The id is consistent within a play but **not between plays**.
* ``player_num``: the player jersey number. This number is the official one, and did not change for Liverpool in 2019.
* ``x``, ``y``: coordinates for the player/ball. Pitch coordinates go from 0 to 100 on each axis.
* ``dx``, ``dx``: change in (x,y) coordinates from last frame to current frame
* ``z``: height, from 0 to 1.5 (only filled for the ball)
* ``bgcolor``: the main color for the team (used as background color)
* ``edgecolor`` the secondary color (used as edge color)
