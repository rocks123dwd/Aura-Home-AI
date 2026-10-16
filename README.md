# Aura Home AI

A house AI you connect to your home. Ask it questions, tell it what to do, and it controls your smart devices (lights and the like) through its own device-control layer. No Home Assistant dependency.

> **Status:** early development. Core chat and device control work; memory does not exist yet.

## Features

- **Conversational assistant**: ask questions in plain English, powered by the [Groq API](https://groq.com/).
- **Smart device control**: switch lights and other devices on and off by asking.
- **Custom control code**: talks to devices directly rather than building on top of Home Assistant.
- **Shared storage**: designed to keep data on a household NAS.

## Not yet implemented

- Persistent memory (it forgets everything between conversations)

## Requirements

- Python or Node runtime (fill in whichever the project uses)
- A Groq API key
- Smart devices reachable on your local network
- (Optional) A NAS or shared drive for data storage

## Setup

```bash
git clone <your-repo-url> aura
cd aura
```

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_key_here
```

Install dependencies and run:

```bash
# Replace with the actual commands for your stack
<install command>
<run command>
```

## Usage

Once running, talk to it:

```
> turn off the living room lights
> what's the capital of Australia?
```

## Configuration

| Setting | Description |
| --- | --- |
| `GROQ_API_KEY` | API key used for AI responses |

Device definitions (names, rooms, protocols) live in the project's device config. Add your devices there so Aura can find them.

## Roadmap

- [ ] Conversation memory
- [ ] More device types
- [ ] NAS-backed data storage
- [ ] Rebrand to **Astra Home**

## Security

Never commit your `.env` file or API keys. Aura can control physical devices, so keep it on a trusted network and don't expose it to the internet without authentication.

## Built with

Groq API and [Claude Code](https://claude.com/claude-code).
