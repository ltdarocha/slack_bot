<!---#
Create a Slackbot and deploy into Heroku
--->
# Create a Slackbot application to interact with Slack public channels/messages

Requirements:

- Have a Slack account

<!---
- Have a Heroku account
--->
To create a Slackbot you will have to create a Slack Application. Go to: https://api.slack.com/apps.

![image](https://imgur.com/v46QTjv.png)

Now you will have to "Add a bot User" into the created Application.

![image](https://imgur.com/ATPTdBq.png)

Install your App in your Slack Workspace.

![image](https://imgur.com/kgL9ZT8.png)

![image](https://imgur.com/yaJSOxw.png)

You will be given two authorization tokens. One for your bot and the other to interact with data in your Workspace. Do not share these tokens with anyone.

![image](https://imgur.com/Ba2XUq0.png)

To be able to use these tokens to send and fetch data from your public channels, you need to add the following Permission Scopes.

![image](https://imgur.com/3EyZmmp.png)

Now you are ready to use the Tokens and start building your own project to interact with your Slack messages and create a Slackbot.

<!---
![image](https://imgur.com/gq52tUQ.png)

### Deploy your bot in Heroku.

From the command line you will go inside the folder where your Slackbot code is in.

```
cd <path_to_your_code>
```

#### Important files to deploy your bot

Important files that have to be in the folder that contains your App code:

1) requirements.txt - this will contain packages version requirements from your python application

```
pip freeze > requirements.txt
```

2) runtime.txt - this file will contain the python version you are running your code

```
echo 'python-3.6.4' > runtime.txt
```

3) Procfile - this file will tell heroku which file it should run

```
echo 'worker: python slack_bot_app.py' > Procfile
```

#### Push bot to heroku

From command line:

```
heroku login
git init
heroku git:remote -a deploy-slack-bot (name of your heroku application)
git push heroku master
heroku ps:scale worker=1
```

slack6 image - add permisions
see which scopes are needed
save changes
reinstall app

make sure to add your bot to the channel


spotify:

install homebrew
pip install node
--->
