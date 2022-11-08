## Lab 09

- Name: Robert Croop
- Email: croop.@2 @wright.edu

## Part 1 Answers

- Make sure infinity is in your Lab09 folder in GitHub

## Part 2 Answers

1. Getting started
   - Command to find the PID: look in task manager
   - PID of "Terminal A": 13928
   - PID of "Terminal B": 7956
2. Using `./` to run `infinity` in Terminal B
   - PID of script: 8426
   - Command to kill script: kill 8426
   - Effects of running the script: Cannot use terminal
3. Using `source` to run `infinity` in Terminal B
   - PID of script: 8327
   - Command to kill the script: kill 8327
   - Effects of killing the script: all the sub-processes
4. Running `infinity` as a background job in Terminal B
   - Command to run script in background: bash infinity.sh &
   - Job ID of script: 1
   - PID of script: 9007
   - Command to kill script via job id: kill %1
   - Effects of exiting terminal: The process is terminated
5. Run `infinity` in a `screen` or `tmux` session
   - Command(s) to run `infinity` in a screen session: bash infinity .sh (after screen is initialized)
   - Detach from `screen` / `tmux` session: CTRL, A, d
   - Command to show `screen` / `tmux` sessions: screen -ls
   - Effects of exiting terminal: Still running, as it is sperate from the window
   - Command / steps to kill the `screen` / `tmux` session: fill the process inside the screen as normal

## Part 3 Answers

1. git branch updates
2. git checkpout updates
3. navigate and edit as normal
4. git push --set-upstream origin updates
5. Confirmed? No
6.
7.
8.
9. Confirmed?
10.
