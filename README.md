


### Create a .env File

Create a file named `.env` in the root of your project. Add this line to the file:

```bash
export SLACK_TOKEN=replace_me
```

When we give you a Slack API token, replace `replace_me` with the token.

Once you have your token, open a terminal and type:

```bash
source .env
```

This will expose the variables in your `.env` file to the current terminal session. **You will need to 
type `source .env` for each new terminal window you open.** If you see this error `Missing configuration. Config must 
include either slackToken AND/OR clientId, clientSecret, and port` you forgot to type `source .env` :smile:

### Install Depedencies

Use `npm install` in the root of your project to install all the project dependencies.

## Start Your Bot

This project uses `npm` scripts to perform tasks. You can find them in the `package.json` file.

Type `npm start` in a terminal window to start your bot. Find your bot in Slack and it should have a green active icon next to it. If you don't see that, check your terminal for logs (did you remember to `source .env`?).

In Slack type `hello bot` and see if it responds. You can also type `@<botname> help` to see what help commands it has.

Heads up: your bot will restart on every code change. This is a great feature for development, not so useful in production :smile:

## First Exercise

Once you have your bot running, it's time to dig in! Take a look at the README in this branch for the first exercise: 
https://github.com/SparkPost/pizza-bot/tree/01-plugin
