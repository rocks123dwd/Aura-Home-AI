# Aura Home

Aura is a house AI made by Meme. You talk to it like you'd talk to a person, and it answers questions and runs the devices around your home, starting with the lights.

It doesn't sit on top of Home Assistant. Aura has its own device-control code, so it talks to your gear directly and nothing else needs to be installed for it to work.

## What it does

- Answers questions in plain English, using the Groq API
- Turns lights and other smart devices on and off when you ask
- Keeps its data on the home NAS, so it stays in the house

## What it doesn't do yet

Aura has no memory. Every conversation starts from scratch, so it won't remember what you told it yesterday. That's the next thing on the list.

## Running it

Aura needs a Groq API key to think, and your devices need to be on the same network as the machine running it. Put the key in a `.env` file as `GROQ_API_KEY` and start it up.

## A word of caution

Aura controls real devices in a real house, so keep it on your home network and don't expose it to the internet.

## Credits

Made by Meme.

Aura is being rebranded as Astra Home.
