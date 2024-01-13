# Battleship practice project

This repo is designed to be a challenge for anyone trying to start in the coding world or to enhance their skills.

Designed to be implemented in `python3`.

The challenge will consist of several points that sum to a grade of quality by a judge (only me at the moment). This will range in difficulty and should help anyone to improve.

# Summary

The challenge consists of creating a battleship Game that is playable from 0 to 2 persons.

- Player vs Player
- Player vs AI
- AI vs AI

You can find the Battleship game rules [>here<](https://www.thesprucecrafts.com/the-basic-rules-of-battleship-411069)

# Challenge Points

## Required

- [ ] Fork this repo
- [ ] Make it so the user can send its input as `A1`, `F6` and so on
- [ ] The AI must be able to play using randomly generated input (aka not very smart moves)
- [ ] The Game must be able to start and finish when one of the players has lost
- [ ] The Game must be turned based
- [ ] It must have some sort of GUI 
  - [ ] To start a game
  - [ ] To visualize what moves have been played
  - [ ] To visualize a winner
- [ ] Make a **happy path game** (Meaning if the player or AI behave properly and perfectly the game should start and finish no problem)
- [ ] Basic version control with readable commit messages

## Beginner

- [ ] Make the UI in the console using ascii characters, printable so the user can play the game vertically, (meaning on side of the board above the other) against the opponent
- [ ] Make the game using replayable, meaning play multiple games on a row
- [ ] Make the commit messages descriptive and relevant (keep a good version control of the program)
- [ ] Divide the program into reusable functions that make the code readable
- [ ] Edit the `Readme.md` file to have instructions on how to install (if required) and how to run it.
- [ ] Add `try-except` clauses so that it is able to handle **not happy paths** *i.e. the user sends something like `Z-1` which is not a valid input*

## Challenging

- [ ] Make the UI better, meaning able to be played horizontally to better display the board for each player
- [ ] Enhance the AI, so that it plays still randomly, but if it finds a battleship, keep attacking it until it destroys it
- [ ] Make the `Readme` file complaint with better *Markdown practices*
```bash
> # Something kind of like this
> # add lines like this so that it looks better for the readers
> # as an example
> python3 my_battleship_program.py
```
- [ ] Write logs of the games, record scores and moves from each player in a *directory/file* (I recommend the *logs/* directory, if it doesn't exist, it must be created)
- [ ] Make better `try-except` clauses, meaning instead of catching generic error types, catch specific error classes in your program
```python
# like so
try:
    # Do something
except ValueError:
    # Log that the user sent something weird and we log that specific error
except IndexError:
    # Some value is out of range, print why and where
except:
    # Some generic clause
```

## Advanced

- [ ] Make it portable, i.e. make it so that you are using `venv` or `conda` to install required packages and using the correct python version, this also means that you'll require a `requirements.txt` file to be added in the repo [reference](https://docs.python.org/es/3/library/venv.html)
- [ ] Write `unittests` that can be used to assert Quality in the program and prevent breaking changes
- [ ] Keep tags for versions of your code so that they can be downloaded by others [>Read this for reference<](https://www.atlassian.com/es/git/tutorials/inspecting-a-repository/git-tag)
- [ ] Write the program in an Object Oriented fashion, meaning instead of plain functions, make classes and objects that interact with each other in order to play a game
- [ ] Make the game pausable, meaning if the user inputs a command the game is saved in local storage to be continued later, can be a raw file, but I recommend using `pickle`
- [ ] Make it so that it can be run directly from the CLI with arguments, I recommend checking the `argparse` lib
```bash
# Kind of like this to play against an easy AI
python3 my-program.py --ai-level 1
# Kind of like this to play against an hard AI
python3 my-program.py --ai-level 2
# Or 2 players
python3 my-program.py --pvp
```
- [ ] Make better logs, there are libraries dedicated to printing logs, catching and documenting exceptions, etc, I recommend checking [loguru](https://github.com/Delgan/loguru)

## Very Hard

- [ ] Make an awesome UI using a library like `PyGame` or something along the lines
- [ ] Make a Github Action to test the repo's unittests in the cloud, in case anyone wants to contribute to your repo

## Impossible
- [ ] Make it playable online against another player using something like `Django`, mounting it on a server in `AWS`, `Firebase/GCP`, etc


#### Solution link

#### [Do not open till you have tried first!!](https://github.com/JOmarCuenca/battleship-practice-project-implementation)
