# routine
Recording workout routes, gym sessions, and stretching routines.


## Background
I spend most of my day at a desk working as an engineer, and recently I started getting back pain. I wanted a simple way to stay consistent with daily stretching, hoping it would help reduce the main. Something easy enough that I can make this into a habit.

I did not want to:

* install another app and learn how to use the app for tracking
* open my laptop everytime I make a recording
* type ssh into my laptop on my phone
* build and maintain a full product
* create a serious engineering project
* overengineer a personal habit tracker
* maintain anything day to day

I wanted something very lightweight.

## Solution

This project uses GitHub as a plain log repository (think of it as archive) and OpenAI ChatGPT to log data. Whenever I complete a stretch session, I ask ChatGPT to update the repo and commit the change.

Commit message format:

```logs: {date} morning```

```logs: {date} night```

* No GitHub Actions.
* No branching workflow.　(Don't be mad. This is not engineering repo)
* No separate app.
* No infrastructure to maintain.

## How It Works
Do stretching in the morning or night.
Ask ChatGPT to update the log.
ChatGPT commits directly while I’m logged in.
Git history becomes the timeline of consistency.

## Directroy Structure
logs/{date}.md
Readme.md

## Future Extensions
I might entend the future I can continue my stretch for 6 months. (well, it's still might and I cannot promise)
A few candidates are 
* Calendar Sync
* Visualization / Deep Analysis
