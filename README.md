# GitHub Actions Stale bot script 😴

![GitHub last commit (branch)](https://img.shields.io/github/last-commit/timothechauvet/stale-branch-bot/main)

## What's this 🤓
GitHub Action that I developed for a GitHub Enterprise Server (GHES) instance because the usual actions wouldn't work. 

It does that :
1. scans all branches every monday at 10am
2. detects which has commits from at least 30 days
3. pings each last-commiters in a single Issue

## Usage 🤖
1. Take out that .yml file
2. Put it in your repo under `.github/workflows`
3. Configure it
4. Enjoy

## Configuration ⚙️
You must configure these in the .yml directly since I'm not uploading it as a template

- `cron` (line 6) : Setup the frequency of each runs
- `runs-on` (line 14) : If you're on a GHES server, usually you would go with "self-hosted"
- `30 days` (lines 32, 35) : Time before the bot pings the users
- `api.github.com` (lines 44, 52, 65) : Change with your GHES server URL starting with "api."
- `comment_body` (lines 57-60) : Change the message, including the "github.com" urls
- `issues/1` (line 65) : Change the issue number that the bot would send messages to


## Contributions 🫵
For bugs, ideas or features requests, please submit an issue in this repository.

## Contact 🤗
- via LinkedIn : https://www.linkedin.com/in/timothechauvet/
- via Mail : timothe@chauvet.cloud
- or via an issue in this repository
