# Gaming Session Fitness Timer
A lightweight Bash background utility designed to help gamers stay active, maintain good posture, and balance health goals seamlessly with long gaming sessions.

## Project Goal
During long gaming sessions, it is incredibly easy to lose track of time and remain sedentary for hours, leading to poor posture and a lack of daily physical activity. This project solves that problem by running a lightweight timer utility in the background that automates movement reminders and tracks quick, mid-session micro-workouts.

## MVP Scope (Version 1.0)
The Minimum Viable Product includes the following core functionalities:
- **Background Timer Loop:** Continuously tracks time intervals using the native system `sleep` utility without interrupting system performance.
- **Random Exercise Selector:** Automatically picks a randomized short workout challenge from a predefined array list using `$RANDOM`.
- **Interactive Prompts:** Halts the timer to display terminal alerts and takes direct user input via `read` to confirm completion.
- **Local File Logging:** Automatically appends date-stamped completion metrics directly to a local CSV file via output redirection.

## Tech Stack
- **Language:** Bash Scripting (Bourne Again SHell)
- **Built-in Utilities:** `sleep`, `read`, `date`, `echo`, `printf`, `$RANDOM`
- **Data Storage:** Local plain text CSV file (`workout_log.csv`) utilizing standard `>>` file redirection operators.
- **External Dependencies:** None (Runs completely natively on standard Unix/Linux terminals).

## Future Plans (Version 2.0+)
Features planned for post-MVP iterations include:
- Implementing native desktop GUI notifications instead of terminal-bound text alerts.
- Creating a customizable workout routine profile editor to let users add their own movements.
- Generating automated weekly graphical progress report charts directly in the console.
