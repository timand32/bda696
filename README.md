# BDA696 Assignments

## Assignment #1

Main executable file located at ./apps/iris/iris.py.

## Assignment #2

Script located at scripts/batting_average.sql.

## Assignment #3

Main executable file located at ./assignments/hw3/app.py.

## Assignment #4

Main executable file located at ./assignments/hw4/app.py.

## Midterm

Main executable file located at ./assignments/midterm/midterm.py.

Report on different datasets by changing `TITLE` at the top of midterm.py.

Add new datasets in ./assignments/midterm/data/get_data.py.

## Assignment #5

Main executable file located at ./assignments/hw5/hw5.py.

./assignments/hw5/scripts/pitcher.sql should be ran first.

I tried the following starting pitcher stats (100-day stats and prior career stats):

1. IP (Innings Played)
2. GS (Games Started)
3. S9 (Strikeouts per 9 innings pitched)
4. H9 (Hits per 9 innings pitched)
5. H9 (Home runs per 9 innings pitched)
6. IP Ratio (home starting pitcher's IP/away starting pitcher's IP)

The following was used for the rest:

home starting pitcher's stat - away starting pitcher's stat

## Assignment #6

Everything should run after executing "docker-compose up" in the root directory, assuming baseball.sql is also in the root. Additionally, everything should get saved in a new "docker-output" folder (the only catch is that the script can't automatically open the browser now).

Note that you'll need to manually shut down the mariadb container, as I am unsure how to make that shut down when the other container finishes running (it might be somewhere in the lecture notes...).

I've included [this](https://github.com/vishnubob/wait-for-it) script from [this] Stack Overflow issue. I was running into issues when my main script tried running before the database service started.

The Python script ran at the end is my HW5 submission (I recall the professor saying we could do this instead of the task mentioned on the lecture slides).
