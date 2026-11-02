# Scheduling-AI-Automation-Project
Appointment booking bot using a local LLM, n8n and Google Calendar

# Scheduling bot (local LLM + n8n)

Books, moves and cancels appointments from plain chat messages.
Built with n8n, Ollama (qwen3:4b, runs locally) and Google Calendar.

## How it works
The AI only extracts fields (action, date words, time, purpose).
Code checks each value appears in the user's message, calculates the
date, and decides what happens. Nothing is deleted unless exactly one
event matches.

## What went wrong first
- Limitation on performance - hosted locally on MacBook Pro M1 2020 with 8GB RAM
- [real example 2]
- [real example 3]

## Results
Tested on 20 messages: 18 passed on the first run,  after fixes.
(Test log: test-log.pdf) - link pdf

## Limitations
No confirmation step yet. Dates are read as the next occurrence.

## Demo
[video link] - .nmp4 file

## Run it yourself
Import scheduling-bot-v2.1.json into n8n, then select your own
Ollama credential, Google Calendar credential and calendar.
