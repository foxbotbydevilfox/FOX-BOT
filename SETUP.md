# FOX Setup Guide

This guide explains how to configure and run **FOX**, an all-in-one Discord bot made by **Devil Fox**.

## 1. Install Node.js

Use **Node.js 25** and npm.

Check the installed versions:

```bash
node -v
npm -v
```

## 2. Install Dependencies

Run this command in the project directory:

```bash
npm install
```

## 3. Configure Environment Variables

Create a file named `.env` in the project root. Add the values required by the project, such as:

```env
DISCORD_TOKEN=YOUR_DISCORD_BOT_TOKEN
CLIENT_ID=YOUR_CLIENT_ID
MONGO_URI=YOUR_MONGODB_URI
```

Use the variable names already expected by the source code. Never publish real credentials.

## 4. Configure the Bot

Review the project configuration files and set your preferred values:

- Default prefix: `?`
- Bot name: `FOX`
- Developer: `Devil Fox`
- Version: `1.0.0`
- License: `FOX`
- Footer: `Made By Devil Fox`
- Status: `Idle`
- Activity: `Listening - OWNER Devil Fox | /help`

## 5. Start the Bot

Start the bot with:

```bash
npm start
```

The project also includes these npm scripts:

```bash
npm run deploy
npm run format
```

Use the deploy script only when you need to register or update commands.

## 6. GitHub Upload Checklist

Before pushing the project to GitHub, confirm that these files are not uploaded:

- `.env`
- Bot tokens
- API keys
- MongoDB credentials
- Private keys
- Personal access tokens

Recommended `.gitignore` entries:

```gitignore
node_modules/
.env
.env.*
*.log
```

## 7. Support

- **Support server:** https://discord.gg/devil-s-den-1402859890502008904
- **GitHub:** https://github.com/foxbotbydevilfox/FOX-BOT/

**Made By Devil Fox**

## Central Configuration

Project branding and runtime presence settings are stored in `config.json`. To rebrand the bot, update the relevant values there, including `botName`, `developer`, `version`, `license`, `footerText`, `supportServer`, `github`, `embedColor`, `activity`, and `status`. Runtime embeds, help colors, bot information, and presence read from this configuration.
