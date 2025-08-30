# Pomodoro Timer

A simple Pomodoro timer application built with Python and `tkinter`. This app uses the Pomodoro technique to help you focus on your tasks by splitting work sessions into intervals, typically 25 minutes, separated by short breaks. After completing a set of 8 sessions, a longer break is given.

## Features

- **Work Sessions**: Starts a 25-minute work session.
- **Break Sessions**: Short breaks (5 minutes) and long breaks (20 minutes) after a set of work sessions.
- **Session Tracking**: Keeps track of completed work sessions and provides progress feedback.
- **Sound Alerts**: Beeps to notify the user when it's time to work or take a break.
- **Message Alerts**: Shows a message box when a break or work session starts.

## Requirements

- Python 3.x
- `tkinter` (comes pre-installed with Python)
- `winsound` (for sound alerts)

## How to Run

1. Clone this repository or download the files to your local machine.
2. Run the Python script:

    ```bash
    python pomodoro_timer.py
    ```

## Code Explanation

### `start_timer()`
This function:
- Starts the countdown for work, short break, or long break depending on the current session.
- Disables the start button during the countdown.

### `count_down(count)`
- Updates the timer every second.
- When the timer reaches zero, it plays a beep sound and starts the next session.

### `reset_timer()`
- Resets the timer to "00:00" and stops the current session.
- Resets the session counter and allows the user to start fresh.

### `show_work_message()` and `show_break_message()`
- Shows message boxes when the user starts a work session or break.
- Plays a beep sound using `winsound`.

### Long Break
After completing 8 work sessions, a long break (20 minutes) is taken, and a session summary is shown.

## Contributing

Feel free to submit issues or pull requests if you have improvements or bug fixes.
